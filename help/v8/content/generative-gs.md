---
audience: end-user
title: 콘텐츠 지원 시작하기
description: Content Assistant 시작
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: a34454c3c160f6a962fe064f35c26580bb7a4d94
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 34%

---

# 콘텐츠 지원 시작하기 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="콘텐츠 지원"
>abstract="게재 내용을 작성하고 개인화한 후에는 콘텐츠 지원을 사용하여 콘텐츠를 개선할 수 있습니다. 이 기능은 생성하려는 내용을 설명하여 콘텐츠를 미세 조정할 수 있도록 함으로써 개인화 및 콘텐츠 개선 프로세스를 간소화합니다."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="콘텐츠 생성을 위한 컨텍스트 정의"
>abstract="선택한 콘텐츠를 콘텐츠 생성을 위한 입력으로 사용하려면 **현재 콘텐츠로 개선** 토글을 활성화합니다. 또한 브랜드 자산을 업로드하여 소스로 사용할 수도 있습니다. 선택한 콘텐츠를 사용하지 않는 경우 브랜드 자산 업로드와 브랜드 자산 선택이 필수입니다."

생성 AI를 기반으로 하는 콘텐츠 도우미는 이메일 콘텐츠를 개선하는 데 유용한 도구입니다. 이는 개인화 및 콘텐츠 개선을 단순화하여 이메일 게재를 최적화하여 대상자에게 더 나은 공감을 줍니다.

이 기능은 전체 이메일 콘텐츠를 자동으로 생성하여 시간을 절약하고 일관된 품질을 보장합니다. 생성 AI를 사용하면 매력적인 이메일을 쉽게 만들 수 있으므로 커뮤니케이션의 효율성과 효율성을 향상시킬 수 있습니다.


이메일의 Campaign 콘텐츠 도우미에서 다음을 수행할 수 있습니다. [이미지 생성](generative-image.md), [텍스트 컨텐츠 생성](generative-content.md), [전체 HTML 컨텐츠 생성](generative-email.md).

>[!NOTE]
>
>이 기능은 Alpha 버전에서 사용할 수 있으며 사전 통지 없이 변경될 수 있습니다. 10월 초에 활성화될 예정입니다.

## 보호 기능 및 제한 사항 {#generative-guardrails}

전자 메일 생성을 위해 Content Assistant를 사용하는 방법에 대한 일반 지침은 다음과 같습니다.

* 생성된 콘텐츠의 품질은 사용자가 정의하는 마케팅 목표/프롬프트의 영향을 많이 받습니다. GenAI 모델이 정확하게 해석할 수 있도록 잘 정의된 프롬프트를 사용하십시오. 
* 브랜드 에셋을 업로드하여 브랜드 콘텐츠에 정확하게 맞춥니다. 그 외의 경우 콘텐츠는 공개적으로 사용 가능한 정보를 기반으로 합니다. 업로드된 콘텐츠는 PDF, JPEG, PNG 또는 ZIP 파일(지원되는 파일 형식 포함) 형식일 수 있습니다.
* 업로드된 브랜드 에셋의 권장 크기는 10MB 미만입니다. 파일이 크거나 이미지가 많으면 작동할 수 있지만 처리 시간은 늘어납니다.
* Adobe Campaign 작성 이메일 템플릿 사용(권장 사항) [기본 제공 전자 메일 템플릿](../content/email-sample-templates.md) 이메일 콘텐츠를 만듭니다. 이메일 템플릿에는 최대 8~10개의 이미지가 권장됩니다.


Campaign Content Assistant에는 다음 제한 사항이 적용됩니다.

* 지원되는 언어는 영어입니다.
* 이메일 채널에만 사용 가능
* GenAI 콘텐츠가 항상 정확하지는 않을 수 있습니다. 엔지니어가 모델을 개선할 수 있도록 피드백을 공유하십시오.
* 여러 브랜드 자산을 업로드할 수 있지만 특정 세대에 대해 하나만 활용할 수 있습니다



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="텍스트 생성" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>콘텐츠 지원을 사용하여 텍스트 생성</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="이미지 생성" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>콘텐츠 지원을 사용하여 이미지 생성</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="이메일 생성" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>콘텐츠 지원을 사용하여 이메일 생성</strong></a>
</div>
<p></td>
</tr></table>
