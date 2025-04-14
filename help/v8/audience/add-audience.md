---
audience: end-user
title: 기존 대상자 선택
description: 대상자 선택 방법 알아보기
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 18%

---

# 기존 대상자 선택 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="기존 대상자 선택"
>abstract="목록을 찾아 기존 대상자를 선택합니다. “필터 표시” 아이콘을 사용하여 목록을 필터링하거나 특정 폴더를 선택합니다."

이 섹션에서는 게재의 대상 모집단을 정의할 때 기존 대상자를 선택하는 방법을 설명합니다. 게재의 기본 대상을 정의할 때 다음을 수행할 수도 있습니다.
* 쿼리 모델러를 사용하여 [일회성 대상자를 만듭니다](one-time-audience.md).
* [외부 파일에서 대상자를 로드합니다](file-audience.md)(전자 메일 전용).

게재에서 타깃팅할 수 있는 대상은 **대상** 왼쪽 메뉴에서 액세스할 수 있습니다. 이는 클라이언트 콘솔, Campaign 웹 대상자 워크플로 또는 Adobe Experience Platform과 같은 여러 소스에서 생성됩니다. [대상자에 대해 자세히 알아보기](manage-audience.md)

메시지의 기존 대상자를 선택하려면 아래 단계를 따르십시오.

1. 게재 만들기 도우미의 **대상** 섹션에서 **[!UICONTROL 대상 선택]** 단추를 클릭한 다음 **[!UICONTROL 대상 선택]**&#x200B;을 선택합니다.

   [이 스크린샷은 게재 만들기 도우미의 **대상 선택** 단추를 보여 줍니다.](assets/create-audience.png){zoomable="yes"}

1. 이 화면에는 현재 폴더의 기존 대상이 모두 표시됩니다.

   [이 스크린샷은 현재 폴더에 있는 기존 대상자 목록을 보여 줍니다.](assets/create-audience2.png){zoomable="yes"}

   Adobe Experience Platform에서 대상을 선택하려면 화면의 필터 섹션에서 `AEP Audiences folder`을(를) 찾아봅니다. [Adobe Experience Platform 대상에 대해 자세히 알아보기](manage-audience.md#monitor)

   [이 스크린샷은 AEP 대상 폴더가 선택된 필터 섹션을 보여 줍니다.](assets/select-audience-folder.png){zoomable="yes"}

1. 필터 섹션에서 필터링 옵션에 액세스하여 대상자 목록을 세분화할 수 있습니다. 이렇게 하려면 **규칙 추가**&#x200B;를 클릭하여 대상 목록에 대한 고급 필터를 만들 수 있는 쿼리 모델러에 액세스합니다. [쿼리 모델러를 사용하는 방법을 알아봅니다](../query/query-modeler-overview.md)

   예를 들어 아래와 같이 대상의 출처를 기준으로 필터링하는 규칙을 정의할 수 있습니다.

   [이 스크린샷은 원래 위치에 따라 대상에 적용된 필터를 보여 줍니다.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. 대상자를 게재 기본 대상으로 추가하려면 **확인**&#x200B;을 클릭합니다. 완료되면 **규칙 편집** 단추를 클릭하여 쿼리 모델러를 사용하여 대상을 세분화할 수 있습니다.

   [이 스크린샷은 대상자를 세분화하기 위한 **규칙 편집** 단추를 보여 줍니다.](assets/refine-audience.png){zoomable="yes"}

1. 캠페인의 영향을 측정하기 위해 컨트롤 그룹을 설정할 수도 있습니다. 컨트롤 그룹이 메시지를 받지 않습니다. 이를 통해 메시지를 받은 모집단의 동작을 받지 않은 연락처의 동작과 비교할 수 있습니다. [자세히 알아보기](control-group.md)