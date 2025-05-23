---
audience: end-user
title: 쿼리 모델러로 작업
description: Adobe Campaign 웹 쿼리 모델러를 사용하여 작업하는 방법을 알아봅니다.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 22%

---

# 쿼리 모델러로 작업 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="새로운 규칙 빌더"
>abstract="이제 개선된 사용자 인터페이스에서 복잡한 조건을 정의하는 데 도움이 되는 새로운 규칙 작성기를 사용할 수 있습니다. 필요에 따라 이전 규칙 빌더에서 새로운 규칙 빌더로 전환할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko" text="릴리스 정보 참조"

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="새 쿼리 모델러"
>abstract="Adobe Campaign Web에는 다양한 기준에 따라 특정 대상을 선택하기 위해 데이터베이스 필터링 프로세스를 단순화하는 쿼리 모델러가 있습니다. 여기에는 고급 표현식 및 연산자의 사용이 포함됩니다. 쿼리 모델러는 데이터를 필터링하기 위한 규칙을 정의해야 하는 모든 상황에서 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="쿼리 모델러"
>abstract="데이터베이스의 수신자 또는 기타 타기팅 차원에 대한 필터링 기준을 정의합니다. Adobe Experience Platform 대상자를 활용하여 타깃 대상자를 더욱 세분화하고 캠페인 효과를 극대화합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="대상 조정"
>abstract="이들 규칙은 클라이언트 콘솔에서만 변경할 수 있습니다."

Adobe Campaign 웹 사용자 인터페이스에는 다양한 기준을 기반으로 데이터베이스를 필터링하는 프로세스를 간소화하는 쿼리 모델러가 포함되어 있습니다. 클라이언트 콘솔에서 생성된 쿼리와 완벽하게 호환되므로 웹 사용자 인터페이스로 원활하게 전환할 수 있습니다.

또한 쿼리 모델러는 매우 복잡하고 긴 쿼리를 효율적으로 관리하여 향상된 유연성과 정밀도를 제공합니다. 또한 조건 내에 사전 정의된 필터를 지원하므로 사용자가 쿼리를 쉽게 세분화할 수 있는 동시에 포괄적인 대상 타기팅 및 세분화 전략에 고급 표현식 및 연산자를 활용할 수 있습니다.

## 쿼리 모델러에 액세스

쿼리 모델러는 데이터를 필터링하기 위한 규칙을 정의해야 하는 모든 상황에서 사용할 수 있습니다.

