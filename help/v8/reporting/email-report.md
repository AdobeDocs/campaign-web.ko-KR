---
audience: end-user
title: 이메일 게재 보고서
description: 이메일 게재 보고서에 액세스하고 사용하는 방법을 알아봅니다
badge: label="Beta"
source-git-commit: f2ae73ce56e2e5128fecd8b74a6bdb096b8b75ec
workflow-type: tm+mt
source-wordcount: '2205'
ht-degree: 8%

---

# 이메일 게재 보고서 {#email-report}

다음 **이메일 게재 보고서** 은 이메일 채널과 관련된 포괄적인 통찰력과 데이터를 제공합니다. 개별 게재의 성과, 효율성 및 결과에 대해 자세한 정보와 함께 포괄적인 개요를 제공합니다.

## 게재 요약 {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="전송 보고"
>abstract="그는 **전송 중** 보고서 내의 탭에서는 게재 관련 방문자의 상호 작용 및 발생 가능한 오류에 대한 심층적인 통찰력을 제공합니다."

### 초기 대상 집단 {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="초기 대상 집단"
>abstract="다음 **초기 대상 모집단** 그래프는 게재 준비 결과를 기반으로 수신자 및 메시지와 관련된 데이터를 표시합니다."

다음 **[!UICONTROL 초기 대상 모집단]** 그래프는 수신자와 관련된 데이터를 표시합니다. 지표는 게재를 준비하는 동안 계산되며 초기 대상자, 보낼 메시지 수, 제외된 수신자 수를 표시합니다.

![](assets/reporting_email_1.png){align="center" zoomable="yes"}

정확한 숫자를 표시하려면 마우스를 그래프의 일부 위에 놓습니다.

![](assets/reporting_email_1.1.png){align="center" zoomable="yes"}


+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 초기 대상자]**: 타겟팅된 총 수신자 수.

* **[!UICONTROL 게재하기]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 제외]**: 대상 모집단에서 제외된 총 수신자 수입니다.
+++

### 게재 통계 {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="게재 통계"
>abstract="다음 **게재 통계** 그래프는 게재의 성공 및 발생한 오류를 자세히 설명합니다."


다음 **[!UICONTROL 게재 통계]** 그래프는 게재의 성공을 자세히 설명합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/reporting_email_2.png){align="center" zoomable="yes"}

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 메시지 전송됨]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새로운 격리]**: 배달할 메시지 수와 관련하여 배달 실패 후 격리된 총 주소 수(사용자 알 수 없음, 잘못된 도메인)입니다.

+++

### 제외 이유  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="게재 통계"
>abstract="다음 **제외 이유** 그래프와 표는 게재를 준비하는 동안 거부된 메시지의 규칙별 분류를 보여 줍니다."


다음 **[!UICONTROL 제외 이유]** 그래프와 표는 게재를 준비하는 동안 거부된 메시지의 규칙별 분류를 보여 줍니다. 제외 규칙은 다음에 자세히 설명되어 있습니다. [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 알 수 없는 사용자]**: 이메일 주소가 잘못되었음을 나타내기 위해 게재 중에 생성된 오류 유형.

* **[!UICONTROL 잘못된 도메인]**: 이메일 주소의 도메인이 잘못되었거나 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성되는 오류 유형입니다.

* **[!UICONTROL 사서함 가득 참]**: 5회 게재 시도 후 생성된 오류 유형은 수신자의 받은 편지함에 메시지가 너무 많음을 나타냅니다.

* **[!UICONTROL 계정 비활성화]**: 주소가 더 이상 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성된 오류 유형.

* **[!UICONTROL 거부됨]**: IAP(인터넷 액세스 공급자)에서 주소를 거부할 때 오류 유형 이 생성됩니다(예: 보안 규칙 적용 후).

* **[!UICONTROL 연결할 수 없음]**: 메시지 배포 문자열에서 발생하는 오류 유형: SMTP 릴레이 장애, 일시적으로 도메인에 연결할 수 없음 등

* **[!UICONTROL 연결되지 않음]**: 전송 시 수신자의 휴대폰이 꺼져 있거나 네트워크에서 연결이 끊겼음을 나타내는 오류 유형입니다.

+++

