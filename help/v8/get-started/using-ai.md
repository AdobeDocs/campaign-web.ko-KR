---
title: Campaign Web에서 AI 기반 상황별 도움말 사용
description: Campaign 웹 도움말 팝오버에서 질문하기
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: 577f4652-b3e5-4fa1-9a98-91815fe92d83
source-git-commit: 2e5ddb7aca83a1a348ca50603d38a89c2762bb80
workflow-type: ht
source-wordcount: '0'
ht-degree: 100%

---

# AI 기반 상황별 도움말 {#using-ai}

제품 상황별 도움말 상자에서 사용할 수 있는 Q&amp;A AI 기반 상황별 도움말을 사용하여 제품 설명서 및 현재 제품 컨텍스트를 기반으로 AI 생성 답변을 빠르게 얻을 수 있습니다.

상황별 도움말에 임베드된 **생성형 AI 기반 상황별 도움말**&#x200B;은 설명서 검색을 혁신하고 방대한 설명서 저장소를 손쉽게 선별하여 필요한 정확한 정보를 즉시 찾아내는 방법에 대한 질문의 답변을 제공합니다.

Campaign 생성형 AI의 기능 덕분에 이 구성 요소는 사용자의 경험을 변화시켜 정보 검색 및 문제 해결을 용이하게 합니다. 복잡한 작업에서 지침을 구하거나 광범위한 문서를 탐색할 때 AI 기반 상황별 도움말은 모든 상호 작용에서 비교할 수 없는 효율성과 정확성을 제공하는 최고의 보조 앱입니다.

<img src="assets/do-not-localize/CH+AI-BETA.gif" width="80%"/>


>[!AVAILABILITY]
>
>* AI 기반 상황별 도움말 기능은 Beta 버전으로 사용할 수 있으며 사전 통지 없이 변경될 수 있습니다.
>
>* 이 기능은 **영어**&#x200B;로만 사용할 수 있습니다. 이 버전에서는 다른 언어가 지원되지 않습니다. 따라서 이 기능을 사용하기 전에 [선호 언어](connect-to-campaign.md#language-pref)를 영어로 설정해야 합니다.
>
>* 현재 Campaign 이메일 디자이너에서는 AI 기반 상황별 도움말을 사용할 수 없습니다.


<!--
## Consent {#consent-ai}

Campaign knowledge assistant embeeded in the contextual help boxes uses AI. Your use of this capability constitutes consent that the information you provide in your session will be collected, used, disclosed, and retained by Adobe in accordance with the terms of Adobe's Customer Feedback Program. Please do not provide any personal information about yourself or other parties (including your name or contact information) in the knowledge assistant.

## Privacy {#privacy-ai}

Your data is encrypted and private following our standard data protection practices. Learn more about [Adobe Privacy Policies](https://www.adobe.com/privacy/policy.html){target="_blank"}.

The knowledge assistant AI capability does not use your data to train our models. We do not allow any partners or 3rd parties to use your data for training their models or any other purpose.

For information specific to Adobe AI policies in Experience Cloud apps and solutions, refer to [this page](https://business.adobe.com/products/sensei/adobe-sensei.html){target="_blank"}.
-->

## 추천 질문 {#questions-ai}

입력 필드에서 Adobe Campaign AI 기반 상황별 도움말이 세 가지 추천 질문을 제공합니다. 이 질문은 AI에서 생성되며 도움말 상자 및 현재 제품 전후 상황과 관련이 있습니다. 답변을 확인하려면 질문을 선택합니다.

![상황별 도움말 추천 질문](assets/do-not-localize/suggested-questions.png){width="600" align="left"}{zoomable="yes"}


## 답변 {#answers-ai}

Adobe Campaign AI 기반 상황별 도움말에서 도움을 제공하지만 사실을 확인해야 합니다. 잘못된 정보, 부정확하거나 오해의 소지가 있는 답변이 출력될 수 있습니다. 모든 도움말 상자에 링크된 제품 설명서를 확인하십시오.

도움말 팝오버 아래쪽에 있는 **복사** 아이콘을 사용하여 답변을 클립보드에 복사할 수 있습니다.

![상황별 도움말 답변 복사](assets/do-not-localize/copy-answer.png){width="600" align="left"}{zoomable="yes"}


## 피드백 {#feedback-ai}

인공 지능 및 머신 러닝 모델은 시간이 지남에 따라 개선되어 특정 사용 사례를 보다 잘 처리하게 됩니다. Campaign AI 기반 상황별 도움말은 향후 몇 개월에 걸쳐 계속해서 개선될 예정입니다. 답변을 읽을 때 부적절한 응답이 있는 경우 <img src="assets/do-not-localize/thumb.png" width="10%"/> 버튼을 사용해 바로 엔지니어에게 알려주세요.

## 권장 사항  {#recommendations-ai}

AI 기반 상황별 도움말에 질문할 때 현재 제품 컨텍스트, 즉 현재 화면과 현재 도움말 상자의 내용이 고려됩니다.

결과적으로 가장 좋은 방법은 사용자 인터페이스 컨텍스트와 관련된 질문을 하는 것입니다. 예를 들어 워크플로에서 푸시 게재를 보내는 방법에 대해 알아보려면 **워크플로** 왼쪽 메뉴 항목을 찾은 다음 해당 특정 컨텍스트에서 상황별 도움말 상자를 사용하십시오. 보고 지표에 대해 자세히 알아보려면 캠페인 또는 게재 보고서를 찾은 다음 시작하십시오.

또한 AI 기반 상황별 도움말을 최대한 활용하려면 질문할 때 다음과 같은 사항이 권장됩니다.

* 최대한 정확하고 구체적으로 작성해야 하며 모호하지 않아야 합니다. 답변이 더욱 정확하고 유용할 것입니다.
* AI 기반 상황별 도움말이 올바른 정보를 찾을 수 있도록 배우려는 내용에 대해 가능한 한 많은 세부 정보를 추가하십시오.
* 더 나은 답변을 얻으려면 질문을 바꾸고 수정하십시오. 답변이 정확하지 않거나 유용하지 않은 경우 다양한 접근 방식을 시도하고 맥락을 추가하여 더 나은 결과를 얻어 보십시오.
* 중립적인 어조로 적절한 용어와 문구를 사용하십시오.
* 답변을 평가하고 피드백을 제공하여 엔지니어가 귀하의 경험을 통해 학습하고 결과를 개선할 수 있도록 하십시오.
