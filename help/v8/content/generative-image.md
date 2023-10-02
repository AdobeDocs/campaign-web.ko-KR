---
audience: end-user
title: 콘텐츠 도우미를 사용하여 이미지 생성
description: Content Assistant 시작
badge: label="Alpha"
source-git-commit: 2eea0827a1daf4af002587d09c11e2279aaf933c
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 2%

---


# 콘텐츠 도우미를 사용하여 이미지 생성 {#generative-image}

이메일을 만들고 개인화한 후에는 생성 AI에서 제공하는 콘텐츠 도우미를 사용하여 콘텐츠를 개선할 수 있습니다. 이 기능은 개인화 및 콘텐츠 개선 프로세스를 단순화합니다.

콘텐츠 도우미를 사용하여 이메일에서 이미지를 생성하고 개선하려면 아래 단계를 따르십시오. 에 설명된 대로 컨텐츠 도우미를 사용하여 전체 HTML 컨텐츠를 만들 수도 있습니다. [이 페이지](generative-email.md)에 설명된 대로 또는 텍스트 콘텐츠를 생성합니다. [이 페이지](generative-content.md).

>[!NOTE]
>
>이 기능의 사용을 시작하기 전에 관련 항목을 읽어 보십시오. [보호 및 제한 사항](generative-gs.md#guardrails-and-limitations).

아래 예에서는 Content Assistant를 활용하여 콘텐츠를 최적화하고 개선하여 보다 사용자 친화적인 환경을 구현하는 방법을 알아봅니다. 다음 단계를 수행하십시오.

1. 이메일 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**.

   이메일 게재를 구성하는 방법에 대한 자세한 내용은 을(를) 참조하십시오. [이 페이지](../content/create-email-content.md).

1. 다음을 입력합니다. **[!UICONTROL 기본 세부 정보]** 게재를 위해. 완료되면 다음을 클릭합니다. **[!UICONTROL 이메일 콘텐츠 편집]**.

1. 콘텐츠 도우미를 사용하여 변경할 에셋을 선택합니다.

1. 오른쪽 메뉴에서 **[!UICONTROL 경험 생성]**.

   ![](assets/image-genai-1.png)

1. 결과를 보다 세밀하게 조정하려면 프롬프트를 추가하십시오.

   ![](assets/image-genai-2.png)

1. 선택 **[!UICONTROL 파일 업로드]** 추가 컨텍스트를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 추가하려면 콘텐츠 도우미를 사용하십시오.

   다음을 클릭할 수도 있습니다. **[!UICONTROL 업로드된 콘텐츠]** 를 클릭하여 이전에 업데이트한 파일을 찾습니다. 업로드된 콘텐츠는 현재 사용자만 재사용할 수 있습니다.

1. 다음 항목 선택 **[!UICONTROL 종횡비]** 에셋. 에셋의 너비와 높이를 결정합니다.

   16:9, 4:3, 3:2 또는 1:1과 같은 일반적인 비율 중에서 선택할 수 있는 옵션이 있거나 사용자 지정 크기를 입력할 수 있습니다.

1. 사용자 지정 **[!UICONTROL 색상 및 톤]**, **[!UICONTROL 컨텐츠 유형]**, **[!UICONTROL 조명]** 및 **[!UICONTROL 컴포지션]** 원하는 에셋 특성과 일치하는 설정입니다.

   ![](assets/image-genai-3.png)

1. 프롬프트 구성이 만족스러우면 **[!UICONTROL 생성]**.

1. 찾아보기 **[!UICONTROL 변형 제안]** 원하는 자산을 찾습니다. 클릭 **[!UICONTROL 미리 보기]** 선택한 변형의 전체 화면 버전을 보려면 다음과 같이 하십시오.

   ![](assets/image-genai-5.png)

1. 클릭 **[!UICONTROL 선택]** 적절한 콘텐츠를 찾았으면

   ![](assets/image-genai-6.png)

1. 메시지 콘텐츠를 정의한 후 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다.  [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png)

1. 콘텐츠, 대상자 및 일정을 정의했으면 이메일 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)