---
product: campaign
title: 게재 액세스
description: Campaign 웹에서 게재에 액세스하고 관리하는 방법을 알아봅니다
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: ecff4e56bd346aadf381a1bf2077204804938f62
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 68%

---

# 게재 액세스 {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="게재"
>abstract="게재는 이메일, SMS 또는 푸시와 같은 특정 채널을 통해 대상자에게 전송되는 커뮤니케이션입니다. 이 화면에서는 기존 게재를 편집, 복제, 삭제할 수 있습니다. 또한 완료된 게재에 대한 보고서를 볼 수 있습니다. **게재 만들기** 버튼을 클릭하여 새 게재를 추가합니다."

## 게재 액세스 {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="추가 대상"
>abstract="이러한 규칙은 클라이언트 콘솔에서만 변경할 수 있습니다."

게재는 왼쪽 탐색 메뉴의 **[!UICONTROL 게재]** 메뉴에서 액세스할 수 있습니다. 클라이언트 콘솔 또는 웹 사용자 인터페이스에서 만든 모든 게재가 이 목록에 표시됩니다. 이 화면에서 모든 기존 게재를 모니터링하거나, 복제 또는 삭제하거나, 새 게재를 만들 수 있습니다.

![](assets/deliveries-list.png)

게재를 열려면 목록에서 해당 이름을 클릭합니다. 게재가 열리면 전용 보고서를 사용하여 매개 변수 편집, 실행 확인 또는 성능 모니터링과 같은 다양한 작업을 수행할 수 있습니다.

![](assets/delivery-details.png)

>[!NOTE]
>
>클라이언트 콘솔에서 만든 게재를 여는 경우 대상자에 대해 **[!UICONTROL 추가 대상]** 섹션이 표시될 수 있습니다. 즉, 이 게재에 대해 여러 타겟이 구성되었습니다. 이러한 매개 변수는 콘솔에서만 수정할 수 있습니다.
>
>![](assets/target-warning-audience.png){zoomable="yes"}

## 게재 복제 {#delivery-duplicate}

게재 목록 또는 게재 대시보드에서 기존 게재의 사본을 만들 수 있습니다.

게재 목록에서 게재를 복제하려면 다음 단계를 수행합니다.

1. 게재 이름 옆 오른쪽에서 세 점 버튼을 클릭하여 복제합니다.
1. **[!UICONTROL 복제]**&#x200B;를 선택합니다.
1. 중복 확인: 새 게재 대시보드가 중앙 화면에서 열립니다.

대시보드에서 게재를 복제하려면 다음 단계를 수행합니다.

1. 게재를 열고 화면 상단의 **[!UICONTROL 자세히...]** 버튼을 클릭합니다.
1. **[!UICONTROL 복제]**&#x200B;를 선택합니다.
1. 중복 확인: 중앙 화면에서 새 게재는 현재 게재를 대체합니다.

## 게재 삭제 {#delivery-delete}

게재 목록(왼쪽 레일의 메인 게재 항목 또는 캠페인의 게재 목록 중 하나)에서 게재가 삭제됩니다.

게재 목록에서 게재를 삭제하려면 다음 단계를 수행합니다.

1. 게재 이름 옆 오른쪽에서 세 점 버튼을 클릭하여 복제합니다.
1. **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
1. 삭제를 확인합니다.

![게재 목록에서 게재 삭제](assets/delete-delivery-from-list.png)

모든 게재는 이 목록에서 사용할 수 있지만, 워크플로에서 생성된 게재는 여기에서 삭제할 수 없습니다. 워크플로 컨텍스트에서 생성된 게재를 삭제하려면 워크플로에서 게재 활동을 삭제해야 합니다.

워크플로에서 게재를 삭제하려면 다음 단계를 수행합니다.

1. 게재 활동을 선택합니다.
1. 오른쪽 패널의 **[!UICONTROL 삭제]** 아이콘을 클릭합니다.
1. 삭제를 확인합니다. 게재에 하위 노드가 있는 경우 하위 노드를 삭제하거나 유지하도록 선택할 수도 있습니다.

![워크플로에서 게재 삭제](assets/delete-delivery-from-wf.png)