## 게재 처리량 {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="게재 처리량 위젯"
>abstract="다음 **게재 처리량** 보고서는 지정된 기간 내에 전체 플랫폼의 게재 처리량에 대한 자세한 정보를 제공합니다."

이 보고서는 지정된 기간 내에 전체 플랫폼의 게재 처리량에 대한 자세한 정보를 제공합니다. 메시지 게재 속도를 측정하는 데 사용되는 기본 지표는 시간당 전송된 메시지 수입니다.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## 브로드캐스트 통계 {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="브로드캐스트 통계 위젯"
>abstract="다음 **브로드캐스트 통계** 보고서에는 각 도메인에서 발생할 수 있는 오류에 대해 사용 가능한 데이터가 포함되어 있습니다."

다음 **[!UICONTROL 브로드캐스트 통계]** 표에는 각 도메인에서 발생할 수 있는 오류에 대해 사용 가능한 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 처리된 이메일]**: 게재 서버에서 처리된 총 메시지 수입니다.

* **[!UICONTROL 전달됨]**: 처리된 총 메시지 수와 비교하여 성공적으로 처리된 메시지 수의 백분율입니다.

* **[!UICONTROL 하드 바운스]**: 처리된 총 메시지 수와 비교하여 잘못된 이메일 주소와 같은 영구적인 &quot;하드&quot; 바운스 수 비율입니다.

* **[!UICONTROL 소프트 바운스]**: 처리된 총 메시지 수 대비 전체 받은 편지함과 같은 일시적인 오류인 &quot;소프트&quot; 바운스 수의 비율입니다

* **[!UICONTROL 열림]**: 성공적으로 처리된 메시지 수와 비교하여 메시지를 한 번 이상 연 타겟팅된 수신자 수의 백분율입니다.

* **[!UICONTROL 클릭수]**: 성공적으로 처리된 메시지 수와 비교하여 게재를 한 번 이상 클릭한 사람 수의 백분율입니다.

* **[!UICONTROL 구독 취소]**: 성공적으로 처리된 메시지 수와 비교한 구독 취소 링크의 클릭 수의 백분율입니다.
+++

## 비게재 항목 {#non-deliverables-email}

### 유형별 오류 분류 {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="유형별 오류 분류"
>abstract="다음 **유형별 오류 분류** 테이블 및 그래프에는 알 수 없는 사용자, 사서함 가득 참, 잘못된 도메인 등의 각 오류 유형에 사용할 수 있는 데이터가 포함되어 있습니다."

다음 **[!UICONTROL 유형별 오류 분류]** 테이블 및 그래프에는 오류 유형에 사용할 수 있는 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

이 보고서에 표시된 오류는 격리 프로세스를 트리거합니다. 격리 관리에 대한 자세한 내용은 다음을 참조하십시오. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 알 수 없는 사용자]**: 이메일 주소가 잘못되었음을 나타내기 위해 게재 중에 생성된 오류 유형.

* **[!UICONTROL 잘못된 도메인]**: 이메일 주소의 도메인이 잘못되었거나 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성되는 오류 유형입니다.

* **[!UICONTROL 사서함 가득 참]**: 5회 게재 시도 후 생성된 오류 유형은 수신자의 받은 편지함에 메시지가 너무 많음을 나타냅니다.

* **[!UICONTROL 계정 비활성화]**: 주소가 더 이상 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성된 오류 유형.

* **[!UICONTROL 거부됨]**: IAP(인터넷 액세스 공급자)에서 주소를 거부할 때 오류 유형 이 생성됩니다(예: 보안 규칙 적용 후).

* **[!UICONTROL 연결할 수 없음]**: 메시지 배포 문자열에서 발생하는 오류 유형: SMTP 릴레이 장애, 일시적으로 도메인에 연결할 수 없음 등

* **[!UICONTROL 연결되지 않음]**: 전송 시 수신자의 휴대폰이 꺼져 있거나 네트워크에서 연결이 끊겼음을 나타내는 오류 유형입니다.

+++


### 도메인별 오류 분류 {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="도메인별 오류 분류"
>abstract="다음 **도메인별 오류 분류** 표 및 그래프는 각 도메인에 따라 발생한 각 오류 유형에 대해 사용 가능한 데이터를 표시합니다."


