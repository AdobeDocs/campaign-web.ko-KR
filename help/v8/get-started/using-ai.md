---
title: Campaign Web에서 AI 기반 상황별 도움말 사용
description: Campaign 웹 도움말 팝오버에서 질문하기
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: 577f4652-b3e5-4fa1-9a98-91815fe92d83
source-git-commit: b2de0d0061e5c2b582c3e73ccaf2dab1490cc854
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 14%

---

# AI 기반 상황별 도움말 {#using-ai}

제품 상황별 도움말 상자에서 제공되는 Q&amp;A AI 기반의 상황별 도움말을 사용하여 제품 설명서 및 현재 제품 컨텍스트를 기반으로 AI가 생성한 빠른 답변을 얻을 수 있습니다.

상황별 도움말에 포함된 **Gen AI의 상황별 도움말**&#x200B;은(는) 방대한 문서 리포지토리를 손쉽게 살펴보고 필요한 정확한 정보를 즉시 찾아내어 문서 검색 및 사용 방법 질문에 대한 답변을 혁신적으로 제공합니다.

Campaign Gen AI의 기능 덕분에 이 구성 요소는 사용자 경험을 향상시켜 정보 검색 및 문제 해결을 단순화합니다. 복잡한 작업에 대한 지침을 찾거나 광범위한 문서를 탐색하는 경우, AI 기반의 상황별 도움말은 모든 상호 작용에서 탁월한 효율성과 정확성을 제공하는 궁극적인 동반자 역할을 합니다.

<!--
[Animation showing AI-powered contextual help in action](assets/do-not-localize/CH+AI-BETA.gif)-->

>[!AVAILABILITY]
>
>* AI 기반의 상황별 도움말은 Beta 버전에서 사용할 수 있으며 사전 공지 없이 변경될 수 있습니다.
>
>* 이 기능은 **영어**&#x200B;로만 사용할 수 있습니다. 이 버전에서는 다른 언어가 지원되지 않습니다. 따라서 이 기능을 사용하기 전에 [기본 언어](connect-to-campaign.md#language-pref)가 영어로 설정되어 있는지 확인하십시오.
>
>* 지금은 Campaign 이메일 Designer에서 AI 기반의 상황별 도움말을 사용할 수 없습니다.

<!--
## Consent {#consent-ai}

Campaign knowledge assistant embedded in the contextual help boxes uses AI. Your use of this capability constitutes consent that the information you provide in your session will be collected, used, disclosed, and retained by Adobe in accordance with the terms of Adobe's Customer Feedback Program. Please do not provide any personal information about yourself or other parties (including your name or contact information) in the knowledge assistant.

## Privacy {#privacy-ai}

Your data is encrypted and private following our standard data protection practices. Learn more about [Adobe Privacy Policies](https://www.adobe.com/privacy/policy.html){target="_blank"}.

The knowledge assistant AI capability does not use your data to train our models. We do not allow any partners or third parties to use your data for training their models or any other purpose.

For information specific to Adobe AI policies in Experience Cloud apps and solutions, refer to [this page](https://business.adobe.com/products/sensei/adobe-sensei.html){target="_blank"}.
-->

## 추천 질문 {#questions-ai}

입력 필드에서 Adobe Campaign AI 기반의 상황별 도움말은 3가지 제안 질문을 제공합니다. 이러한 질문은 AI가 생성한 질문이며 도움말 상자와 관련이 있고 현재 제품 컨텍스트와 일치합니다. 답변을 확인하려면 질문을 선택합니다.

[상황별 도움말의 추천 질문 예](assets/do-not-localize/suggested-questions.png){width="600" align="left"}{zoomable="yes"}

## 답변 {#answers-ai}

Adobe Campaign AI 기반 상황별 도움말에서 도움을 제공하지만 사실을 확인해야 합니다. 이는 부정확하거나 오해의 소지가 있는 정보를 출력할 수 있습니다. 모든 도움말 상자에 연결된 제품 설명서를 항상 확인합니다.

도움말 팝오버 하단에 있는 **복사** 아이콘을 사용하여 클립보드에 대한 답변을 복사합니다.

[상황별 도움말의 답변 복사 예](assets/do-not-localize/copy-answer.png){width="600" align="left"}{zoomable="yes"}

## 피드백 {#feedback-ai}

인공 지능 및 머신 러닝 모델은 시간이 지남에 따라 개선되어 특정 사용 사례를 보다 잘 처리하게 됩니다. Campaign AI 기반의 상황별 도움말은 지속적으로 향상됩니다. 사용 <img src="assets/do-not-localize/thumb.png" width="10%"/>개의 단추를 사용하여 답변을 읽을 때마다 엔지니어에 부적절한 응답을 표시합니다.

## 추천 {#recommendations-ai}

AI 기반의 상황별 도움말에서 질문을 할 때는 현재 있는 화면, 현재 도움말 상자의 콘텐츠 등 현재 제품 컨텍스트가 고려됩니다.

결과적으로 가장 좋은 방법은 사용자 인터페이스 컨텍스트와 관련된 질문을 하는 것입니다. 예를 들어 워크플로우에서 푸시 게재를 보내는 방법을 알아보려면 **워크플로우** 왼쪽 메뉴 항목으로 이동하여 해당 컨텍스트에서 상황별 도움말 상자를 사용하십시오. 보고 지표에 대해 자세히 알아보려면 캠페인 또는 게재 보고서를 찾아 그 다음 단계에서 시작하십시오.

AI 기반의 상황별 도움말의 이점을 극대화하려면 다음 권장 사항을 따르십시오.

* 명확하고 구체적이며 모호함을 피하십시오. 정확한 대답은 명확한 질문에 따라 다릅니다.
* AI 기반의 상황별 도움말이 올바른 정보를 찾는 데 도움이 되도록 배우고자 하는 내용에 대한 자세한 정보를 제공합니다.
* 질문에 대한 구문을 변경하고 세분화하여 응답의 정확도를 향상시킵니다. 답변이 도움이 되지 않는다면 다른 접근 방법을 시도하고 컨텍스트를 추가하십시오.
* 중립적인 어조로 적절한 용어와 문구를 사용하십시오.
* 답변을 평가하고 피드백을 제공하여 엔지니어가 결과를 개선할 수 있도록 지원합니다.