---
audience: end-user
title: DM 채널에 대한 캠페인 보고서
description: DM 채널에 대한 캠페인 보고서 이해
exl-id: 7817d4c5-1f97-4b17-8a5f-f1a5b8701fe9
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 19%

---

# DM 채널에 대한 캠페인 보고서 {#campaign-reports-direct-mail}

각 캠페인 보고서는 캠페인의 성공 및 오류를 자세히 설명하는 다양한 위젯으로 나뉩니다. DM 채널의 경우 보고서 및 지표가 아래에 자세히 설명되어 있습니다. [이 페이지](campaign-reports.md)에서 캠페인 보고서에 액세스하는 방법을 알아보세요.

## 게재 요약 {#delivery-summary-direct}

### 게재 개요 {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_delivery_overview_direct_mail"
>title="게재 개요"
>abstract="**게재 개요**&#x200B;는 각 다이렉트 메일 게재와 방문자의 상호 작용에 대한 심층적인 인사이트를 제공하는 핵심 성과 지표(KPI)를 제시합니다. 지표는 아래에 설명되어 있습니다."

**[!UICONTROL 게재 개요]**&#x200B;에는 주요 성과 지표(KPI)가 표시되어 각 DM 게재와 방문자의 상호 작용에 대한 심도 있는 통찰력을 제공합니다. 지표는 아래에 설명되어 있습니다.

![DM 캠페인 게재 지표 개요](assets/direct-mail-campaign-overview.png){zoomable="yes"}{align="center"}

+++게재 개요 지표에 대해 자세히 알아봅니다.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 배달됨]**: 보낸 총 메시지 수와 관련하여 성공적으로 보낸 메시지 수입니다.

* **[!UICONTROL 오류]**: 보낸 총 메시지 수와 관련하여 게재 및 자동 반환 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 총 클릭 수]**: 게재를 한 번 이상 클릭한 총 고유 수신자 수입니다.

+++

### 초기 타깃 대상자 통계 {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_target_audience_direct_mail"
>title="초기 타깃 대상자 통계"
>abstract="수신자 데이터 및 메시지 정보는 게재 준비 분석을 반영하여 **초기 타깃 대상자 통계** 테이블에 표시됩니다."

**[!UICONTROL 초기 대상 통계]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 게재를 준비하는 동안 계산되며 초기 대상자, 보낼 메시지 수 및 제외된 수신자 수를 표시합니다.

![DM 캠페인에 대한 초기 대상 통계](assets/direct-mail-campaign-target-audience.png){zoomable="yes"}

+++초기 타겟 대상 통계 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 초기 대상]**: 타깃팅된 총 받는 사람 수

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수입니다.

* **[!UICONTROL 규칙에 의해 거부됨]**: 누락된 주소, 격리된 주소 또는 차단 목록에 추가하다의 주소와 같이 규칙을 적용할 때 분석 중에 무시된 총 주소 수입니다.

+++

### 실행 통계 {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_execution_statistics_direct_mail"
>title="게재 통계"
>abstract="**실행 통계** 테이블에는 다이렉트 메일 게재의 성공과 발생한 오류가 자세히 설명되어 있습니다."

![DM 캠페인에 대한 실행 통계](assets/direct-mail-campaign-exec.png)

**[!UICONTROL 실행 통계]** 테이블은 모든 DM 게재의 성공 여부를 아래에 설명된 세부 지표와 함께 분류합니다.

+++게재 통계 지표에 대해 자세히 알아봅니다.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수입니다.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 배달할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새 격리]**: 배달할 메시지 수와 관련하여 배달 실패 후 격리된 총 주소 수(예: 사용자 알 수 없음, 잘못된 도메인)입니다.

+++

### 생성된 클릭스트림 {#click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_clicks_direct_mail"
>title="생성된 클릭스트림"
>abstract="**생성된 클릭스트림** 테이블에는 수신자가 게재된 내용과 상호 작용한 방식과 관련하여 사용 가능한 데이터가 표시됩니다."

![DM 캠페인에 대한 스트림 데이터 클릭](assets/direct-mail-campaign-clicks.png){zoomable="yes"}{align="center"}

**생성된 클릭 스트림** 테이블은 대상 프로필에서 제외된 사용자 프로필에서 메시지를 받지 못하게 하는 이유를 설명합니다.

+++생성된 클릭 스트림 지표에 대해 자세히 알아봅니다.

* **[!UICONTROL 고유 클릭 수]**: 게재를 한 번 이상 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 총 클릭 수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 받는 사람 수와 관련하여 게재를 클릭한 대상 받는 사람 수의 비율입니다.

+++