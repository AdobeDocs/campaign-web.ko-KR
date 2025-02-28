---
title: 사용자 정의 필드
description: 사용자 정의 필드를 구성하는 방법 및 인터페이스에서 해당 가시성을 알아봅니다.
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 27e44682178267353418de210af51067eee4141b
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 24%

---


# 사용자 정의 필드 구성 {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="사용자 정의 세부 정보 편집"
>abstract="선택한 스키마의 인터페이스에 표시되는 모든 사용자 정의 필드가 표시됩니다. 위, 아래 화살표를 사용하여 인터페이스에 표시되는 순서를 변경하고, 구분자를 추가하여 필드를 하위 섹션으로 그룹화할 수 있습니다. 사용자 정의 필드를 삭제하거나 가시성 조건 등의 설정을 편집하려면 줄임표 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_general"
>title="일반"
>abstract="사용자 정의 필드의 일반 설정을 정의합니다. 레이블이 제공되지 않으면 스키마에 정의된 레이블이 표시됩니다. **다음의 경우 표시** 필드를 사용하여 필드가 표시되는 시기를 제어하는 xtk 표현식으로 조건을 정의합니다. 인터페이스에서 필드를 필수 또는 읽기 전용으로 표시할 수도 있습니다."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_link"
>title="링크 속성"
>abstract="쿼리 모델러를 사용하여 링크 유형 사용자 정의 필드를 표시하는 규칙을 지정합니다. 예를 들어 다른 필드의 입력에 따라 목록 값을 제한합니다."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_layout"
>title="레이아웃"
>abstract="기본적으로 사용자 정의 필드는 인터페이스에 두 개의 열로 표시됩니다. 이 옵션을 켜짐으로 토글하면 사용자 정의 필드가 두 개의 열 대신 전체 폭 화면으로 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_separatorproperties"
>title="구분자 속성"
>abstract="하위 섹션의 인터페이스에 표시할 이름을 지정합니다."

<!-- NOT USED IN THE UI?-->

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings"
>title="속성 설정"
>abstract="속성 설정"

사용자 지정 필드는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가된 추가 속성입니다. 조직의 요구 사항에 맞게 새 속성을 포함하여 스키마를 사용자 지정할 수 있습니다. [Adobe Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}에서 스키마를 확장하는 방법을 알아보세요.

사용자 지정 필드는 Campaign 웹 인터페이스의 프로필 세부 사항과 같은 다양한 화면에 표시할 수 있습니다. 관리자는 표시되는 필드와 표시 방법을 제어할 수 있습니다. 이러한 변경 사항은 모든 Campaign 사용자에게 적용됩니다.

>[!NOTE]
>
>사용자 정의 필드를 관리하려면 관리자 권한이 있어야 합니다.

사용자 정의 필드는 다음 스키마에서 사용할 수 있습니다.

* 캠페인(nms)
* 플랜(nms)
* 프로그램(nms)
* 수신자 (nms)
* 시드 주소(nms)
* 게재(nms)

## 인터페이스에 사용자 정의 필드 추가 {#add}

인터페이스에 사용자 지정 필드를 표시하려면 다음 단계를 수행합니다.

1. 왼쪽 탐색 창에서 **[!UICONTROL 스키마]** 메뉴로 이동하여 원하는 스키마를 찾습니다.

   필터 창의 **[!UICONTROL 편집 가능]** 필터를 사용하여 사용자 지정 필드가 있는 스키마를 빠르게 식별합니다.

   ![](assets/custom-fields-open.png)

1. 목록에서 스키마 이름을 선택하여 엽니다. 자세한 스키마 보기에는 [스키마 세부 정보에 대한 자세한 정보](../administration/schemas.md)가 표시됩니다. 사용자 정의 필드에 액세스하려면 **[!UICONTROL 사용자 정의 세부 정보 편집]** 단추를 클릭하십시오. 이 예제에서는 **[!UICONTROL 수신자]** 스키마에 대한 필드를 추가하려고 합니다.

   ![](assets/custom-fields-edit.png)

1. 스키마가 표시되도록 인터페이스에 표시되는 사용자 지정 필드 목록입니다. 여기에서 &quot;CRM ID&quot; 필드는 프로필의 세부 사항 화면에 표시되며 필수 항목으로 표시되어 있습니다.

   | 사용자 정의 필드 구성 | 인터페이스에서 렌더링 |
   |  ---  |  ---  |
   | ![](assets/custom-fields-detail.png){zoomable="yes"} | ![](assets/custom-fields-detail-crm.png){zoomable="yes"} |

