---
audience: end-user
title: AI Assistant - Content Accelerator 시작하기
description: AI Assistant - Content Accelerator 시작하기
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: ff46f8d9c0b46d5b74dee4317ade6a496841c408
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 20%

---

# AI Assistant - Content Accelerator 작업  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="AI Assistant Content Accelerator"
>abstract="AI Assistant를 사용하면 시간을 절약하고 효율성을 개선하며 더 나은 결과를 도출하는 동시에 직관적이고 단순하며 번거롭지 않은 이메일, SMS 및 푸시와 같은 채널 전반의 마케팅 캠페인을 만들고 실행할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko" text="릴리스 정보 참조"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 어시스턴트"
>abstract="게재 내용을 작성하고 개인화한 후 AI 어시스턴트를 사용하여 콘텐츠를 개선할 수 있습니다. 이 기능은 생성하려는 내용을 설명하여 콘텐츠를 미세 조정할 수 있도록 함으로써 개인화 및 콘텐츠 개선 프로세스를 간소화합니다."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign에서 AI 어시스턴트로 컨텍스트 정의"
>abstract="선택한 콘텐츠를 콘텐츠 생성을 위한 입력으로 사용하려면 **현재 콘텐츠로 개선** 토글을 활성화합니다. 또한 브랜드 자산을 업로드하여 소스로 사용할 수도 있습니다. 선택한 콘텐츠를 사용하지 않는 경우 브랜드 자산 업로드와 브랜드 자산 선택이 필수입니다."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 생성형 AI 약관"
>abstract="이 기능의 이용에는 Adobe Experience Cloud 생성형 AI 사용자 가이드라인에 대한 계약이 적용됩니다. 이 기능을 통한 모든 출력 내용이 정확한지 검토하고 사용 사례에 적합한지 확인해 보시기 바랍니다."
>additional-url="https://www.adobe.com/kr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 생성형 AI 사용자 가이드라인"

>[!INFO]
>
>기능을 직접 탐색하고 기능을 완전히 이해할 수 있도록 설계된 [대화형 데모](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator)를 통해 실습 경험에 몰입하세요.


마케팅 산업의 경쟁력이 높아짐에 따라 브랜드는 효과적인 콘텐츠를 효율적이고 빠르게 생성할 수 있는 효율적인 방법을 모색하고 있습니다. Microsoft Azure OpenAI 및 Adobe Firefly에서 제공하는 콘텐츠 가속용 Adobe Campaign 웹의 AI Assistant는 Adobe의 AI 콘텐츠 생성 기능으로, 마케터가 이메일, SMS, 푸시와 같은 채널 전반에서 전문적이고 브랜드 일관적인 콘텐츠를 만드는 방식을 혁신합니다. 고급 GenAI 모델과 브랜드 가이드라인에 대한 깊은 이해를 바탕으로 AI Assistant는 브랜드 윤곽이 잡힌 스타일, 레이아웃, 색조 등에 최적화된 콘텐츠로 마케팅 목표를 기반으로 개인화되고, 매력적이며, 효과적인 콘텐츠를 자동 생성합니다.

AI Assistant를 사용하면 시간을 절약하고 효율성을 개선하며 더 나은 결과를 도출하는 동시에 직관적이고 단순하며 번거롭지 않은 이메일, SMS 및 푸시와 같은 채널 전반의 마케팅 캠페인을 만들고 실행할 수 있습니다.

