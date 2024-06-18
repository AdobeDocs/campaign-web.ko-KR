---
audience: end-user
title: 게재 경고
description: 게재 경고 작업 방법을 알아봅니다.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 2%

---

# 게재 경고 기준 {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="게재 경고 기준 대시보드"
>abstract="Campaign 웹 사용자 인터페이스는 대시보드에 추가할 수 있는 미리 정의된 경고 기준(낮은 처리량을 가진 게재, 준비에 실패한 게재...)을 제공합니다. 필요에 따라 고유한 기준을 만들 수도 있습니다."

Campaign 웹 사용자 인터페이스는 대시보드에 추가할 수 있는 미리 정의된 경고 기준(낮은 처리량을 가진 게재, 준비에 실패한 게재...)을 제공합니다. 필요에 따라 고유한 기준을 만들 수도 있습니다.

경고 기준은 **게재 경고** 왼쪽 탐색 창의 메뉴 아래에서 **기준** 탭.

![](assets/alerting-criteria-list.png)

## 사전 정의된 경고 기준 {#ootb-criteria}

Campaign 웹 사용자 인터페이스에서 사전 정의된 경고 기준을 사용할 수 있습니다. 이러한 기준은 아래와 같은 다양한 시나리오를 다룹니다.

* **게재 실패**: 정의된 범위 내에서 예약된 잘못된 상태의 모든 게재.
* **준비 중인 게재 실패**: 정의된 범위 내에서 수정된 모든 게재로서, 준비 단계(대상 계산 및 콘텐츠 생성)에 실패했습니다.
* **소프트 바운스에 대한 잘못된 오류 비율이 있는 게재**: 정의된 범위 내에서 정의된 비율보다 큰 소프트 바운스 오류 비율과 함께 진행 중 이상의 상태로 예약된 모든 게재.
* **하드 바운스에 대한 오류 비율이 잘못된 게재**: 정의된 범위 내에서 정의된 비율보다 큰 하드 바운스 오류 비율과 함께 진행 중 이상의 상태로 예약된 모든 게재.
* **긴 시작 보류 중인 게재**: 정의된 범위 내에서 시작 보류 상태가 정의된 기간보다 긴 예약된 게재. 시작 보류 상태는 메시지가 아직 시스템에서 고려되지 않았음을 의미합니다.
* **낮은 처리량의 게재**: 정의된 기간 이상 동안(처리된 메시지의 정의된 비율 미만) 정의된 값보다 낮은 처리량으로 시작된 게재.
* **게재 진행 중**: 정의된 범위 내에서 진행 중 상태로 예약된 모든 게재.

>[!NOTE]
>
>위의 기준에 대한 모든 매개 변수에 기본값이 적용됩니다. 이러한 값은 다음에서 사용자 지정할 수 있습니다 **기준 매개 변수** 게재 경고 대시보드의 섹션. 여기서 사용 중입니다. [대시보드 작업 방법 알아보기](../msg/delivery-alerting-dashboards.md)

## 경고 기준 만들기 {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="게재 경고 기준 만들기"
>abstract="Adobe Campaign에서 제공하는 사전 정의된 경고 기준 외에도 필요에 따라 고유한 기준을 만들 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="경고에 추가할 표시기"
>abstract="전자 메일 경고의 &quot;세부 정보&quot; 섹션에 열로 표시할 지표를 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="경고 유형"
>abstract="다음을 지정합니다. **경고 유형** (기준의 경우) 경고의 &quot;요약&quot; 섹션에서 게재 기준 옆에 표시할 레이블과 색상을 의미합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="기준 빈도"
>abstract="기준을 충족하는 각 게재에 대해 일별 경고 빈도를 제어합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="경고 기준 만들기"
>abstract="고유한 게재 필터를 만들려면 Campaign v8 콘솔에서 사전 정의된 새 필터를 만듭니다. **관리** > **구성** > **사전 정의된 필터** 노드."

새 기준을 만들려면 다음 단계를 수행하십시오.

1. 다음 위치로 이동 **게재 아예르팅** 왼쪽 탐색 창에서 메뉴를 선택하고 **기준** 탭.
1. 다음을 클릭합니다. **게재 경고 기준 만들기** 단추를 클릭합니다.
1. 기준에 대한 레이블을 제공합니다. 내부 이름은 자동으로 채워지고 읽기 전용입니다.
1. 다음 **이 기준에 의해 적용된 게재 필터** 을 사용하면 사전 정의된 필터를 적용하여 기준의 범위를 세분화할 수 있습니다.

   아래 예에서는 **진행 중인 게재(critInProgressDeliveries)** 필터가 선택되었습니다. 즉, 기준은 &quot;진행 중&quot; 상태의 게재만 고려합니다.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >사전 정의된 필터 중 사용자의 요구에 맞는 필터가 없는 경우 관리자에게 연락하여 고유한 필터를 만들 수 있습니다.  Campaign 콘솔에서 사전 정의된 필터를 만드는 방법에 대한 자세한 내용은 [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >이 작업은 고급 사용자만 수행해야 합니다.

1. 다음에서 **경고에 추가할 지표** 섹션에서 전자 메일 경고의 &quot;세부 정보&quot; 섹션에 열로 표시할 지표를 선택합니다.

1. 다음을 지정합니다. **경고 유형** (기준의 경우) 경고의 &quot;요약&quot; 섹션에서 게재 기준 옆에 표시할 레이블과 색상을 의미합니다.

1. 다음 **기준 빈도** 섹션에서 기준을 충족하는 각 게재에 대해 매일 경고 빈도를 제어할 수 있습니다.

   * **이 게재 기준은 모든 알림에서 반복됩니다.**: 그날의 모든 이메일 알림에서 기준을 충족하는 게재를 표시합니다.
   * **이 게재 기준은 당일의 첫 번째 발생 시에만 전송됩니다**: 그 날의 첫 번째 보고서에서만 기준을 충족하는 게재를 표시하고 후속 이메일 경고에서는 반복하지 않습니다.
