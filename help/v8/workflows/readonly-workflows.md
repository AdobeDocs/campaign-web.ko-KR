---
audience: end-user
title: 읽기 전용 워크플로 기본 정보
description: 워크플로우가 읽기 전용 모드인 이유를 알아봅니다.
source-git-commit: 6985e8cb11f12ab7818cc71441a4d3b41f1a0493
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# 읽기 전용 워크플로 기본 정보 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="이 워크플로는 읽기 전용입니다."
>abstract="권한 또는 워크플로 유형 때문에 이 워크플로를 편집할 수 없습니다."

일부 워크플로우는 읽기 전용 모드일 수 있습니다. 다음에서 볼 수 있습니다.

- 언급 **[!UICONTROL **&#x200B;읽기 전용&#x200B;**]**  근처 **[!UICONTROL 설정]** 단추
- 작업 버튼에 액세스할 수 없음

![](assets/readonly-workflow.png){zoomable="yes"}

읽기 전용 워크플로우에서는 아무것도 편집할 수 없습니다. 활동의 설정을 변경할 수 없습니다.


![](assets/scheduler-readonly.png){zoomable="yes"}


워크플로우를 삭제할 권한도 없습니다.

![](assets/readonly-rights.png){zoomable="yes"}

## 읽기 전용 워크플로우의 이유

읽기 전용 모드는 이러한 워크플로우를 편집할 수 있는 권한 및 액세스 권한이 없는 사용자를 위한 것입니다. [여기에서 자세히 알아보기](../get-started/permissions.md)

캠페인 사용자는 Adobe Campaign에서 액세스할 수 있는 데이터에 제한이 있을 수 있습니다. 관리자는 일부 기능을 볼 수 있지만 작업할 수는 없습니다.

## 읽기 전용 워크플로 유형

워크플로우의 유형에 따라 읽기 전용 모드가 다를 수 있습니다.

### 캠페인 워크플로

읽기 전용 캠페인 워크플로우의 경우 사용자가 모니터링 버튼에 액세스할 수 없습니다.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 기술 워크플로우

기술 워크플로우는 캠페인 사용자를 위해 읽기 전용 모드입니다.
기본 제공 기술 워크플로우는 관리자 사용자의 경우에도 모든 사용자를 위해 읽기 전용 모드입니다. 하지만 사용자는 **pause** 또는 **stop** 필요할 경우. 이러한 작업만 허용됩니다. [여기에서 자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}