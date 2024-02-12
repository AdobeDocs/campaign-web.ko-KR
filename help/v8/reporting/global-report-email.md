---
audience: end-user
title: 이메일 채널에 대한 전역 보고서
description: 이메일 채널에 대한 글로벌 보고서에 대해 자세히 알아보기
exl-id: 37c575e5-fd18-4a35-a11a-922d5bda1bae
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 24%

---

# 이메일 채널에 대한 전역 보고서 {#global-report-direct}

글로벌 보고서는 채널 수준의 트래픽 및 참여 지표에 대한 포괄적인 개요를 사용자에게 제공합니다.

다음 위치로 이동 **[!UICONTROL 보고서]** 내 메뉴 **[!UICONTROL 보고]** 섹션. 보고서 날짜, 폴더 또는 규칙에 따라 데이터를 필터링할 수 있습니다. [자세히 알아보기](global-reports.md)

## 게재 요약 {#delivery-summary-email}

### 게재 개요 {#delivery-overview-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_deliveries_overview_email"
>title="게재 개요"
>abstract="**게재 개요**&#x200B;에는 귀하가 보내는 이메일 게재 및 캠페인과 대상자가 어떻게 상호 작용하는지에 대한 심층적인 인사이트를 제공하는 주요 성과 지표(KPI)가 표시됩니다."

다음 **[!UICONTROL 게재 개요]** 은 방문자와 각 이메일 게재의 상호 작용에 대한 심층적인 통찰력을 제공하는 주요 성능 지표(KPI)를 제공합니다. 지표는 아래에 요약되어 있습니다.

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++게재 개요 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 전달됨]**: 성공적으로 전송된 메시지 수와 총 전송된 메시지 수

* **[!UICONTROL 총 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 총 클릭수]**: 한 번 이상 게재를 클릭한 총 수신자 수

* **[!UICONTROL 바운스 수 및 오류]**: 총 보낸 메시지 수와 관련하여 게재 및 자동 반환 처리 중에 누적된 총 오류.

* **[!UICONTROL 구독 취소]**: 구독 취소를 클릭한 수신자 수입니다.
+++

### 타겟팅된 대상자 {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_email"
>title="초기 타깃 대상자 통계"
>abstract="**타겟팅된 대상자** 표와 그래프는 수신자 참여에 대한 인사이트를 제공하므로 캠페인 및 게재의 효과를 평가하는 데 도움이 됩니다."

에 대한 테이블 및 그래프 **[!UICONTROL 타깃팅된 대상]** 아래에 제공된 세부 지표를 사용하여 수신자와 관련된 데이터를 표시합니다.

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++타깃팅된 대상 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 타깃팅된 대상]**: 타겟팅된 총 수신자 수.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 제외]**&#x200B;차단 목록에 추가하다 : 분석 중에 무시된 총 주소 수: 격리된 주소, 격리된 주소 수 등 규칙 적용 시

+++

### 게재 통계 {#delivery-summary-email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_email_delivery_stats"
>title="게재 통계"
>abstract="**게재 통계** 그래프와 표는 성공적인 게재, 오류, 새로운 격리를 포함한 주요 지표를 간략하게 설명하여 게재 성과를 평가하기 위한 간결한 개요를 제공합니다."

다음 **[!UICONTROL 게재 통계]** 표에는 모든 이메일 게재의 성공 사례가 자세히 설명되어 있습니다.

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++게재 통계 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류 / 바운스]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새로운 격리]**: 배달할 메시지 수와 관련하여 배달 실패 후 격리된 총 주소 수(사용자 알 수 없음, 잘못된 도메인)입니다.

+++

### 제외 이유 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusion_email"
>title="제외 이유"
>abstract="**제외 이유** 그래프와 표는 게재 준비 중 메시지가 거부되는 구체적인 이유를 보여 주며, 규칙별로 자세한 분류를 제공합니다."

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

제외 그래프 및 표는 타겟팅된 프로필에서 제외된 사용자 프로필이 메시지를 받지 못하는 이유를 설명합니다.

