---
title: Campaign 웹 사용자 인터페이스의 보호 및 제한 사항
description: Campaign 웹 사용자 인터페이스의 보호 및 제한 사항
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 65%

---

# 보호 기능 및 제한 사항 {#guardrails-limitations}

Campaign 클라이언트 콘솔에서 만들거나 수정한 구성 요소로 Campaign 웹 사용자 인터페이스에서 작업하는 경우 아래 나열된 보호 기능 및 제한 사항이 적용됩니다.

## 워크플로 {#wf-guardrails-limitations}

### 활동

Campaign 웹 사용자 인터페이스에서 아직 지원되지 않는 워크플로우 활동은 읽기 전용이며 호환되지 않는 활동으로 표시됩니다. 워크플로를 실행하고, 메시지를 전송하고, 로그를 확인하는 등의 작업은 수행할 수 있습니다. Campaign 웹 사용자 인터페이스와 Campaign 클라이언트 콘솔 모두에서 사용할 수 있는 워크플로우 활동을 편집할 수 있습니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

웹 사용자 인터페이스에서 아직 지원되지 않는 워크플로우 활동 설정은 표시되지 않습니다. 그러나 워크플로가 실행되면 이러한 설정이 적용됩니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

콘솔에서 **보강** 활동을 통해 조정 및 보강을 모두 수행할 수 있습니다. Campaign 웹 사용자 인터페이스에서 조정 기능을 아직 사용할 수 없습니다. 클라이언트 콘솔에서 을 정의한 경우 **데이터 보강** 활동은 Campaign 웹 사용자 인터페이스에 호환되지 않는 읽기 전용 활동으로 표시됩니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### 캔버스

Campaign 웹 사용자 인터페이스에서 새 워크플로우를 만들 때 캔버스는 하나의 진입점만 지원합니다. 하지만 콘솔에 여러 진입점이 있는 워크플로를 만든 경우에는 Campaign 웹 사용자 인터페이스에서 워크플로를 열고 편집할 수 있습니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

루프는 아직 Campaign 웹 사용자 인터페이스에서 사용할 수 없습니다. 콘솔을 사용하여 루프를 포함하는 워크플로를 만든 경우 Campaign 웹 사용자 인터페이스에서 액세스할 수 없습니다. 오류 메시지가 표시됩니다.

| 콘솔 | 웹 |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

활동이 추가되거나 제거될 때마다 노드 위치가 새로 고쳐집니다. 콘솔에서 워크플로우를 만들고 Campaign 웹 사용자 인터페이스를 사용하여 수정한 후 콘솔에서 다시 열면 몇 가지 사소한 위치 지정 불완결성을 볼 수 있습니다. 이는 워크플로의 프로세스 및 작업에 영향을 주지 않습니다.

| 초기 워크플로 | 위치 변경 |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## 미리 정의된 필터 {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="이 필터는 읽기 전용입니다."
>abstract="일부 미리 정의된 필터는 해당 제품 버전의 사용자 인터페이스에서 사용할 수 없습니다. 이러한 필터는 읽기 전용으로 표시됩니다. 쿼리 모델러에서 쿼리의 그래픽 표현을 볼 수 없고 필터를 편집할 수 없는 경우에도 필터를 사용할 수 있으며 화면의 **속성** 섹션에서 필터링 조건을 볼 수 있습니다."

해당 버전의 제품에서는 게재 대상을 선택하거나 워크플로에서 대상자를 구성할 때 일부 미리 정의된 필터를 사용자 인터페이스에서 사용할 수 없습니다. 이러한 필터는 읽기 전용으로 표시됩니다.

특정 오류 메시지가 표시됩니다.

![](assets/filter-unavailable.png){width="70%" align="left"}

쿼리 모델러에서 쿼리의 그래픽 표현을 볼 수 없고 필터를 편집할 수 없는 경우에도 필터를 사용할 수 있으며 화면의 **속성** 섹션에서 필터링 조건을 볼 수 있습니다.

![](assets/rule-edit.png){width="70%" align="left"}

SQL 쿼리에 액세스하여 정확한 설정을 확인할 수도 있습니다. 이렇게 하려면 **코드 보기** 버튼을 클릭하십시오.

![](assets/rule-code-view.png){width="70%" align="left"}

**계산** 버튼을 클릭하면 필터 기준에 맞는 항목 수를 확인할 수 있습니다.

![](assets/rule-calculate.png){width="70%" align="left"}

해당 항목을 표시하려면 **결과 보기** 버튼을 사용하십시오.

![](assets/rule-view-results.png){width="70%" align="left"}

웹 인터페이스에서 필터를 빌드하고 지원되지 않는 속성을 사용하여 콘솔에서 이를 수정하면 웹 인터페이스에서 그래픽 표현을 더 이상 사용할 수 없습니다. 어떤 경우에도 필터를 계속 사용할 수 있습니다.

지원되지 않는 속성은 다음과 같습니다.

### 지원되지 않는 데이터 유형 {#unsupported-data-type}

클라이언트 콘솔에서 사용할 수 있는 다음 데이터 유형은 웹 인터페이스에 필터나 규칙을 표시할 때 지원되지 않습니다.

* datetime
* 시간
* timespan
* 중복
* 부동

### 지원되지 않는 필터링 기능 {#unsupported-filtering-capabilities}

클라이언트 콘솔에서 복잡한 표현식과 함수로 필터를 작성한 경우 웹 인터페이스에서 편집할 수 없습니다.

또한 다음 연산자는 지원되지 않습니다.

* 숫자 유형
   * 다음에 포함됨
   * 다음에 없음

* 문자열 유형
   * 다음보다 큼
   * 다음보다 작음:
   * 다음보다 크거나 같음
   * 다음보다 작거나 같음
   * 비슷함
   * 비슷하지 않음

* 날짜 유형
   * 다음 또는 이후
   * 다음 또는 이전
   * 다음과 같지 않음
   * 비어 있음
   * 비어 있지 않음
   * 다음에 포함됨
   * 다음에 없음
   * 마지막

* 1-N 링크
   * 개수, 합계, 평균, 최소, 최대
