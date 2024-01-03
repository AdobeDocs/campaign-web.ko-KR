---
audience: end-user
title: 푸시 채널에 대한 글로벌 보고서
description: 푸시 채널에 대한 글로벌 보고서 이해
badge: label="제한 공개"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 4%

---

# 푸시 채널에 대한 글로벌 보고서 {#campaign-reports-push}

글로벌 보고서는 채널 수준의 트래픽 및 참여 지표에 대한 포괄적인 개요를 사용자에게 제공합니다.

다음 위치로 이동 **[!UICONTROL 보고서]** 내 메뉴 **[!UICONTROL 보고]** 섹션. 보고서 날짜, 폴더 또는 규칙에 따라 데이터를 필터링할 수 있습니다. [자세히 알아보기](global-reports.md)

## 게재 요약 {#delivery-summary-push}

### 게재 요약 {#delivery-overview-push}

다음 **[!UICONTROL 게재 개요]** 보고서는 방문자가 모든 푸시 알림 전달을 수행하는 방법에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_push_delivery_overview.png)

+++게재 개요 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 전달됨]**: 성공적으로 전송된 메시지 수와 총 전송된 메시지 수

* **[!UICONTROL 총 클릭수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 오류]**: 총 보낸 메시지 수와 관련하여 게재 및 자동 반환 처리 중에 누적된 총 오류.

+++

### 타겟팅된 대상자 {#delivery-summary-push-initial-target}

다음 **[!UICONTROL 타깃팅된 대상]** 테이블 및 그래프는 전송된 각 푸시 알림 게재에 대해 수신자와 관련된 데이터를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_push_targeted_audience.png)

+++타깃팅된 대상 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 타깃팅된 대상]**: 타겟팅된 총 수신자 수.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 제외]**&#x200B;차단 목록에 추가하다 : 분석 중에 무시된 총 주소 수: 격리된 주소, 격리된 주소 수 등 규칙 적용 시

+++

### 게재 통계 {#delivery-summary-push-exec-stats}

다음 **[!UICONTROL 게재 통계]** 표에서 모든 푸시 알림 전달의 성공 여부를 확인할 수 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_push_delivery_statistics.png)

+++게재 통계 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 총 메시지 수]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류 / 바운스]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새로운 격리]**: 게재 실패 후 격리된 총 주소 수(예: 잘못된 등록, 메시지 거부, 페이로드 오류) 게재할 메시지 수 관련.

  푸시 알림 오류 유형은 [Adobe Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### 제외 이유 {#causes-exclusion}

다음 **[!UICONTROL 제외 이유]** 그래프 및 표에는 타겟팅된 프로필에서 제외된 사용자 프로필에서 메시지를 받을 수 없는 이유가 표시됩니다.

푸시 알림 오류 유형은 [Adobe Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## 게재 처리량 {#delivery-throughput-sms}

![](assets/global_report_push_delivery_statistics.png)

이 보고서는 지정된 기간 내의 게재 처리량에 대한 포괄적인 세부 정보를 제공합니다.

