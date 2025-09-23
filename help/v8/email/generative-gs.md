---
audience: end-user
title: AI 어시스턴트 시작하기
description: AI 어시스턴트 시작
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 22%

---

# AI 어시스턴트로 작업하기 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 어시스턴트"
>abstract="게재를 만들고 개인화한 후 AI 어시스턴트를 사용하여 콘텐츠를 더욱 풍부하게 만들 수 있습니다. 이 기능은 사용자가 생성하고자 하는 콘텐츠를 설명하여 콘텐츠를 세부 조정함으로써 개인화 및 콘텐츠 개선을 간소화합니다."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign에서 AI 어시스턴트로 컨텍스트 정의"
>abstract="선택한 콘텐츠를 콘텐츠 생성을 위한 입력으로 사용하려면 **현재 콘텐츠로 개선** 토글을 활성화합니다. 또한 브랜드 자산을 업로드하여 소스로 사용할 수도 있습니다. 선택한 콘텐츠를 사용하지 않는 경우 브랜드 자산 업로드 및 선택이 필수 작업으로 설정됩니다."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 생성형 AI 약관"
>abstract="이 기능에 대한 액세스 가능 여부는 Adobe Experience Cloud 생성형 AI 사용자 가이드라인에 대한 사용자의 동의 여부에 따라 달라집니다. 이 기능을 통한 모든 출력 내용이 정확한지 검토하고 사용 사례에 적합한지 확인해 보시기 바랍니다."
>additional-url="https://www.adobe.com/kr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 생성형 AI 사용자 가이드라인"