1. 인터페이스에 사용자 지정 필드를 추가하려면 줄임표 버튼을 클릭하고 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 사용자 지정 필드 선택]**: 인터페이스에 표시할 사용자 지정 필드를 하나 이상 선택합니다.
   * **[!UICONTROL 사용자 지정 필드 목록을 자동으로 채우기]**: 스키마에 대해 정의된 모든 사용자 지정 필드를 인터페이스에 추가합니다.

   ![](assets/custom-fields-add.png)

1. 사용자 정의 필드가 추가되면 다음 작업을 수행할 수 있습니다.

   * **필드 순서 바꾸기**: 위쪽 및 아래쪽 화살표를 사용합니다.
   * **필수 필드 만들기**: **필수** 확인란을 선택합니다.
   * **필드 설정 편집**: 줄임표 버튼을 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택합니다. [자세히 알아보기](#settings)
   * **필드 삭제**: 줄임표 버튼을 클릭하고 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
   * **인터페이스의 하위 섹션으로 필드 구성**: 위쪽 및 아래쪽 화살표 옆에 있는 줄임표 단추를 클릭하고 **[!UICONTROL 구분 기호 추가]**&#x200B;를 선택하십시오. [자세히 알아보기](#separator)

## 사용자 정의 필드 설정 구성 {#settings}

각 사용자 지정 필드에 대한 특정 설정을 구성하려면 원하는 필드 옆에 있는 줄임표 버튼을 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

![](assets/custom-fields-settings.png)

사용 가능한 설정은 다음과 같습니다.

* **[!UICONTROL 특성]**: 사용자 지정 필드의 이름입니다.
* **[!UICONTROL 레이블(사용자 지정)]**: 인터페이스에 표시할 레이블입니다. 레이블이 제공되지 않으면 스키마에 정의된 레이블이 표시됩니다.
* **[!UICONTROL 보이는 경우]**: 필드가 표시되는 시기를 제어하는 xtk 식을 사용하여 조건을 정의합니다. 예를 들어 다른 필드가 비어 있으면 이 필드를 숨깁니다.
* **[!UICONTROL 필수]**: 인터페이스에서 필드를 필수 항목으로 만듭니다.
* **[!UICONTROL 읽기 전용]**: 인터페이스에서 필드를 읽기 전용으로 만듭니다. 사용자가 필드의 값을 편집할 수 없습니다.
* **[!UICONTROL 필터 설정]**(링크 유형 필드의 경우): 쿼리 모델러를 사용하여 링크 유형 사용자 지정 필드를 표시하는 규칙을 지정합니다. 예를 들어 다른 필드의 입력에 따라 목록 값을 제한합니다.

  `$(<field-name>)` 구문을 사용하여 조건의 다른 필드에 입력한 값을 참조할 수도 있습니다. 이렇게 하면 아직 데이터베이스에 저장되지 않은 경우에도 양식에 입력한 대로 필드의 현재 값을 참조할 수 있습니다.

  아래 예에서 조건은 @ref 필드의 값이 @refCom 필드에 입력한 값과 일치하는지 확인합니다. 반대로 `$(@refCom)` 대신 `@refCom`을(를) 사용하면 데이터베이스에 있는 @ref 필드의 값이 참조됩니다.

  +++보기 예

  ![](assets/custom-fields-ref.png)

+++

* **[!UICONTROL 두 열 분산]**: 기본적으로 사용자 지정 필드는 두 열로 인터페이스에 표시됩니다. 이 옵션을 켜짐으로 토글하면 사용자 정의 필드가 두 개의 열 대신 전체 폭 화면으로 표시됩니다.

## 하위 섹션의 사용자 정의 필드 구성 {#separator}

Campaign 웹 사용자 인터페이스를 사용하면 인터페이스에 사용자 지정 필드를 함께 그룹화하여 가독성을 높이기 위해 구분 기호를 추가할 수 있습니다. 이렇게 하려면 다음 단계를 수행합니다.

1. 위쪽 및 아래쪽 화살표 옆에 있는 줄임표 단추를 클릭하고 **[!UICONTROL 구분 기호 추가]**&#x200B;를 선택합니다.

1. 구분 기호를 나타내는 새 줄이 목록에 추가됩니다. 줄임표 버튼을 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택하여 하위 섹션 이름을 지정합니다.

1. 위쪽 및 아래쪽 화살표를 사용하여 구분 기호를 원하는 위치로 이동합니다. 구분 기호 아래에 나열된 필드는 그 아래에 그룹화됩니다.

   이 예에서 &quot;관심 있는 컬렉션&quot; 및 &quot;브랜드&quot; 필드는 &quot;컬렉션&quot; 하위 섹션으로 그룹화됩니다.

   | 사용자 정의 필드 구성 | 인터페이스에서 렌더링 |
   |  ---  |  ---  |
   | ![](assets/custom-fields-separator.png){zoomable="yes"} | ![](assets/custom-fields-section.png){zoomable="yes"} |
