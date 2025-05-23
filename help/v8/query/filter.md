---
audience: end-user
title: 필터 목록
description: 기본 제공 및 사용자 지정 필터를 사용하여 Adobe Campaign 웹 목록을 필터링하는 방법을 알아봅니다.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 485d8b4b715192cc5edb6442df0fa958e29d15ff
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 필터 목록 {#filter-lists}

Adobe Campaign 웹은 각 객체 목록 내에 필터를 제공하므로 특정 컨텍스트 기준에 따라 정보를 필터링할 수 있습니다. 예를 들어 상태, 채널, 연락 날짜 또는 폴더를 기반으로 게재를 필터링할 수 있습니다. 증명을 숨길 수도 있습니다.

>[!IMPORTANT]
>
>쿼리 모델러에 대한 완전히 새로운 인터페이스를 사용할 수 있습니다. 새 규칙 빌더를 사용하면 간소화된 인터페이스를 통해 쿼리를 더 쉽게 작성할 수 있습니다. 이 경험으로 전환하려면 오른쪽 상단 모서리에서 토글 버튼을 누릅니다. 언제든지 토글을 눌러 새 인터페이스를 비활성화하면 클래식 쿼리 모델러로 돌아갈 수 있습니다. 이 새 인터페이스에서 쿼리 모델러와 동일한 원칙을 적용할 수 있습니다.
>![새 규칙 빌더 인터페이스](assets/query-modeler-toggle.png){zoomable="yes"}에 대한 토글을 보여 주는 이미지

## 필터 적용 {#apply}

목록에 필터를 적용하려면 검색 창 옆에 있는 목록의 왼쪽 위 모서리에 있는 **[!UICONTROL 필터 표시]** 단추를 클릭합니다.

선택한 목록에 사용할 수 있는 필터를 표시하는 필터 창이 열립니다. 예를 들어 캠페인의 상태, 시작 및 종료 날짜 또는 저장소 폴더를 기준으로 캠페인을 필터링할 수 있으며 구독 서비스 목록은 캠페인의 채널 및 저장소 폴더를 기준으로 필터링될 수 있습니다.

![목록에 사용 가능한 필터를 표시하는 필터 창](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

자체 기준에 따라 목록을 필터링하려면 사용자 지정 필터를 만듭니다. 이렇게 하려면 필터 창의 맨 아래로 이동하여 **규칙 추가** 단추를 클릭하십시오. [사용자 지정 필터를 만드는 방법을 알아봅니다](#custom).

목록에 적용되면 검색 창 아래에 필터가 표시됩니다. 언제든지 개별 필터를 제거하거나 **모두 지우기** 단추를 클릭하여 모든 필터를 제거할 수 있습니다.

## 맞춤형 필터 만들기 {#custom}

맞춤형 필터를 사용하면 고유한 특정 기준에 따라 목록을 세분화할 수 있습니다. Campaign 쿼리 모델러를 사용하여 디자인되었습니다. 사용자 지정 필터를 만들려면 다음 단계를 수행합니다.

1. 필터 창을 열고 창 아래쪽에 있는 **규칙 추가** 단추를 클릭합니다.

1. 쿼리 모델러가 열립니다. 필요에 맞게 필터 기준을 정의하고 결합합니다. 쿼리 모델러를 사용하는 방법에 대한 자세한 정보는 [이 섹션](../query/query-modeler-overview.md)에서 확인할 수 있습니다.

   아래 예제는 실행 또는 요가 부서의 운영자가 실행하는 SMS 캠페인을 캠페인 목록에 표시하도록 디자인된 사용자 지정 필터를 보여줍니다.

   ![부서별로 필터링된 SMS 캠페인을 표시하는 사용자 지정 필터 예](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. 사용자 지정 필터가 구성되면 **[!UICONTROL 확인]**&#x200B;을 클릭하여 목록에 적용합니다.