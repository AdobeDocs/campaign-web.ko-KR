---
audience: end-user
title: 읽기 전용 워크플로 정보
description: 워크플로우가 읽기 전용 모드인 이유를 알아봅니다.
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 13%

---

# 읽기 전용 워크플로 정보 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="이 워크플로는 읽기 전용입니다."
>abstract="귀하의 권리 또는 워크플로 유형으로 인해 이 워크플로를 편집할 수 없습니다."

일부 워크플로우는 읽기 전용입니다. 기본 제공 기술 워크플로우는 항상 읽기 전용이지만 다른 유형의 워크플로에서도 이 재구성을 활성화할 수 있습니다.

Campaign 사용자는 Adobe Campaign 데이터에 대한 액세스가 제한될 수 있습니다. Campaign 관리자는 사용자에게 일부 기능을 볼 수 있는 권한을 부여할 수 있지만 편집하거나 수정할 수는 없습니다. 데이터에 대한 사용자 권한은 데이터 및 프로세스 보안을 보장하기 위한 핵심 권한입니다. [이 섹션](../get-started/permissions.md)에서 Campaign의 권한 관리에 대해 자세히 알아보세요.

워크플로우가 읽기 전용 모드에 있는 경우:

* **[!UICONTROL 설정]** 단추 근처의 **[!UICONTROL 읽기 전용]** 언급
* 작업 버튼에 액세스할 수 없음

![](assets/readonly-workflow.png){zoomable="yes"}

읽기 전용 워크플로우에서는 어떤 것도 편집할 수 없습니다. 활동의 설정을 변경할 수 없습니다.

![](assets/scheduler-readonly.png){zoomable="yes"}

사용자는 워크플로우를 삭제할 수 없습니다.

![](assets/readonly-rights.png){zoomable="yes"}


## 읽기 전용 워크플로 유형 {#readonly-workflow-types}

워크플로우의 유형에 따라 읽기 전용 모드가 다를 수 있습니다.

### 캠페인 워크플로 {#readonly-campaign-wf}

읽기 전용 캠페인 워크플로우의 경우 사용자가 모니터링 버튼에 액세스할 수 없습니다.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 기술 워크플로 {#readonly-tech-wf}

기본 제공 기술 워크플로우는 관리자도 모든 캠페인 사용자에 대해 읽기 전용입니다. 그러나 필요한 경우 사용자는 **일시 중지**&#x200B;하거나 **중지**&#x200B;할 수 있습니다. 이러한 작업만 허용됩니다.

![](assets/readonly-technical-workflow.png){zoomable="yes"}

[이 섹션](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)에서 기술 워크플로우에 대해 자세히 알아보세요.
