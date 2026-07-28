---
title: 맞춤형 필터 추가
description: 목록 보기의 필터 창에서 사용자 정의 필터를 빠른 액세스 필드로 추가하는 방법을 알아봅니다.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 맞춤형 필터 추가 {#custom-filters}

**[!UICONTROL 인벤토리 목록 구성]** > **[!UICONTROL 사용자 지정 필터]** 섹션에서 스키마 목록 보기의 [필터 창](../query/filter.md)에서 **[!UICONTROL 고급 필터]** 규칙 빌더 위에 빠른 액세스 필드로 표시되는 특성을 선택할 수 있습니다.

화면 정의 화면 및 액세스 방법에 대한 자세한 내용은 [화면 정의 액세스](schemas-browse-access.md#screen-def) 섹션을 참조하십시오.

## 맞춤형 필터 추가 {#add}

1. **[!UICONTROL 스키마]** 메뉴로 이동한 다음 필터를 사용하여 편집 가능한 스키마를 찾습니다.

1. 목록에서 스키마 이름을 선택하여 열고 스키마 세부 정보 보기에서 **[!UICONTROL 화면 편집]** 단추를 클릭하여 화면 정의에 액세스합니다.

1. **[!UICONTROL 인벤토리 목록 구성]** 섹션으로 이동하여 **[!UICONTROL 사용자 지정 필터]** 테이블 위의 줄임표 아이콘을 클릭한 다음 **[!UICONTROL 특성 선택]**&#x200B;을 선택합니다.

   ![사용자 지정 필터 선택](assets/schemas-custom-filters1.png)

1. 하나 이상의 속성을 선택하고 확인합니다.

   다음을 선택할 수 있습니다.

   * 스키마의 직접 속성(예: 코드 또는 범주).
   * 링크 속성(예: 제품에 연결된 브랜드). 이 경우 필터는 연결된 스키마로 제한된 검색 선택기를 사용합니다.
   * 링크의 하위 속성(예: 연결된 폴더의 전체 이름 또는 연결된 수신자의 이메일).

   ![직접 특성 및 링크 하위 특성을 표시하는 특성 선택기](assets/schemas-custom-filters2.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 위쪽 및 아래쪽 화살표를 사용하거나 필터를 드래그하여 사용자 정의 필터의 순서를 재지정하고 행의 휴지통 아이콘을 사용하여 필터를 제거할 수 있습니다.

1. 이 스키마에 대한 레코드 목록으로 이동한 후 필터 창을 엽니다. 선택한 특성은 **[!UICONTROL 고급 필터]** 규칙 빌더 위에 **[!UICONTROL 사용자 지정 필터]**(으)로 표시됩니다.

   ![필터 창에 표시되는 사용자 지정 필터](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >날짜 또는 날짜 및 시간 속성을 기반으로 하는 사용자 지정 필터가 날짜 범위 선택기로 표시됩니다.

1. 사용자 정의 필터 중 하나에 값을 입력하거나 선택하여 목록을 세분화합니다.

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->