| 사용 | 예제 |
|  ---  |  ---  |
| **대상 정의**: 메시지 또는 워크플로에서 타겟팅할 모집단을 지정하고 필요에 맞는 새 대상을 쉽게 만들 수 있습니다. [대상자를 만드는 방법을 알아봅니다](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [대상 만들기 인터페이스에 액세스하는 방법을 보여 주는 이미지] |
| **워크플로 활동 사용자 지정**: **분할** 및 **조정**&#x200B;과 같은 워크플로 활동 내에 규칙을 적용하여 특정 요구 사항에 맞게 조정하십시오. [워크플로우 활동에 대해 자세히 알아보기](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [워크플로 사용자 지정 옵션에 액세스하는 방법을 보여 주는 이미지] |
| **미리 정의된 필터**: 데이터 목록을 사용하거나 게재 대상을 구성하는 등 다양한 필터링 작업 중에 바로 가기 역할을 하는 미리 정의된 필터를 만듭니다. [미리 정의된 필터로 작업하는 방법을 알아봅니다](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [미리 정의된 필터에 액세스하는 방법을 보여 주는 이미지] |
| **보고서 데이터 필터링**: 보고서에 표시된 데이터를 필터링할 규칙을 추가합니다. [보고서 작업 방법 알아보기](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [보고서에서 데이터를 필터링하는 방법을 보여 주는 이미지] |
| **목록 사용자 지정**: 사용자 지정 규칙을 만들어 수신자 또는 게재 목록과 같은 목록에 표시되는 데이터를 필터링합니다. [목록을 필터링하는 방법 알아보기](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [목록 필터를 사용자 지정하는 방법을 보여 주는 이미지] |
| **조건부 콘텐츠 빌드**: 다른 수신자에게 표시할 콘텐츠를 정의하는 조건을 만들어 개인화되고 관련 있는 메시징을 보장하여 이메일 콘텐츠를 동적으로 만듭니다. [조건부 콘텐츠를 만드는 방법을 알아봅니다](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [조건부 콘텐츠를 만드는 방법을 보여 주는 이미지] |

>[!NOTE]
>
>대상이나 사전 정의된 필터와 같이 규칙이 적용된 클라이언트 콘솔에서 만든 개체에 액세스할 때 **[!UICONTROL 대상 세분화]** 섹션이 표시될 수 있습니다. 즉, 규칙 대상을 세분화하기 위해 추가 매개 변수가 구성되었습니다. 이러한 매개 변수는 콘솔에서만 수정할 수 있습니다.
>
>![대상 세분화에 대한 경고를 표시하는 이미지](assets/target-warning.png){zoomable="yes"}

## 쿼리 모델러 인터페이스 {#interface}

쿼리 모델러는 쿼리를 작성하는 중앙 캔버스와 쿼리에 대한 정보를 제공하는 오른쪽 창을 제공합니다.

>[!IMPORTANT]
>
>쿼리 모델러에 대한 완전히 새로운 인터페이스를 사용할 수 있습니다. 새 규칙 빌더를 사용하면 간소화된 인터페이스를 통해 쿼리를 더 쉽게 작성할 수 있습니다. 이 경험으로 전환하려면 오른쪽 상단 모서리에서 토글 버튼을 누릅니다. 언제든지 토글을 눌러 새 인터페이스를 비활성화하면 클래식 쿼리 모델러로 돌아갈 수 있습니다. 이 새 인터페이스에서 쿼리 모델러와 동일한 원칙을 적용할 수 있습니다.
>![새 규칙 빌더 인터페이스](assets/query-modeler-toggle.png){zoomable="yes"}에 대한 토글을 보여 주는 이미지


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="새로운 규칙 빌더 경험"
>abstract="이 토글을 사용하여 기존 쿼리 모델러와 새로운 규칙 빌더 경험 사이를 전환할 수 있습니다. 새로운 규칙 빌더를 사용하면 간결하고 직관적인 인터페이스를 통해 쿼리를 더 쉽게 작성할 수 있습니다."

![쿼리 모델러 인터페이스를 표시하는 이미지](assets/query-interface.png){zoomable="yes"}

### 중앙 캔버스 {#canvas}

쿼리 모델러 중앙 캔버스는 쿼리를 빌드하기 위해 다른 구성 요소를 추가 및 결합하는 곳입니다. [쿼리를 작성하는 방법 알아보기](build-query.md)

>[!BEGINTABS]

>[!TAB 클래식 쿼리 모델러]

캔버스의 오른쪽 아래 모서리에 있는 도구 모음에서는 쿼리 구성 요소를 쉽게 조작하고 캔버스를 탐색할 수 있는 옵션을 제공합니다.

* **여러 선택 모드**: 여러 필터링 구성 요소를 선택하여 원하는 위치에 복사하여 붙여 넣으십시오.
* **회전**: 캔버스를 세로로 전환합니다.
* **화면에 맞춤**: 캔버스 확대/축소 수준을 화면에 맞춥니다.
* **축소** / **확대**: 캔버스를 축소하거나 확대합니다.
* **맵 표시**: 현재 위치를 표시하는 캔버스의 스냅숏을 엽니다.

>[!TAB 새 규칙 빌더 경험]

캔버스의 오른쪽 위 모서리에 있는 도구 모음에서는 쿼리 구성 요소를 쉽게 조작하고 캔버스를 탐색할 수 있는 옵션을 제공합니다.

* **선택 영역 위로 이동**: 구성 요소를 행 위로 이동합니다.
* **선택 영역 아래로 이동**: 구성 요소를 행 아래로 이동합니다.
* **그룹 선택**: 두 개의 구성 요소를 그룹에 넣으십시오.
* **선택 해제**: 단일 그룹의 구성 요소를 구분합니다.
* **모두 확장**: 모든 그룹을 확장합니다.
* **모두 축소**: 모든 그룹을 축소합니다.
* **모두 제거**: 모든 그룹 및 구성 요소를 제거합니다.

>[!ENDTABS]

### 규칙 속성 창 {#rule-properties}

오른쪽의 **[!UICONTROL 규칙 속성]** 창에서는 쿼리에 대한 정보를 제공합니다. 다양한 작업을 수행하여 쿼리를 확인하고 요구 사항에 맞는지 확인할 수 있습니다. 이 창은 대상자를 만들기 위한 쿼리를 작성할 때 표시됩니다. [쿼리를 확인하고 확인하는 방법을 알아보세요](build-query.md#check-and-validate-your-query)
