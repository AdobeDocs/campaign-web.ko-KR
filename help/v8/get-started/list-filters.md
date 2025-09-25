---
audience: end-user
title: 목록 찾아보기 및 필터링
description: Campaign Web v8 목록을 찾아보고 필터링하는 방법 살펴보기
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 1cec57c38b5f196db0881c498044fc9b999ed3b0
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# 목록 찾아보기 및 필터링 {#list-screens}

왼쪽 탐색 메뉴의 대부분 링크에는 **게재** 또는 **캠페인** 목록 등 오브젝트 목록이 표시됩니다. 이들 중 일부 목록 화면은 읽기 전용입니다. 아래 설명대로 목록 표시를 사용자 정의하고 해당 목록을 필터링할 수 있습니다.

## 목록 화면 사용자 정의 {#custom-lists}

목록은 열에 표시됩니다. 열 구성을 변경하여 추가 정보를 표시할 수 있습니다. 이렇게 하려면 목록의 오른쪽 상단에 있는 **사용자 정의 레이아웃에 대한 열 구성** 아이콘을 클릭합니다.

[목록 열의 레이아웃을 사용자 정의하는 데 사용되는 열 구성 아이콘을 보여 주는 스크린샷.](assets/config-columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

**열 구성** 화면에서 열을 추가 또는 제거하고 열이 표시되는 순서를 변경합니다.

아래와 같이 **드래그 앤 드롭**&#x200B;하거나 **위쪽 및 아래쪽 화살표**&#x200B;를 사용하여 목록의 순서를 변경할 수 있습니다.

[끌어다 놓기나 화살표 버튼을 사용하여 목록 열을 재정렬하는 방법을 보여 주는 스크린샷.](assets/list-reorder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

예를 들어 이 설정의 경우

[열 구성 화면의 열 설정 예를 보여 주는 스크린샷.](assets/columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

목록에는 다음 열이 표시됩니다.

[예제 설정에 따라 구성된 열이 포함된 결과 목록을 보여 주는 스크린샷.](assets/column-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

## 데이터 정렬 {#sort-lists}

열 머리글을 클릭하여 목록의 항목을 정렬할 수 있습니다. 목록이 해당 열에 정렬되어 있음을 나타내는 화살표(위 또는 아래)가 표시됩니다.

숫자 또는 날짜 열의 경우 **위쪽** 화살표는 목록이 오름차순으로 정렬됨을 나타내고 **아래쪽** 화살표는 내림차순으로 정렬됨을 나타냅니다. 문자열 또는 영숫자 열의 경우 값이 알파벳순으로 나열됩니다.

## 필터 {#list-built-in-filters}

검색 창을 사용하거나 기본 제공 필터 및 맞춤형 필터를 사용하여 상황별 기준에 따라 목록을 조정하여 항목을 더 빨리 찾습니다.

[목록 보기를 구체화하는 데 사용할 수 있는 필터 옵션을 보여 주는 스크린샷.](assets/filter.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

필터를 사용하고 나만의 맞춤형 필터를 만드는 방법에 대한 자세한 내용은 [이 섹션](../query/filter.md)에서 확인할 수 있습니다.

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

Only the most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes set as `advanced` attributes in the data schema are hidden from the configuration screens.

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list updates instantly.

[The screenshot shows the Display advanced attributes toggle used to reveal hidden attributes in the rule builder palette.](assets/adv-toggle.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}
-->