>[!IMPORTANT]
>
>* 이 기능의 사용을 시작하기 전에 관련 [보호 기능 및 제한 사항](#generative-guardrails)을 읽어 보십시오.
>
>* Content Acceleration을 위해 Adobe Campaign 웹에서 AI Assistant를 사용하려면 먼저 [사용자 계약](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)에 동의해야 합니다. 자세한 내용은 Adobe 담당자에게 문의하세요.

## AI Assistant - Content Accelerator 액세스 {#generative-access}

+++  콘텐츠 생성 관련 권한을 할당하는 방법을 알아봅니다

1. **제품 프로필 만들기** - [Admin Console](https://stage.adminconsole.adobe.com/)에서 다음 특정 패턴을 사용하여 제품 프로필을 만듭니다. `Campaign - <instance-name> - AIAssistant`

1. **사용자 추가** - 해당 제품 프로필에 필요한 사용자 추가,
또는

   **사용자 그룹을 만들고** 해당 사용자 그룹을 제품 프로필에 추가하고 사용자를 제품 프로필에 추가합니다.

+++

## 보호 기능 및 제한 사항 {#generative-guardrails}

Adobe Campaign Web for Content Acceleration에서 이메일 생성을 위해 AI Assistant를 사용하는 방법에 대한 일반 지침은 다음과 같습니다.

* 생성된 콘텐츠의 품질은 사용자가 정의하는 마케팅 목표/프롬프트의 영향을 많이 받습니다. GenAI 모델이 정확하게 해석할 수 있도록 잘 정의된 프롬프트를 사용하십시오. 
* 브랜드 에셋을 업로드하여 브랜드 콘텐츠에 정확하게 맞춥니다. 그 외의 경우 콘텐츠는 공개적으로 사용 가능한 정보를 기반으로 합니다. 업로드된 콘텐츠는 PDF, JPEG, PNG 또는 ZIP 파일(지원되는 파일 형식 포함) 형식일 수 있습니다.
* 업로드된 브랜드 자산의 최대 크기는 50MB입니다. 파일이 크거나 이미지가 많으면 작동할 수 있지만 처리 시간은 늘어납니다.
* [기본 제공 전자 메일 템플릿](../email/create-email-templates.md), 브랜드별 템플릿 또는 사용자 지정 템플릿을 사용하여 콘텐츠 가속기를 사용하여 전자 메일 콘텐츠를 만드십시오. 최대 8~10개의 이미지가 포함된 이메일 템플릿이 권장됩니다.
* 변형을 선택할 때 썸네일 업, 썸네일 다운 또는 플래그 아이콘을 사용하여 문제가 있는 출력을 보고해야 합니다.
* AI 비서 사용은 Adobe Experience Cloud 생성 AI 사용자 지침의 적용을 받습니다. [자세히 알아보기](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* 미디어 제작에서 생성 AI 도구 사용의 투명성을 증진하기 위한 Adobe의 약속의 일부로, Adobe은 Firefly 생성 에셋이 포함된 콘텐츠 또는 프로젝트를 다운로드하거나 내보낼 때 Content credentials을 적용합니다. [자세히 알아보기](https://helpx.adobe.com/firefly/using/content-credentials.html)

Adobe Campaign Web for Content Acceleration의 AI Assistant에는 다음과 같은 제한이 적용됩니다.

* Adobe Campaign Web for Content Acceleration의 AI Assistant는 현재 영어로만 지원됩니다. 영어가 아닌 입력은 일관되지 않거나 잘못된 결과를 생성할 수 있습니다. 비영어 응답에서 발생하는 문제는 현재 해결되거나 개선되지 않을 것입니다.
* 이메일, 푸시 및 SMS 채널에만 사용할 수 있습니다.
* GenAI 콘텐츠가 항상 정확하지는 않을 수 있습니다. 엔지니어가 모델을 세분화할 수 있도록 피드백을 공유하십시오.
* 여러 브랜드 자산을 업로드할 수 있지만 특정 세대에 대해 하나만 활용할 수 있습니다.

## AI Assistant 콘텐츠 생성 기능 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="이메일 생성" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI Assistant를 사용하여 전자 메일 생성</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS 생성" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>AI Assistant를 사용하여 SMS 생성</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="푸시 생성" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI 도우미를 사용하여 푸시 알림 생성</strong></a>
</div>
<p></td>
</tr></table>