다음 **[!UICONTROL 도메인별 오류 분류]** 표 및 그래프는 각 도메인에서 발생할 수 있는 오류에 대해 사용 가능한 데이터를 표시합니다.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

각 도메인 이름 옆에 있는 아이콘을 클릭하여 세부 정보를 확인합니다.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

사용 가능한 지표는 와 동일합니다. [유형별 오류 분류](#email-delivery-breakdown-type) 위에서 설명했습니다.

## 지표 추적 {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="보고 추적"
>abstract="다음 **추적** 보고서 내의 탭은 링크당 수신자 동작, 열기 및 클릭 분류와 게재 중 가장 자주 클릭한 URL에 대한 세부 정보를 포함하여 중요한 데이터를 제공합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="열람 및 클릭스루 비율 위젯"
>abstract="다음 **열람 및 클릭스루 비율** 테이블에는 게재 시 수신자 참여와 관련된 데이터가 표시됩니다."

### 게재 통계  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" 게재 통계"
>abstract="다음 **게재 통계** 보고서는 보낸 이메일에 사용할 수 있는 데이터에 대한 성공, 열기, 클릭 수 등과 같은 자세한 정보를 제공하는 주요 성능 지표(KPI)를 제공합니다."


다음 **[!UICONTROL 게재 통계]** 보고서는 보낸 이메일에 사용할 수 있는 데이터에 대한 자세한 정보를 제공하는 주요 성능 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/reporting_email_5.png){align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 고유 열람 수]**: 메시지를 한 번 이상 연 타겟팅된 총 수신자 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 옵트아웃 링크 클릭]**: 구독 취소 링크의 클릭 수입니다.

* **[!UICONTROL 미러 링크 클릭]**: 미러 페이지 링크를 클릭한 횟수.

* **[!UICONTROL 발송 예측]**: 타겟팅된 수신자가 전달한 이메일 수 예상.
+++

### 열람 및 클릭스루 비율 {#email-tracking-click-through}

다음 **[!UICONTROL 열람 및 클릭스루 비율]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/reporting_email_6.png){align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 전송됨]**: 전송된 총 메시지 수입니다.

* **[!UICONTROL 컴플레인]**: 수신자가 원치 않는 것으로 보고한 이 도메인에 대한 메시지 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

* **[!UICONTROL 클릭수]**: 동일한 게재를 한 번 이상 클릭한 고유한 타깃팅된 수신자 수입니다.

* **[!UICONTROL 원시 재활동]**: 게재를 한 번 이상 클릭한 수신자 수와 게재를 한 번 이상 연 수신자 수의 비율입니다.
+++

## URL 및 클릭 스트림 {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL 및 클릭 스트림 위젯"
>abstract="다음 **URL 및 클릭 스트림** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다."

* 다음 **[!UICONTROL URL 및 클릭 스트림]** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다.

  ![](assets/reporting_email_7.png){align="center"}

  +++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

   * **[!UICONTROL 반응성]**: 게재를 연 예상 대상 수신자 수와 관련하여 게재에서 클릭한 대상 수신자 수의 비율입니다.

   * **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

   * **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

   * **[!UICONTROL 플랫폼 평균]** : 각 비율(반응성, 개별 클릭 및 누적된 클릭)에 표시되는 이 평균 비율은 이전 6개월 동안 전송된 게재에 대해 계산됩니다. 유형화가 동일한 게재 및 동일한 채널의 게재만 고려됩니다. 증명이 제외됩니다.

+++

* **[!UICONTROL 가장 많이 방문한 상위 10개 링크]** 그래프와 표에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다.

  ![](assets/reporting_email_8.png){align="center"}

  +++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

   * **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

   * **[!UICONTROL 백분율]**: 게재와 상호 작용한 사용자의 백분율입니다.

+++

* **[!UICONTROL 시간 경과에 따른 클릭 수 분류]** 그래프에는 링크당 수신자 동작에 사용할 수 있는 데이터가 포함되어 있습니다.

  ![](assets/reporting_email_9.png){align="center"}

## 사용자 활동 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="사용자 활동 위젯"
>abstract="다음 **사용자 활동** 그래프는 차트 형태로 열람 및 클릭에 대한 분류를 보여줍니다. 데이터를 타겟팅할 기간을 선택할 수 있습니다(마지막 날 또는 시간 또는 30분)."

