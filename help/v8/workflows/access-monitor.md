---
audience: end-user
title: Adobe Campaign Web을 사용하여 워크플로 만들기
description: Adobe Campaign Web을 사용하여 워크플로를 빌드하는 방법 알아보기
badge: label="Alpha"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 23%

---

# 워크플로 액세스 및 관리 {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="워크플로"
>abstract="이 화면에서 독립 실행형 워크플로 및 캠페인 워크플로의 전체 목록에 액세스하고 현재 상태, 마지막/다음 실행 일자를 확인하고 새 워크플로를 만들 수 있습니다. 사용 가능한 워크플로 템플릿에 액세스하려면 “템플릿” 탭으로 이동합니다."

다음 **[!UICONTROL 워크플로]** 메뉴를 사용하면 전체 워크플로 목록에 액세스할 수 있습니다. 이 목록에는 두 항목이 모두 포함됩니다. **독립 실행형 워크플로** 이 화면에서 만들어짐 **캠페인 워크플로우**: 캠페인 내에서 생성됩니다.

![](assets/workflow-list.png)

목록의 각 워크플로에는 현재 워크플로에 대한 정보가 표시됩니다 [상태](#status)마지막으로 실행되거나 수정된 시간과 다음에 예약된 실행 날짜 및 시간입니다.

다음을 클릭하여 표시된 열을 사용자 지정할 수 있습니다. **[!UICONTROL 사용자 지정 레이아웃에 대한 열 구성]** 아이콘은 목록의 오른쪽 위 모서리에 있습니다. 이를 통해 각 워크플로우에 대해 오류가 발생한 마지막 활동이나 적용된 타겟팅 차원과 같은 추가 정보를 목록에 추가할 수 있습니다.

또한 목록에서 쉽게 검색할 수 있도록 검색 창과 필터를 사용할 수 있습니다. 예를 들어 캠페인에 속하는 워크플로우나 특정 날짜 범위 동안 처리된 워크플로우만 표시하도록 워크플로우를 필터링할 수 있습니다.

워크플로우를 복제하거나 삭제하려면 줄임표 버튼을 클릭한 다음 을 선택합니다 **[!UICONTROL 복제]** 또는 **[!UICONTROL 삭제]**.

>[!NOTE]
>
>진행 중인 워크플로를 복제할 수는 있지만 삭제할 수는 없습니다.

## 워크플로 상태 {#status}

워크플로의 상태는 여러 가지가 될 수 있습니다.

* **[!UICONTROL 초안]**: 워크플로우가 만들어지고 저장되었습니다.
* **[!UICONTROL 진행 중]**: 워크플로우가 현재 실행 중입니다.
* **[!UICONTROL 완료됨]**: 워크플로우 실행이 완료되었습니다.
* **[!UICONTROL 일시 중지됨]**: 워크플로우가 일시 중지되었습니다.
* **[!UICONTROL 잘못됨]**: 워크플로우에서 오류가 발생했습니다. 워크플로우를 열고 로그 및 작업에 액세스하여 오류를 식별하고 해결합니다. [로그 및 작업을 모니터링하는 방법 알아보기](start-monitor-workflows.md#logs-tasks)

워크플로우 실행을 시작하고 모니터링하는 방법에 대한 자세한 내용은에서 확인할 수 있습니다. [이 페이지](start-monitor-workflows.md).

## 워크플로 템플릿 {#templates}

다음 **[!UICONTROL 템플릿]** 탭에는 사용 가능한 모든 워크플로우 템플릿이 나열됩니다.

워크플로 템플릿에는 새 워크플로를 만드는 데 재사용할 수 있는 사전 구성된 활동 및 전체 속성 구성이 포함됩니다. 클라이언트 콘솔에서 생성됩니다. [템플릿 작업 방법 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
