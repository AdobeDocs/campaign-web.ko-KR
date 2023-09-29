---
audience: end-user
title: 이메일 채널에 대한 캠페인 보고서
description: 이메일 채널에 대한 캠페인 보고서에 대해 자세히 알아보기
badge: label="Beta"
source-git-commit: 5d577c07c4d754e9265482f858c17740f304db42
workflow-type: tm+mt
source-wordcount: '1568'
ht-degree: 9%

---


# 이메일 채널에 대한 캠페인 보고서 {#campaign-reports-email-channel}

각 캠페인 보고서는 캠페인의 성공 및 오류를 자세히 설명하는 다양한 위젯으로 나뉩니다. 이메일 채널의 경우 보고서 및 지표가 아래에 자세히 설명되어 있습니다. 에서 캠페인 보고서에 액세스하는 방법 알아보기 [이 페이지](campaign-reports.md).

## 게재 요약 {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="게재 개요"
>abstract="다음 **게재 개요** 은 방문자의 이메일 게재 참여도에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다."

### 게재 개요 {#delivery-summary-email-ovv}

다음 **[!UICONTROL 게재 개요]** 보고서는 방문자의 이메일 게재 참여도에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_1.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 총 전송됨]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 전달됨]**: 성공적으로 전송된 메시지 수와 총 전송된 메시지 수

* **[!UICONTROL 바운스]**: 총 보낸 메시지 수와 관련하여 게재 및 자동 반환 처리 중에 누적된 총 오류.

* **[!UICONTROL 고유 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

+++

### 초기 타겟 대상자 통계 {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="초기 타겟 대상자 통계"
>abstract="초기 타겟 대상자 통계 테이블에는 수신자와 관련된 데이터가 표시됩니다."


다음 **[!UICONTROL 초기 타겟 대상 통계]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_2.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 초기 대상자]**: 타겟팅된 총 수신자 수.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 규칙에 의해 거부됨]**&#x200B;차단 목록에 추가하다 : 분석 중에 무시된 총 주소 수: 격리된 주소, 격리된 주소 수 등 규칙 적용 시

+++

### 실행 통계 {#delivery-summary-email-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="실행 통계"
>abstract="다음 **실행 통계** 표에는 게재의 성공, 즉 게재할 메시지, 성공, 오류 및 새로운 격리에 대해 자세히 설명되어 있습니다."

다음 **[!UICONTROL 실행 통계]** 게재의 성공 여부를 표로 자세히 설명합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_3.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새로운 격리]**: 배달할 메시지 수와 관련하여 배달 실패 후 격리된 총 주소 수(사용자 알 수 없음, 잘못된 도메인)입니다.

  이메일 오류 유형은 [Adobe Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.


+++

### 반응 통계 {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="반응 통계"
>abstract="다음 **반응 통계** 이 표에서는 게재 시 수신자 활동에 사용할 수 있는 데이터, 즉 열기, 구독, 구독 취소, 미러 페이지 링크 클릭수를 보여 줍니다."


다음 **[!UICONTROL 반응 통계]** 표에는 게재를 위한 수신자 활동에 사용 가능한 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_4.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 고유 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 구독 취소]**: 해당 기간 동안 구독 취소를 클릭한 수신자 수입니다.

* **[!UICONTROL 미러 페이지]**: 미러 페이지 링크를 클릭한 수신자 수입니다.

* **[!UICONTROL 발송]**: 이메일을 전달한 수신자 수를 클릭한 수입니다.
+++

### 생성된 클릭스트림 {#delivery-summary-email-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_click_streams"
>title="생성된 클릭스트림"
>abstract="다음 **생성된 클릭 스트림** 표는 수신자가 게재와 상호 작용하는 방법과 관련하여 사용 가능한 데이터를 보여 줍니다."

다음 **[!UICONTROL 생성된 클릭 스트림]** 테이블에는 수신자와 게재의 상호 작용 방식에 따른 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_5.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 수신자 수와 관련하여 게재에서 클릭한 대상 수신자 수의 비율입니다.

+++

## 비게재 항목 {#non-deliverables-email}

### 유형별 오류 분류 {#delivery-summary-email-breakdown-per-type}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="유형별 오류 분류"
>abstract="다음 **유형별 오류 분류** 테이블 및 그래프에는 알 수 없는 사용자, 사서함 가득 참, 잘못된 도메인 등의 각 오류 유형에 사용할 수 있는 데이터가 포함되어 있습니다."

