---
audience: end-user
title: 목록 찾아보기 및 필터링
description: Campaign Web v8 목록을 찾아보고 필터링하는 방법 살펴보기
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 44%

---

# 목록 찾아보기 및 필터링 {#list-screens}

왼쪽 탐색 메뉴의 링크 대부분은 **게재** 또는 **캠페인** 목록과 같은 개체 목록을 표시합니다. 이들 중 일부 목록 화면은 읽기 전용입니다. 아래 자세히 설명된 대로 목록 표시를 사용자 지정하고 이러한 목록을 필터링할 수 있습니다.

## 목록 화면 사용자 정의 {#custom-lists}

목록은 열에 표시됩니다. 열 구성을 변경하여 추가 정보를 표시할 수 있습니다. 이렇게 하려면 목록의 오른쪽 상단에 있는 **사용자 정의 레이아웃에 대한 열 구성** 아이콘을 클릭합니다.

[스크린샷은 목록 열의 레이아웃을 사용자 지정하는 데 사용되는 열 구성 아이콘을 보여 줍니다.](assets/config-columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

**열 구성** 화면에서 열을 추가 또는 제거하고 열이 표시되는 순서를 변경합니다.

아래와 같이 **드래그 앤 드롭**&#x200B;하거나 **위쪽 및 아래쪽 화살표**&#x200B;를 사용하여 목록의 순서를 변경할 수 있습니다.

[스크린샷은 드래그 앤 드롭 또는 화살표 단추를 사용하여 목록 열의 순서를 변경하는 방법을 보여 줍니다.](assets/list-reorder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

예를 들어 이 설정의 경우

[스크린샷은 열 구성 화면에 열 설정의 예제를 표시합니다.](assets/columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

목록에는 다음 열이 표시됩니다.

[스크린샷은 예제 설정에 따라 열이 구성된 결과 목록을 보여 줍니다.](assets/column-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

## 데이터 정렬 {#sort-lists}

열 머리글을 클릭하여 목록의 항목을 정렬할 수 있습니다. 목록이 해당 열에서 정렬됨을 나타내는 화살표(위쪽 또는 아래쪽)가 표시됩니다.

숫자 또는 날짜 열의 경우 **위쪽** 화살표는 목록이 오름차순으로 정렬됨을 나타내고 **아래쪽** 화살표는 내림차순으로 정렬됨을 나타냅니다. 문자열 또는 영숫자 열의 경우 값이 알파벳순으로 나열됩니다.

## 필터 {#list-built-in-filters}

항목을 더 빨리 찾으려면 검색 막대 또는 기본 제공 및 사용자 지정 필터를 사용하여 상황별 기준에 따라 목록을 조정하십시오.

[스크린샷은 목록 보기를 개선하는 데 사용할 수 있는 필터 옵션을 보여 줍니다.](assets/filter.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

필터를 사용하고 사용자 지정 필터를 만드는 방법에 대한 자세한 내용은 [이 섹션](../query/filter.md)에서 확인할 수 있습니다.

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