>[!INFO]
>
>기능을 직접 탐색하고 기능을 완전히 이해할 수 있도록 설계된 [라이브 기능 미리 보기](https://experienceleague.adobe.com/ko/apps/journey-optimizer/ai-assistant-content-accelerator)를 통해 실습 경험에 몰입하세요.

마케팅 업계의 경쟁이 치열해짐에 따라 브랜드는 효과적인 콘텐츠를 신속하게 생성할 수 있는 효율적인 방법을 모색합니다. Microsoft Azure OpenAI 및 Adobe Firefly에서 제공하는 Adobe Campaign 웹의 AI Assistant는 Adobe의 AI 콘텐츠 생성 기능으로, 마케터가 이메일, SMS 및 푸시 알림과 같은 채널 전반에서 전문적이고 브랜드 일관된 콘텐츠를 만드는 방법을 변환합니다. 고급 GenAI 모델과 브랜드 가이드라인에 대한 깊은 이해를 바탕으로 AI Assistant는 마케팅 목표를 기반으로 개인화되고, 매력적이며, 효과적인 콘텐츠를 자동 생성하여 브랜드에 설명된 스타일, 레이아웃, 색조 등에 맞게 콘텐츠를 최적화합니다.

AI Assistant는 이메일, SMS 및 푸시 알림과 같은 채널 전반의 마케팅 캠페인 생성 및 실행을 간소화하므로 시간을 절약하고 효율성을 향상시키며 더 나은 결과를 얻을 수 있습니다.

>[!IMPORTANT]
>
>* 이 기능을 사용하기 전에 관련 [보호 기능 및 제한 사항](#generative-guardrails)을 검토하십시오.
>
>* Adobe Campaign 웹에서 AI Assistant를 사용하기 전에 [사용자 계약](https://www.adobe.com/kr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)에 동의해야 합니다. 자세한 내용은 Adobe 담당자에게 문의하세요.

## AI Assistant 액세스 {#generative-access}

이메일, 푸시 알림 및 SMS용 AI Assistant는 이제 GA(일반 가용성)이며 모든 사용자가 사용할 수 있습니다. 사용자에게 액세스 권한을 부여하는 데 필요한 권한 및 단계는 아래에 자세히 설명되어 있습니다.

+++ 콘텐츠 생성 관련 권한을 할당하는 방법을 알아봅니다

1. **제품 프로필 만들기** - [Admin Console](https://stage.adminconsole.adobe.com/)에서 다음과 같은 특정 패턴을 사용하는 제품 프로필을 만드십시오.
   `Campaign - <instance-name> - AIAssistant`

1. **사용자 추가** - 필요한 사용자를 해당 제품 프로필에 추가하고,\
   또는\
   **사용자 그룹을 만들고** 제품 프로필에 해당 사용자 그룹을 추가한 다음 해당 제품 프로필에 사용자를 추가합니다.

[이 섹션](../get-started/permissions.md)에서 Campaign에서 권한을 정의하는 방법을 알아보세요.

+++

## 가드레일 및 제한 사항 {#generative-guardrails}

이메일 생성을 위해 Adobe Campaign 웹에서 AI Assistant를 사용하는 방법에 대한 일반 지침은 다음과 같습니다.

* 생성된 콘텐츠의 품질은 정의한 마케팅 목표 또는 프롬프트에 따라 크게 달라집니다. GenAI 모델이 정확하게 해석될 수 있도록 잘 정의된 프롬프트를 사용하십시오.
* 브랜드 에셋을 업로드하여 정확한 브랜드 내 콘텐츠를 확인합니다. 그렇지 않으면 콘텐츠는 공개적으로 사용 가능한 정보를 기반으로 합니다. 업로드된 콘텐츠는 PDF, JPEG, PNG 또는 ZIP 파일(지원되는 파일 형식 포함) 형식일 수 있습니다.
* 업로드된 브랜드 자산의 최대 크기는 50MB입니다. 파일이 크거나 이미지가 많으면 처리 시간이 길어질 수 있습니다.
* [기본 제공 전자 메일 템플릿](../content/create-email-templates.md), 브랜드별 템플릿 또는 사용자 지정 템플릿을 사용하여 AI Assistant를 사용하여 전자 메일 콘텐츠를 만드십시오. 최대 8~10개의 이미지가 포함된 이메일 템플릿이 권장됩니다.
* 변형을 선택할 때 엄지손가락 위로, 엄지손가락 아래로 또는 플래그 아이콘을 사용하여 문제가 있는 출력을 보고합니다.
* AI Assistant 사용 시 Adobe Experience Cloud 생성 AI 사용자 지침이 적용됩니다. [자세히 알아보기](https://www.adobe.com/kr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* 미디어 제작에서 생성 AI 도구 사용에 대한 Adobe의 투명성 약속의 일환으로, Adobe은 Firefly에서 생성한 에셋이 포함된 콘텐츠 또는 프로젝트를 다운로드하거나 내보낼 때 Content Credentials을 적용합니다. [자세히 알아보기](https://helpx.adobe.com/firefly/using/content-credentials.html).

Adobe Campaign 웹의 AI Assistant에는 다음과 같은 제한이 적용됩니다.

* Adobe Campaign 웹의 AI Assistant는 현재 영어로만 지원됩니다. 영어가 아닌 입력은 일관되지 않거나 잘못된 결과를 생성할 수 있습니다. 비영어 응답에서 발생하는 문제는 현재 해결되거나 개선되지 않을 것입니다.
* 이메일, 푸시 및 SMS 채널에만 사용할 수 있습니다.
* GenAI 콘텐츠가 항상 정확하지는 않을 수 있습니다. 엔지니어가 모델을 개선할 수 있도록 피드백을 공유하십시오.
* 여러 브랜드 자산을 업로드할 수 있지만 특정 세대에 대해 하나만 활용할 수 있습니다.

## AI Assistant 콘텐츠 생성 기능 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[AI Assistant를 사용하여 이메일 생성]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI Assistant를 사용하여 전자 메일 생성</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[AI Assistant를 사용하여 SMS 생성]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>AI Assistant를 사용하여 SMS 생성</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[AI Assistant를 사용하여 푸시 알림 생성]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI Assistant를 사용하여 푸시 알림 생성</strong></a>
</div>
<p></td>
</tr></table>