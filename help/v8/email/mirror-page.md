---
audience: end-user
title: 미러 페이지에 대한 링크 추가
description: 미러 페이지에 대한 링크를 추가하고 관리하는 방법 알아보기
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 16%

---

# 페이지 미러링 {#mirror-page}

미러 페이지는 이메일의 온라인 버전입니다. 이메일 마케팅에서 미러 페이지에 링크를 추가하는 것은 좋습니다. 예를 들어 받은 편지함에서 볼 때 렌더링 문제가 발생하거나 이미지가 손상된 경우 사용자는 이메일의 미러 페이지에 액세스할 수 있습니다. 또한 접근성이나 소셜 공유를 장려하기 위해 온라인 버전을 제공하는 것이 좋습니다.

Adobe Campaign에서 생성한 미러 페이지에는 모든 개인화 데이터가 포함됩니다.

![전자 메일의 미러 링크 샘플](assets/mirror-page-link.png){width="600" align="left"}

## 미러 페이지에 대한 링크 추가 {#link-to-mirror-page}

Adobe Campaign에서 전용 **개인화 블록**&#x200B;을(를) 사용하여 전자 메일 콘텐츠의 미러 페이지에 대한 링크를 삽입합니다. 기본 제공 **미러 페이지 링크** 개인 맞춤화 블록은 이메일 콘텐츠에 다음 코드를 삽입합니다. `<%@ include view='MirrorPage' %>`

이메일의 미러 페이지에 대한 링크를 추가하려면 다음 단계를 수행합니다.

1. 요소(텍스트 또는 이미지)를 선택하고 상황별 도구 모음에서 **[!UICONTROL 링크 삽입]**&#x200B;을 클릭합니다.

   ![링크 삽입 옵션을 표시하는 상황별 도구 모음](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. **[!UICONTROL 개인화 추가]** 아이콘을 선택하여 개인화 메뉴에 액세스합니다.

   Adobe Campaign의 ![Personalization 메뉴](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. **[!UICONTROL 조각]** 메뉴에서 **[!UICONTROL 미러 페이지 URL]**&#x200B;을(를) 선택하고 **[!UICONTROL 추가]**&#x200B;를 클릭합니다. [식 조각 사용 방법 알아보기](../content/use-expression-fragments.md)

   ![조각 메뉴의 미러 페이지 URL 옵션](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

미러 페이지가 자동으로 생성됩니다.

이메일이 전송되면 미러 페이지 링크를 클릭하는 수신자는 기본 웹 브라우저에 이메일 콘텐츠가 표시됩니다.

기본적으로 미러 페이지의 보존 기간은 **60일**&#x200B;입니다. 이 기간이 지나면 미러 페이지를 더 이상 사용할 수 없습니다.

>[!CAUTION]
>
>* 미러 페이지 링크는 자동으로 생성되며 편집할 수 없습니다. 여기에는 원본 이메일을 렌더링하는 데 필요한 암호화된 개인화된 모든 데이터가 포함됩니다. 값이 큰 개인화된 속성을 사용하면 미러 페이지 URL이 길어질 수 있으므로 최대 URL 길이로 웹 브라우저에서 링크가 작동하지 않을 수 있습니다.
>
>* 테스트 프로필로 전송된 증명에서 미러 페이지 링크가 활성화되지 않았습니다. 최종 메시지에서만 활성화됩니다.

## 미러 페이지 생성 {#mirror-page-generation}

기본적으로 Adobe Campaign은 이메일 콘텐츠가 비어 있지 않고 미러 페이지에 대한 링크(미러 링크라고도 함)가 포함된 경우 미러 페이지를 자동으로 생성합니다.

게재 속성에서 사용할 수 있는 옵션을 통해 이메일 미러 페이지의 생성 모드를 제어합니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#mirror)