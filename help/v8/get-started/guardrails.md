---
title: Campaign Web 사용자 인터페이스 워크플로의 보호 기능 및 제한 사항
description: Campaign Web 사용자 인터페이스에서 워크플로 작업 시 보호 기능 및 제한 사항
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 100%

---

# 워크플로에 대한 보호 기능 및 제한 사항 {#guardrails-limitations}

Campaign 클라이언트 콘솔에서 생성되거나 수정된 워크플로를 사용하여 Campaign Web 사용자 인터페이스에서 작업할 때 아래에 나열된 보호 기능 및 제한 사항이 적용됩니다.

이 페이지에서는 콘솔과 웹 사용자 인터페이스의 워크플로 작업 시 주요 고려 사항을 파악하지만, 두 인터페이스 간의 잠재적인 비호환성을 모두 포괄하지는 않습니다.

## 워크플로 활동 {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="활동 편집 불가"
>abstract="**쿼리** 또는 **보강** 활동이 콘솔에서 추가 데이터로 구성된 경우, Campaign Web에서 보강 데이터가 고려되어 아웃바운드 전환으로 전달되지만, 편집할 수는 없습니다."

Campaign Web 사용자 인터페이스에서 아직 지원되지 않는 워크플로 활동은 읽기 전용이며 호환되지 않는 활동으로 표시됩니다. 워크플로를 실행하고, 메시지를 전송하며, 로그를 확인하는 등의 작업은 계속 수행할 수 있습니다. Campaign Web 사용자 인터페이스와 클라이언트 콘솔 모두에서 사용할 수 있는 워크플로 활동은 편집할 수 있습니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

**쿼리** 또는 **보강** 활동이 콘솔에서 추가 데이터로 구성된 경우, Campaign Web에서 보강 데이터가 고려되어 아웃바운드 전환으로 전달되지만, 편집할 수는 없습니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

콘솔에서 **보강** 활동을 통해 조정 및 보강을 모두 수행할 수 있습니다. 클라이언트 콘솔의 **보강** 활동에서 조정 설정을 정의한 경우 Campaign Web 사용자 인터페이스에서 **조정** 활동으로 표시됩니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## 워크플로 캔버스 {#wkf-canvas}

Campaign Web 사용자 인터페이스에서 새 워크플로를 생성할 때 캔버스는 하나의 진입점만 지원합니다. 그러나 콘솔에서 여러 진입점이 있는 워크플로우를 생성한 경우 Campaign Web 사용자 인터페이스에서 열고 편집할 수 있습니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

활동이 추가되거나 제거될 때마다 노드 위치가 새로 고쳐집니다. 콘솔에서 워크플로를 생성하고 Campaign Web 사용자 인터페이스를 사용하여 수정한 후 콘솔에서 다시 열면 약간의 위치 결함이 발견될 수 있습니다. 이는 워크플로의 프로세스 및 작업에 영향을 주지 않습니다.

| 초기 워크플로 | 위치 변경 |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |
