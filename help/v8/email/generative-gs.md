---
audience: end-user
title: AI Assistant 시작
description: AI Assistant 시작
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 33%

---

# AI Assistant 시작 {#generative-gs}

>[!BEGINSHADEBOX]

**목차**

* **[AI Assistant 시작](generative-gs.md)**
* [AI Assistant를 사용하여 이메일 생성](generative-content.md)
* [AI Assistant를 사용하여 SMS 생성](generative-sms.md)
* [AI Assistant를 사용하여 푸시 알림 생성](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="게재를 제작하고 개인화하면 AI Assistant를 사용하여 콘텐츠를 개선할 수 있습니다. 이 기능은 생성하려는 내용을 설명하여 콘텐츠를 미세 조정할 수 있도록 함으로써 개인화 및 콘텐츠 개선 프로세스를 간소화합니다."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign에서 AI Assistant를 사용하여 컨텍스트 정의"
>abstract="선택한 콘텐츠를 콘텐츠 생성을 위한 입력으로 사용하려면 **현재 콘텐츠로 개선** 토글을 활성화합니다. 또한 브랜드 자산을 업로드하여 소스로 사용할 수도 있습니다. 선택한 콘텐츠를 사용하지 않는 경우 브랜드 자산 업로드와 브랜드 자산 선택이 필수입니다."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 생성형 AI 약관"
>abstract="이 기능의 이용에는 Adobe Experience Cloud 생성형 AI 사용자 가이드라인에 대한 계약이 적용됩니다. 이 기능에 제공하는 모든 프롬프트, 컨텍스트, 추가 정보 또는 기타 입력 내용은 특정 컨텍스트와 연결되어야 하며, 여기에는 브랜딩 자료, 웹 사이트 콘텐츠, 데이터, 해당 데이터에 대한 스키마, 템플릿 또는 기타 신뢰할 수 있는 문서가 포함될 수 있으나 개인 정보는 포함되지 않아야 합니다(개인 정보에는 특정 개인 사용자와 다시 연결될 수 있는 모든 항목이 포함됨). 이 기능을 통한 모든 출력 내용이 정확한지 검토하고 사용 사례에 적합한지 확인해 보시기 바랍니다."
>additional-url="https://www.adobe.com/kr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 생성형 AI 사용자 가이드라인"

AI 어시스턴트는 이메일 콘텐츠를 개선하는 데 유용한 도구입니다. 이는 개인화 및 콘텐츠 개선을 단순화하여 이메일 게재를 최적화하여 대상자에게 더 나은 공감을 줍니다.

이 기능은 전체 이메일 콘텐츠를 자동으로 생성하여 시간을 절약하고 일관된 품질을 보장합니다. 생성 AI를 사용하면 매력적인 이메일을 쉽게 만들 수 있으므로 커뮤니케이션의 효율성과 효율성을 향상시킬 수 있습니다.

>[!NOTE]
>
>이 기능은 Alpha 버전에서 사용할 수 있으며 사전 공지 없이 변경될 수 있습니다. 10월 초에 활성화될 예정입니다.

## 보호 기능 및 제한 사항 {#generative-guardrails}

이메일 생성을 위해 Campaign에서 AI Assistant를 사용하는 방법에 대한 일반 지침은 다음과 같습니다.

* 생성된 콘텐츠의 품질은 사용자가 정의하는 마케팅 목표/프롬프트의 영향을 많이 받습니다. GenAI 모델이 정확하게 해석할 수 있도록 잘 정의된 프롬프트를 사용하십시오. 
* 브랜드 에셋을 업로드하여 브랜드 콘텐츠에 정확하게 맞춥니다. 그 외의 경우 콘텐츠는 공개적으로 사용 가능한 정보를 기반으로 합니다. 업로드된 콘텐츠는 PDF, JPEG, PNG 또는 ZIP 파일(지원되는 파일 형식 포함) 형식일 수 있습니다.
* 업로드된 브랜드 에셋의 권장 크기는 50MB 미만입니다. 파일이 크거나 이미지가 많으면 작동할 수 있지만 처리 시간은 늘어납니다.
* Adobe Campaign 작성 이메일 템플릿 사용(권장) [기본 제공 전자 메일 템플릿](../email/create-email-templates.md)이메일 콘텐츠를 만들기 위한 브랜드별 템플릿 또는 맞춤형 템플릿입니다. 이메일 템플릿에는 최대 8~10개의 이미지가 권장됩니다.


다음 제한 사항은 Campaign의 AI Assistant에 적용됩니다.

* 지원되는 언어는 영어입니다.
* 이메일, 푸시 및 SMS 채널에만 사용할 수 있습니다.
* GenAI 콘텐츠가 항상 정확하지는 않을 수 있습니다. 엔지니어가 모델을 세분화할 수 있도록 피드백을 공유하십시오.
* 여러 브랜드 자산을 업로드할 수 있지만 특정 세대에 대해 하나만 활용할 수 있습니다.



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="이메일 생성" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI Assistant를 사용하여 이메일 생성</strong></a>
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
<a href="generative-push.md"><strong>AI Assistant를 사용하여 푸시 알림 생성</strong></a>
</div>
<p></td>
</tr></table>