다음 **[!UICONTROL 사용자 활동]** 보고서는 차트 형태로 열람 및 클릭 수를 분류하여 보여줍니다. 데이터를 타겟팅할 기간을 선택할 수 있습니다(마지막 날 또는 시간 또는 30분).

![](assets/reporting_email_10.png){align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

+++

## 추적 통계 {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="추적 통계 위젯"
>abstract="다음 **추적 통계** 그래프는 열람 및 클릭에 대한 통계를 제공합니다. 데이터를 타겟팅할 특정 시간대를 선택할 수 있는 옵션이 있습니다."

다음 **[!UICONTROL 추적 통계]** 그래프는 열람 및 클릭에 대한 통계를 제공합니다. 데이터를 타겟팅할 특정 시간대를 선택할 수 있는 옵션이 있습니다.

![](assets/reporting_email_11.png){align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 열림]**: 이 도메인에 대해 최소 한 번 이상 메시지를 연 고유한 타겟팅된 수신자 수입니다.

+++

## 열람수 분류 {#breakdown-opens}


### 장치별 열기 분류 {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="디바이스별 분류"
>abstract="다음 **장치별 분류** 이 보고서는 해당 기간에 대한 장치별 열기 분류를 보여줍니다. 각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째는 각 장치 유형에 대한 정확한 숫자와 백분율을 표시합니다."

다음 **장치별 분류** 이 보고서는 개인용 컴퓨터, Android 장치, Apple 장치 또는 기타 장치와 같은 기간에 대한 장치별 열기 분류를 보여줍니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째는 각 장치 유형에 대한 정확한 숫자와 백분율을 표시합니다.

![](assets/reporting_email_13.png){align="center"}


### OS별 열기 분류 {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="운영 체제별 분류"
>abstract="다음 **OS별 분류** 보고서는 해당 기간에 대한 운영 체제별 열기 분석을 보여 줍니다. 첫 번째 차트에는 컴퓨터 및 모바일 장치의 열림에 대한 통계가 표시됩니다. 두 번째는 각 OS에 대한 정확한 숫자와 백분율을 표시합니다."

다음 **OS별 분류** 이 보고서는 Windows 시스템, Android 시스템, iOS 시스템 또는 기타 운영 체제별 열기 분류를 보여줍니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 화면에 컴퓨터 및 모바일 운영 체제의 열림에 대한 통계가 표시됩니다. 두 번째는 각 운영 체제에 대한 정확한 숫자와 백분율을 표시합니다.

![](assets/reporting_email_13.1.png){align="center"}

### 브라우저별 열기 분류 {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="브라우저별 분류"
>abstract="다음 **브라우저별 분류** 기간 동안의 브라우저별 열기 분류를 표시합니다. 첫 번째 차트에는 컴퓨터 및 모바일 장치의 열림에 대한 통계가 표시됩니다. 두 번째는 각 브라우저의 정확한 수와 백분율을 표시합니다."

다음 **브라우저별 분류** 보고서는 Chrome, Safari, Internet Explorer 등의 브라우저별 열기 분류를 표시합니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 화면에 컴퓨터 및 모바일 운영 체제의 열림에 대한 통계가 표시됩니다. 두 번째는 각 브라우저의 정확한 수와 백분율을 표시합니다.

![](assets/reporting_email_13.2.png){align="center"}


## 핫클릭 {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Hotclicks 보고서"
>abstract="다음 **핫클릭** 보고서는 각 링크에서 링크 클릭률의 이메일 콘텐츠(HTML 및/또는 텍스트)를 제공합니다. 개인화 블록, 구독 취소 링크, 미러 페이지 링크 및 오퍼 링크는 누적된 총 클릭 수에서 고려되지만 보고서에 표시되지 않습니다."

이 보고서에는 메시지 콘텐츠(HTML 및/또는 텍스트)와 각 링크의 링크 클릭 비율이 표시됩니다. 개인화 블록, 구독 취소 링크, 미러 페이지 링크 및 오퍼 링크는 누적된 총 클릭 수에서 고려되지만 보고서에 표시되지 않습니다.

![](assets/reporting11.png)