이메일 오류 유형은 [Adobe Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## 게재 처리량 {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_email"
>title="게재 처리량"
>abstract="이 **게재 처리량**&#x200B;은 게재 처리량에 대한 포괄적인 인사이트를 제공하며, 지정된 일정 내의 성공 및 오류율을 강조하여 보여 줍니다."

![](assets/global_report_email_delivery_throughput.png){zoomable=&quot;yes&quot;}{align="center"}

게재 처리량 보고서는 게재 프로세스의 효율성에 대한 심층적인 통찰력을 제공하여 지정된 기간 내의 성공 및 오류율에 대한 자세한 개요를 제공합니다.

+++게재 처리량 지표에 대해 자세히 알아봅니다.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

+++

## 비게재 항목 {#non-deliverables-email}

### 유형별 오류 분류 {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_type_email"
>title="유형별 오류 분류"
>abstract="**유형별 오류 분류**&#x200B;를 자세히 설명하는 표와 그래프에는 알 수 없는 사용자, 사서함 가득 참, 잘못된 도메인 등을 포함하여 프로세스 중에 발생한 다양한 오류 유형에 대한 정보가 포함되어 있습니다."

![](assets/global_report_email_breakdown_type.png){zoomable=&quot;yes&quot;}{align="center"}

다음 **[!UICONTROL 유형별 오류 분류]** 표 및 그래프는 다양한 도메인에서 경험하는 잠재적 오류와 관련된 데이터를 나타내며, 아래에 특정 지표가 제공됩니다.

이 보고서에 표시된 오류는 격리 프로세스를 트리거합니다. 격리 관리에 대한 자세한 내용은 다음을 참조하십시오. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++유형별 오류 분류에 대해 자세히 알아보십시오.

* **[!UICONTROL 알 수 없는 사용자]**: 이메일 주소가 잘못되었음을 나타내기 위해 게재 중에 생성된 오류 유형.

* **[!UICONTROL 잘못된 도메인]**: 이메일 주소의 도메인이 잘못되었거나 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성되는 오류 유형입니다.

* **[!UICONTROL 사서함 가득 참]**: 5회 게재 시도 후 생성된 오류 유형은 수신자의 받은 편지함에 메시지가 너무 많음을 나타냅니다.

* **[!UICONTROL 계정 비활성화]**: 주소가 더 이상 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성된 오류 유형.

* **[!UICONTROL 거부됨]**: IAP(인터넷 액세스 공급자)에서 주소를 거부할 때 오류 유형 이 생성됩니다(예: 보안 규칙 적용 후).

* **[!UICONTROL 연결할 수 없음]**: 메시지 배포 문자열에서 발생하는 오류 유형: SMTP 릴레이 장애, 일시적으로 도메인에 연결할 수 없음 등

* **[!UICONTROL 연결되지 않음]**: 전송 시 수신자의 휴대폰이 꺼져 있거나 네트워크에서 연결이 끊겼음을 나타내는 오류 유형입니다.

+++

### 도메인별 오류 분류 {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_domain_email"
>title="도메인별 오류 분류"
>abstract="**도메인별 오류 분류**&#x200B;를 보여 주는 표와 그래프는 발생한 각 오류 유형에 해당하는 데이터를 특정 도메인별로 분류하여 나타냅니다."

![](assets/global_report_email_breakdown_domain.png){zoomable=&quot;yes&quot;}{align="center"}

다음 **[!UICONTROL 도메인별 오류 분류]** 표 및 그래프는 각 도메인 내의 잠재적 오류와 관련된 데이터를 보여 줍니다. 지표는 **[!UICONTROL 유형별 오류 분류]** 위에 자세히 설명된 표 및 그래프입니다.

## 지표 추적 {#tracking-indicators-email}

### 게재 통계 {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_global_delivery_statistics_summary_email"
>title="게재 통계"
>abstract="**게재 통계** 주요 성과 지표(KPI)는 게재 및 캠페인 성과에 대한 포괄적인 개요를 제공하여 성공적인 게재, 발생한 오류 및 사용자 참여에 대한 인사이트를 제시합니다."

다음 **[!UICONTROL 게재 통계]** 지표는 모든 이메일 게재와 관련된 데이터에 대한 자세한 정보를 제공하는 주요 성능 지표(KPI)를 제공합니다. 이러한 지표에 대한 자세한 내용은 아래에 나와 있습니다.

![](assets/global_report_email_delivery_statistics_tracking.png){zoomable=&quot;yes&quot;}{align="center"}

+++게재 통계 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 고유 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 총 열람 수]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 옵트아웃 링크 클릭]**: 구독 취소 링크의 클릭 수입니다.

* **[!UICONTROL 미러 링크 클릭]**: 미러 페이지 링크를 클릭한 횟수.

* **[!UICONTROL 발송 예측]**: 타겟팅된 수신자가 전달한 이메일 수 예상.
+++