다음 **[!UICONTROL 유형별 오류 분류]** 표 및 그래프에는 각 도메인 유형에 대해 발생할 수 있는 오류에 대해 사용 가능한 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

이 보고서에 표시된 오류는 격리 프로세스를 트리거합니다. 격리 관리에 대한 자세한 내용은 다음을 참조하십시오. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

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
>id="acw_campaign_reporting_error_domain"
>title="도메인별 오류 분류"
>abstract="다음 **도메인별 오류 분류** 표 및 그래프는 각 도메인에 따라 발생한 각 오류 유형에 대해 사용 가능한 데이터를 표시합니다."


다음 **[!UICONTROL 도메인별 오류 분류]** 표 및 그래프에는 각 도메인에서 발생할 수 있는 오류에 대해 사용 가능한 데이터가 포함되어 있습니다. 지표는 **[!UICONTROL 유형별 오류 분류]** 위에 자세히 설명된 표 및 그래프입니다.


## 지표 추적 {#tracking-indicators-email}

### 게재 통계 {#delivery-summary-email-statistics}


>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="게재 통계"
>abstract="다음 **게재 통계** 그래프는 게재의 성공 및 발생한 오류를 자세히 설명합니다."

다음 **[!UICONTROL 게재 통계]** 지표는 보낸 이메일에 사용할 수 있는 데이터에 대한 자세한 정보를 제공하는 주요 성능 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_7.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 고유 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 옵트아웃 링크 클릭]**: 구독 취소 링크의 클릭 수입니다.

* **[!UICONTROL 미러 링크 클릭]**: 미러 페이지 링크를 클릭한 횟수.

* **[!UICONTROL 발송 예측]**: 타겟팅된 수신자가 전달한 이메일 수 예상.
+++

### 열람 및 클릭스루 비율 {#delivery-summary-open-rate}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="열람 및 클릭스루 비율"
>abstract="**열람 및 클릭스루 비율** 표에 게재를 이용하는 수신자와 관련된 데이터가 표시됩니다."



다음 **[!UICONTROL 열람 및 클릭스루 비율]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_8.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 전송됨]**: 전송된 총 메시지 수입니다.

* **[!UICONTROL 컴플레인]**: 수신자가 원치 않는 것으로 보고한 이 도메인에 대한 메시지 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 클릭수]**: 동일한 게재를 한 번 이상 클릭한 고유한 타깃팅된 수신자 수입니다.

* **[!UICONTROL 원시 재활동]**: 게재를 한 번 이상 클릭한 수신자 수와 게재를 한 번 이상 연 수신자 수의 비율입니다.
+++

## URL 및 클릭 스트림 {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="URL 및 클릭 스트림"
>abstract="다음 **URL 및 클릭 스트림** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다."

다음 **[!UICONTROL URL 및 클릭 스트림]** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_9.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 수신자 수와 관련하여 게재에서 클릭한 대상 수신자 수의 비율입니다.

* **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 플랫폼 평균]** : 각 비율(반응성, 개별 클릭 및 누적된 클릭)에 표시되는 이 평균 비율은 이전 6개월 동안 전송된 게재에 대해 계산됩니다. 유형화가 동일한 게재 및 동일한 채널의 게재만 고려됩니다. 증명이 제외됩니다.
+++

### 가장 많이 방문한 상위 링크 10개 {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="가장 많이 방문한 상위 링크 10개"
>abstract="다음 **가장 많이 방문한 상위 10개 링크** rgraph 및 표에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다."


다음 **[!UICONTROL 가장 많이 방문한 상위 10개 링크]** 그래프와 표에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_10.png)

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 백분율]**: 게재와 상호 작용한 사용자의 백분율입니다.

+++

### 시간 경과에 따른 클릭수 분류 {#campaign-report-email-breakdown-clicks}


>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="시간 경과에 따른 클릭수 분류"
>abstract="다음 **시간 경과에 따른 클릭 수 분류** 그래프는 링크당 수신자 동작에 사용할 수 있는 데이터를 보여 줍니다."


다음 **[!UICONTROL 시간 경과에 따른 클릭 수 분류]** 그래프에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다.

![](assets/campaign_report_email_11.png)


## 사용자 활동 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="사용자 활동"
>abstract="**사용자 활동** 그래프에 열람 및 클릭의 분류가 차트 형식으로 표시됩니다."

다음 **[!UICONTROL 사용자 활동]** 보고서는 차트 형태로 열람 및 클릭 수를 분류하여 보여줍니다. 이 보고서에 대한 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_email_10.png){align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

+++
