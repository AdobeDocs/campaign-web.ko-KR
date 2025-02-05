---
audience: end-user
title: 이메일에 비주얼 조각 추가
description: 이메일에 시각적 조각을 추가하는 방법 알아보기
badge: label="제한 공개"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 14%

---

# 이메일에 비주얼 조각 추가 {#use-visual-fragments}

>[!AVAILABILITY]
>
>이 기능을 사용하려면 Campaign v8.6.4에 대한 업데이트가 필요합니다. 자세한 내용은 [Campaign v8 클라이언트 콘솔 릴리스 정보](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/releases/release-notes)를 참조하세요.

[이메일 게재](../email/get-started-email-designer.md) 또는 [콘텐츠 템플릿](../email/use-email-templates.md)에서 시각적 조각을 사용할 수 있습니다. 단계는 아래에 자세히 설명되어 있습니다.

![](assets/do-not-localize/fragments.gif)

>[!NOTE]
>
>[이 섹션](fragments.md)에서 콘텐츠 조각을 만들고 관리하는 방법을 알아봅니다.

## 시각적 조각 사용 {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="조각 옵션"
>abstract="이 창에서는 선택한 조각과 관련된 옵션을 사용할 수 있습니다. 이를 통해 조각을 표시할 디바이스를 선택하고 해당 조각의 콘텐츠를 열 수 있습니다. **[!UICONTROL 스타일]** 탭을 사용하여 조각을 더욱 세부적으로 맞춤화할 수 있습니다. 원본 시각적 조각으로 상속을 끊을 수도 있습니다."

<!-- pas vu dans l'UI-->

이메일 콘텐츠에 시각적 조각을 삽입하려면 아래 단계를 수행합니다.

1. [전자 메일 Designer](../email/get-started-email-designer.md)을(를) 사용하여 전자 메일 또는 템플릿 콘텐츠를 엽니다.

1. 왼쪽 레일에서 **[!UICONTROL 조각]** 아이콘을 선택합니다.

   ![](assets/fragments-in-designer.png)

1. 현재 샌드박스에서 만든 모든 시각적 조각 목록이 표시됩니다. 다음을 수행할 수 있습니다.

   * 레이블 입력을 시작하여 특정 조각을 검색합니다.
   * 오름차순 또는 내림차순으로 조각을 정렬합니다.
   * 조각이 표시되는 방법(카드 또는 목록 보기)을 변경합니다.

   >[!NOTE]
   >
   >조각은 생성 날짜별로 정렬됩니다. 최근에 추가된 조각이 목록에 먼저 표시됩니다.

   콘텐츠를 편집하는 동안 일부 시각적 조각이 수정되거나 추가된 경우 **새로 고침** 아이콘을 클릭하여 최신 변경 내용으로 목록을 업데이트합니다.

1. 목록의 시각적 조각을 삽입하려는 영역으로 끌어서 놓습니다. 다른 구성 요소와 마찬가지로 콘텐츠에서 조각을 이동할 수 있습니다.

1. 조각을 선택하여 오른쪽 창에 옵션을 표시합니다.

   ![](assets/fragment-right-pane.png)

   **[!UICONTROL 설정]** 탭에서 다음을 수행할 수 있습니다.

   * 조각을 표시할 장치를 선택합니다.
   * **콘텐츠 편집** 단추를 클릭하여 이 조각의 콘텐츠를 엽니다. [자세히 알아보기](../content/fragments.md#edit-fragments)

     **[!UICONTROL 스타일]** 탭을 사용하여 조각을 추가로 사용자 지정할 수 있습니다.

1. 필요한 경우 원본 시각적 조각으로 상속을 중단할 수 있습니다. [자세히 알아보기](#break-inheritance)

   콘텐츠에서 조각을 삭제하거나 복제할 수도 있습니다. 이러한 작업은 조각 위에 표시되는 상황별 메뉴에서 직접 수행할 수 있습니다.

1. 원하는 만큼 시각적 조각을 추가하고 변경 내용을 **[!UICONTROL 저장]**&#x200B;합니다.

### 읽기 전용 모드의 시각적 조각 {#fragment-readonly}

액세스 권한은 시각적 조각에 적용될 수 있습니다.

특정 시각적 조각에 대한 편집 권한이 없는 경우 콘텐츠 템플릿이 **읽기 전용 모드**&#x200B;로 표시됩니다. 이 경우 **[!UICONTROL 콘텐츠 편집]** 단추가 **[!UICONTROL 콘텐츠 보기]** 단추로 바뀌므로 변경하지 않고 조각을 볼 수 있습니다.

![](assets/fragment-readonly.png){zoomable="yes"}

아래 표시된 대로 모든 기능 아이콘이 비활성화되어 상호 작용이 보기 전용으로 제한됩니다.

![](assets/fragment-readonly-view.png){zoomable="yes"}

## 상속 중단 {#break-inheritance}

시각적 조각을 편집하면 변경 사항이 동기화됩니다. 모든 이메일 게재 및 해당 조각을 포함하는 콘텐츠 템플릿에 자동으로 전파됩니다.

이메일 또는 콘텐츠 템플릿에 추가되면 조각은 기본적으로 동기화됩니다.

그러나 원본 조각에서 상속을 중단할 수 있습니다. 이 경우 조각의 콘텐츠가 현재 디자인에 복사되며, 변경 사항은 더 이상 동기화되지 않습니다.

상속을 중단하려면 아래 단계를 수행합니다.

1. 시각적 조각을 선택합니다.

1. 상황별 툴바에서 잠금 해제 아이콘을 클릭합니다.

   ![](assets/fragment-break-inheritance.png)

1. 해당 조각은 원래 조각에 더 이상 연결되지 않는 독립 실행형 요소가 됩니다. 콘텐츠의 다른 콘텐츠 구성 요소로 편집합니다. [자세히 알아보기](../email/content-components.md)