### 열람 및 클릭스루 비율 {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_open_clickthrough_email"
>title="열람 및 클릭스루 비율"
>abstract="**열람 및 클릭스루 비율** 표는 빠르고 유용한 인사이트가 있는 개요를 위해 열람 비율 및 클릭스루 비율에 대한 데이터를 표시하여 게재에 대한 수신자의 참여도를 보여 줍니다."

다음 **[!UICONTROL 열람 및 클릭스루 비율]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_email_opens.png){zoomable=&quot;yes&quot;}{align="center"}

+++열기 및 클릭스루 비율 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 전송됨]**: 전송된 총 메시지 수입니다.

* **[!UICONTROL 컴플레인]**: 수신자가 원치 않는 것으로 보고한 이 도메인에 대한 메시지 수 및 백분율.

* **[!UICONTROL 고유 열람 수]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자의 수 및 백분율입니다.

* **[!UICONTROL 고유 클릭수]**: 동일한 게재를 한 번 이상 클릭한 고유한 타깃팅된 수신자의 수 및 백분율입니다.

* **[!UICONTROL 원시 재활동]**: 게재를 한 번 이상 클릭한 수신자 수와 게재를 한 번 이상 연 수신자 수의 비율입니다.
+++

## URL 및 클릭 스트림 {#url-email}

### URL 및 클릭스트림 KPI {#url-email-kpis}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_clickstreams_email"
>title="URL 및 클릭 스트림"
>abstract="**URL 및 클릭스트림** 보고서는 게재 중 가장 많이 클릭된 URL에 대한 자세한 인사이트를 제공하는 필수 주요 성과 지표(KPI)를 수록하고 있습니다."

다음 **[!UICONTROL URL 및 클릭 스트림]** 보고서는 게재 중 가장 많은 클릭 수를 받은 URL에 대한 자세한 통찰력을 제공하는 주요 성능 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_9.png){zoomable=&quot;yes&quot;}{align="center"}

+++URL 및 클릭 스트림 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 수신자 수와 관련하여 게재에서 클릭한 대상 수신자 수의 비율입니다.

* **[!UICONTROL 고유 클릭수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 총 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 플랫폼 평균]** : 각 비율(반응성, 개별 클릭 및 누적된 클릭)에 표시되는 이 평균 비율은 이전 6개월 동안 전송된 게재에 대해 계산됩니다. 유형화가 동일한 게재 및 동일한 채널의 게재만 고려됩니다. 증명이 제외됩니다.
+++

### 가장 많이 방문한 상위 링크 10개 {#top10-global-report-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_top10_email"
>title="가장 많이 방문한 상위 링크 10개"
>abstract="**가장 많이 방문한 상위 링크 10개** 그래프와 표는 수신자와 각 링크의 상호 작용에 대한 포괄적인 데이터를 제공합니다."

다음 **[!UICONTROL 가장 많이 방문한 상위 10개 링크]** 그래프와 표에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_email_top10.png){zoomable=&quot;yes&quot;}{align="center"}

+++이장 많이 방문한 상위 10개 링크 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 총 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 백분율]**: 게재와 상호 작용한 사용자의 백분율입니다.

+++

### 시간 경과에 따른 클릭 분류 {#global-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_click_breakdown_email"
>title="시간 경과에 따른 클릭 분류"
>abstract="**시간 경과에 따른 클릭 분류** 그래프는 지정된 일정 동안 수신자가 링크에 어떻게 참여하는지에 대한 포괄적인 보기를 제공합니다."

다음 **[!UICONTROL 시간 경과에 따른 클릭 수 분류]** 그래프에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다.

![](assets/global_report_email_breakdown_clicks.png){zoomable=&quot;yes&quot;}{align="center"}

## 사용자 활동 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_user_activities_email"
>title="사용자 활동"
>abstract="**사용자 활동**&#x200B;을 그래픽으로 표현하면 정보가 풍부한 차트 형식을 통해 열람 및 클릭을 나타내어 수신자 상호 작용을 자세히 분석할 수 있습니다."

다음 **[!UICONTROL 사용자 활동]** 보고서는 차트 형태로 열람 및 클릭 수를 분류하여 보여줍니다. 이 보고서에 대한 지표는 아래에 자세히 설명되어 있습니다.

![](assets/global_report_email_user.png){zoomable=&quot;yes&quot;}{align="center"}

+++사용자 활동 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 총 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 총 열람 수]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 총 수신자 수입니다.

+++
