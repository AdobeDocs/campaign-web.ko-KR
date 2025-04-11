---
audience: end-user
title: 이메일 게재 보고서
description: 이메일 게재 보고서에 액세스하고 사용하는 방법을 알아봅니다
exl-id: 2a0bd3e9-5d75-47c8-bd6a-b3e0b1ce0a01
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 37%

---

# 이메일 게재 보고서 {#email-report}

**전자 메일 게재 보고서**&#x200B;는 전자 메일 채널과 관련된 포괄적인 통찰력과 데이터를 제공합니다. 개별 게재의 성과, 효율성 및 결과에 대해 자세한 정보와 함께 포괄적인 개요를 제공합니다.

## 게재 요약 {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="보고 전송"
>abstract="보고서 내의 **전송** 탭은 방문자와 게재 간의 상호 작용 및 방문자가 경험할 수 있는 잠재적인 오류에 대한 심층적인 인사이트를 제공합니다."

### 초기 대상 집단 {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="초기 대상 집단"
>abstract="**초기 대상 집단** 그래프에는 게재 준비의 결과를 바탕으로 수신자 및 메시지 관련 데이터가 표시됩니다."

**[!UICONTROL 초기 대상 모집단]** 그래프는 수신자와 관련된 데이터를 표시합니다. 지표는 게재를 준비하는 동안 계산되며 초기 대상자, 보낼 메시지 수, 제외된 수신자 수를 표시합니다.

데이터를 표시하는 그래프의 ![스크린샷](assets/reporting_email_1.png){zoomable="yes"}

정확한 숫자를 표시하려면 마우스를 그래프의 일부 위에 놓습니다.

![정확한 숫자를 표시하는 부분에 마우스를 올려 놓은 그래프의 스크린샷](assets/reporting_email_1.1.png){zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 초기 대상]**: 타깃팅된 총 받는 사람 수

* **[!UICONTROL 게재]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 제외]**: 대상 모집단에서 제외된 총 받는 사람 수입니다.
+++

### 게재 통계 {#email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="게재 통계"
>abstract="**게재 통계** 그래프에 게재 성공과 발생한 오류가 자세히 표시됩니다."

**[!UICONTROL 게재 통계]** 그래프는 게재 성공 여부를 자세히 설명합니다. 지표는 아래에 자세히 설명되어 있습니다.

![게재 통계의 세부 정보를 보여 주는 그래프의 스크린샷](assets/reporting_email_2.png){zoomable="yes"}

+++이메일 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 보낸 메시지]**: 게재를 준비한 후 배달할 총 메시지 수입니다.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 배달할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새 격리]**: 배달할 메시지 수와 관련하여 배달 실패(사용자 알 수 없음, 잘못된 도메인) 후에 격리된 총 주소 수입니다.

+++

### 제외 이유  {#email-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="제외 이유 게재"
>abstract="**제외 이유** 그래프와 테이블에는 게재 준비 단계에서 거부된 메시지 규칙당 분류가 표시됩니다."

**[!UICONTROL 제외 원인]** 그래프 및 표는 게재를 준비하는 동안 거부된 메시지의 규칙별 분류를 보여 줍니다. 제외 규칙은 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}에 자세히 설명되어 있습니다.

![제외 그래프 및 표의 스크린샷](assets/reporting_email_3.png){zoomable="yes"}{align="center" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 사용자 알 수 없음]**: 전자 메일 주소가 잘못되었음을 나타내기 위해 배달하는 동안 오류 유형이 생성되었습니다.

* **[!UICONTROL 잘못된 도메인]**: 전자 메일 주소의 도메인이 잘못되었거나 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성되는 오류 유형입니다.

* **[!UICONTROL 사서함 가득 참]**: 받는 사람의 받은 편지함에 메시지가 너무 많음을 나타내기 위해 다섯 번 배달을 시도한 후에 생성된 오류 형식입니다.

* **[!UICONTROL 계정 사용 안 함]**: 주소가 더 이상 존재하지 않음을 나타내기 위해 게재를 보낼 때 오류 유형이 생성되었습니다.

* **[!UICONTROL 거부됨]**: IAP(인터넷 액세스 공급자)에서 주소를 거부할 때 생성되는 오류 형식(예: 보안 규칙(스팸 방지 소프트웨어) 적용 후)입니다.

* **[!UICONTROL 연결할 수 없음]**: 메시지 배포 문자열에서 발생하는 오류 유형: SMTP 릴레이에 문제 발생, 일시적으로 도메인에 연결할 수 없음 등

* **[!UICONTROL 연결되지 않음]**: 전송 시 받는 사람의 휴대폰이 꺼져 있거나 네트워크에서 연결이 끊어져 있음을 나타내는 오류 형식입니다.

+++

## 게재 처리량 {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="게재 처리량"
>abstract="**게재 처리량** 보고서는 지정된 기간 내 전체 플랫폼의 게재 처리량에 대한 자세한 정보를 제공합니다."

이 보고서는 지정된 기간 내에 전체 플랫폼의 게재 처리량에 대한 자세한 정보를 제공합니다. 메시지 게재 속도를 측정하는 데 사용되는 주요 지표는 시간당 전송된 메시지 수입니다.

![게재 처리량의 스크린샷](assets/reporting_email_3.1.png){zoomable="yes"}{align="center" zoomable="yes"}


## 브로드캐스트 통계 {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="브로드캐스트 통계"
>abstract="**브로드캐스트 통계** 보고서에는 각 도메인에서 발생한 잠재 오류에 대한 사용 가능한 데이터가 포함되어 있습니다."

**[!UICONTROL 브로드캐스트 통계]** 표에는 각 도메인에서 발생한 오류에 대해 사용 가능한 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

![브로드캐스트 통계의 스크린샷](assets/reporting_email_4.png){zoomable="yes"}{align="center" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 처리된 전자 메일]**: 게재 서버에서 처리된 총 메시지 수입니다.

* **[!UICONTROL 배달됨]**: 처리된 총 메시지 수와 비교하여 성공적으로 처리된 메시지 수의 백분율입니다.

* **[!UICONTROL 하드 바운스]**: 처리된 총 메시지 수와 비교하여 &quot;하드&quot; 바운스 수, 잘못된 이메일 주소와 같은 영구 오류의 비율입니다.

* **[!UICONTROL 소프트 바운스]**: 처리된 총 메시지 수와 비교하여 &quot;소프트&quot; 바운스 수, 전체 받은 편지함과 같은 임시 오류의 비율

* **[!UICONTROL 열기]**: 메시지를 한 번 이상 연 대상 받는 사람 수와 성공적으로 처리된 메시지 수의 비율입니다.

* **[!UICONTROL 클릭 수]**: 배달을 한 번 이상 클릭한 사람 수와 성공적으로 처리된 메시지 수의 비율입니다.

* **[!UICONTROL 구독 취소]**: 성공적으로 처리된 메시지 수와 비교한 구독 취소 링크의 클릭 수의 백분율입니다.
+++

## 비게재 항목 {#non-deliverables-email}

### 유형별 오류 분류 {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="유형별 오류 분류"
>abstract="**유형별 오류 분류** 그래프에는 발생한 각 오류 유형(알 수 없는 사용자, 사서함 가득 참, 잘못된 도메인 등)과 관련하여 사용 가능한 데이터가 포함되어 있습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type_table"
>title="유형별 오류 분류"
>abstract="**유형별 오류 분류** 테이블은 각 오류 유형의 발생에 대한 포괄적인 분석을 제공합니다."

**[!UICONTROL 유형별 오류 분석]** 테이블 및 그래프에 오류 유형에 사용할 수 있는 데이터가 포함되어 있습니다. 지표는 아래에 자세히 설명되어 있습니다.

이 보고서에 표시된 오류는 격리 프로세스를 트리거합니다. 격리 관리에 대한 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}를 참조하세요.

![유형별 오류 중단의 스크린샷](assets/campaign_report_email_6.png){zoomable="yes"}{align="left" zoomable="yes"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 사용자 알 수 없음]**: 전자 메일 주소가 잘못되었음을 나타내기 위해 배달하는 동안 오류 유형이 생성되었습니다.

* **[!UICONTROL 잘못된 도메인]**: 전자 메일 주소의 도메인이 잘못되었거나 존재하지 않음을 나타내기 위해 게재를 보낼 때 생성되는 오류 유형입니다.

* **[!UICONTROL 사서함 가득 참]**: 받는 사람의 받은 편지함에 메시지가 너무 많음을 나타내기 위해 다섯 번 배달을 시도한 후에 생성된 오류 형식입니다.

* **[!UICONTROL 계정 사용 안 함]**: 주소가 더 이상 존재하지 않음을 나타내기 위해 게재를 보낼 때 오류 유형이 생성되었습니다.

* **[!UICONTROL 거부됨]**: IAP(인터넷 액세스 공급자)에서 주소를 거부할 때 생성되는 오류 형식(예: 보안 규칙(스팸 방지 소프트웨어) 적용 후)입니다.

* **[!UICONTROL 연결할 수 없음]**: 메시지 배포 문자열에서 발생하는 오류 유형: SMTP 릴레이에 문제 발생, 일시적으로 도메인에 연결할 수 없음 등

* **[!UICONTROL 연결되지 않음]**: 전송 시 받는 사람의 휴대폰이 꺼져 있거나 네트워크에서 연결이 끊어져 있음을 나타내는 오류 형식입니다.

+++

### 도메인별 오류 분류 {#email-delivery-breakdown-domain}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="도메인별 오류 분류"
>abstract="**도메인별 오류 분류** 그래프에는 각 도메인에 따라 발생한 각 오류 유형에 대해 사용 가능한 데이터가 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain_table"
>title="도메인별 오류 분류"
>abstract="**도메인별 오류 분류** 테이블은 사용된 도메인에 따라 각 오류 발생에 대한 포괄적인 분석을 제공합니다."

**[!UICONTROL 도메인당 오류 분석]** 테이블 및 그래프는 각 도메인에서 발생한 오류에 대해 사용 가능한 데이터를 표시합니다.

![도메인별 오류 분석 스크린샷](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

각 도메인 이름 옆에 있는 아이콘을 클릭하여 세부 정보를 확인합니다.

![각 도메인의 세부 정보가 포함된 도메인별 오류 분류의 스크린샷](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

사용 가능한 지표는 위에서 설명한 유형별 [오류 분류](#email-delivery-breakdown-type)와 동일합니다.

## 지표 추적 {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="보고 추적"
>abstract="보고서의 **추적** 탭은 링크당 수신자 비헤이비어, 열람 및 클릭 분석, 게재 중 가장 자주 클릭한 URL에 대한 자세한 정보 등 중요 데이터를 제공합니다."


### 게재 통계  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" 게재 통계"
>abstract="**게재 통계** 보고서는 보낸 이메일에 사용할 수 있는 데이터에 대한 자세한 정보를 포함하는 주요 성과 지표(KPI, 예: 성공, 열람 수, 클릭 수 등)를 제공합니다."


**[!UICONTROL 게재 통계]** 보고서는 보낸 전자 메일에 사용할 수 있는 데이터에 대한 자세한 정보를 제공하는 주요 성능 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![게재 통계의 스크린샷](assets/reporting_email_5.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 처리된 메시지 수입니다.

* **[!UICONTROL 고유 열기 수]**: 메시지를 한 번 이상 연 총 대상 받는 사람 수입니다.

* **[!UICONTROL 열기]**: 메시지를 한 번 이상 연 이 도메인의 개별 대상 받는 사람 수입니다.

* **[!UICONTROL 옵트아웃 링크 클릭 수]**: 구독 취소 링크 클릭 수.

* **[!UICONTROL 미러 링크 클릭 수]**: 미러 페이지 링크 클릭 수.

* **[!UICONTROL 전달 예상]**: 대상 받는 사람이 전달한 전자 메일 수를 예상합니다.
+++

### 열람 및 클릭스루 비율 {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="열람 및 클릭스루 비율"
>abstract="**열람 및 클릭스루 비율** 테이블에 게재를 이용하는 수신자와 관련된 데이터가 표시됩니다."



**[!UICONTROL 열기 및 클릭스루 비율]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

열기 및 클릭스루 비율 테이블의 ![스크린샷](assets/reporting_email_6.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 전송됨]**: 보낸 총 메시지 수

* **[!UICONTROL 컴플레인]**: 받는 사람이 원치 않는 것으로 보고한 이 도메인에 대한 메시지 수입니다.

* **[!UICONTROL 열기]**: 메시지를 한 번 이상 연 이 도메인의 개별 대상 받는 사람 수입니다.

* **[!UICONTROL 클릭 수]**: 같은 게재를 한 번 이상 클릭한 고유한 대상 받는 사람의 수입니다.

* **[!UICONTROL 원시 재활동]**: 게재를 한 번 이상 클릭한 수신자 수와 한 번 이상 연 수신자 수의 비율입니다.
+++

## URL 및 클릭 스트림 {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL 및 클릭 스트림"
>abstract="**URL 및 클릭스트림** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 포함하는 주요 성과 지표(KPI)를 제공합니다."


**[!UICONTROL URL 및 클릭스트림]** 보고서는 게재 중 가장 많이 클릭한 URL에 대한 자세한 정보를 포함하는 주요 성과 지표(KPI)를 제공합니다.

![URL 및 클릭 스트림 보고서의 스크린샷](assets/reporting_email_7.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 받는 사람 수와 관련하여 게재를 클릭한 대상 받는 사람 수의 비율입니다.

* **[!UICONTROL 고유 클릭 수]**: 게재를 한 번 이상 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 클릭 수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 플랫폼 평균]**: 각 비율(반응성, 개별 클릭 수 및 누적된 클릭 수) 아래에 표시되는 이 평균 비율은 이전 6개월 동안 전송된 게재에 대해 계산됩니다. 유형화가 동일한 게재 및 동일한 채널의 게재만 고려됩니다. 증명이 제외됩니다.

+++

### 가장 많이 방문한 상위 링크 10개 {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="가장 많이 방문한 상위 링크 10개"
>abstract="**가장 많이 방문한 상위 링크 10개** 그래프와 테이블에는 링크당 수신자 비헤이비어와 관련하여 사용 가능한 데이터가 포함되어 있습니다."


**[!UICONTROL 가장 많이 방문한 상위 링크 10개]** 그래프와 테이블에는 링크당 수신자 비헤이비어와 관련하여 사용 가능한 데이터가 포함되어 있습니다.

![가장 많이 방문한 상위 10개 링크 그래프의 스크린샷](assets/reporting_email_8.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭 수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 백분율]**: 게재와 상호 작용한 사용자의 비율입니다.

+++

### 시간 경과에 따른 클릭 분류 {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="시간 경과에 따른 클릭 분류"
>abstract="**시간 경과에 따른 클릭 분류** 그래프는 링크당 수신자 비헤이비어와 관련하여 사용 가능한 데이터를 보여 줍니다."


**[!UICONTROL 시간 경과에 따른 클릭 수 분석]** 그래프에는 링크당 받는 사람 동작에 사용할 수 있는 데이터가 포함되어 있습니다.

![시간 경과에 따른 클릭 수 분석 스크린샷](assets/reporting_email_9.png){zoomable="yes"}{align="center"}

## 사용자 활동 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="사용자 활동"
>abstract="**사용자 활동** 그래프에 열람 및 클릭의 분류가 차트 형식으로 표시됩니다. 데이터를 타기팅할 기간을 마지막 날, 시간 또는 30분 중에서 선택할 수 있습니다."

**[!UICONTROL 사용자 활동]** 보고서는 차트 형식으로 열린 횟수와 클릭수의 분류를 표시합니다. 데이터를 타기팅할 기간을 마지막 날, 시간 또는 30분 중에서 선택할 수 있습니다.

사용자 활동 보고서의 ![스크린샷](assets/reporting_email_10.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭 수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 열기]**: 메시지를 한 번 이상 연 이 도메인의 개별 대상 받는 사람 수입니다.

+++

## 추적 통계 {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="추적 통계"
>abstract="**추적 통계**: 그래프는 열람 및 클릭에 대한 통계를 제공합니다. 데이터 타기팅을 위한 특정 시간대를 선택할 수 있는 옵션이 있습니다."

**[!UICONTROL 추적 통계]**: 그래프는 열람 및 클릭에 대한 통계를 제공합니다. 데이터 타기팅을 위한 특정 시간대를 선택할 수 있는 옵션이 있습니다.

추적 통계 그래프의 ![스크린샷](assets/reporting_email_11.png){zoomable="yes"}{align="center"}

+++이메일 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 클릭 수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 열기]**: 메시지를 한 번 이상 연 이 도메인의 개별 대상 받는 사람 수입니다.

+++

## 열람수 분류 {#breakdown-opens}

### 디바이스별 열람수 분류 {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="디바이스별 분류"
>abstract="**디바이스별 분류** 보고서에 관련 기간 동안 디바이스별로 열람의 분류가 표시됩니다. 각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째에는 각 디바이스 유형별로 정확한 숫자와 백분율이 표시됩니다."

**장치별 분류** 보고서는 개인 컴퓨터, Android 장치, Apple 장치 또는 기타 장치의 기간별 열림 분류를 표시합니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째에는 각 디바이스 유형별로 정확한 숫자와 백분율이 표시됩니다.

![장치별 분석 보고서의 스크린샷](assets/reporting_email_13.png){zoomable="yes"}{align="center"}


### OS별 열람수 분류 {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="운영 체제별 분류"
>abstract="**OS별 분류** 보고서에는 관련 기간 동안 운영 체제별로 열람의 분류가 표시됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째에는 각 운영 체제별로 정확한 숫자와 백분율이 표시됩니다."

**OS별 분류** 보고서는 Windows 시스템, Android 시스템, iOS 시스템 또는 기타 운영 체제별 열기 분류를 표시합니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 화면에 컴퓨터 및 모바일 운영 체제의 열림에 대한 통계가 표시됩니다. 두 번째는 각 운영 체제에 대한 정확한 숫자와 백분율을 표시합니다.

![OS별 분류 보고서의 스크린샷](assets/reporting_email_13.1.png){zoomable="yes"}{align="center"}

### 브라우저별 열람수 분류 {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="브라우저별 분류"
>abstract="**브라우저별 분류**&#x200B;에는 관련 기간 동안 브라우저별로 열람의 분류가 표시됩니다. 첫 번째 차트에는 컴퓨터 및 모바일 디바이스에서의 열람과 관련된 통계가 표시됩니다. 두 번째에는 각 브라우저별로 정확한 숫자와 백분율이 표시됩니다."

**브라우저별 분류** 보고서는 Chrome, Safari, Internet Explorer 등의 브라우저별 열기 분류를 표시합니다.

각 범주별로 두 개의 차트가 사용됩니다. 첫 번째 화면에 컴퓨터 및 모바일 운영 체제의 열림에 대한 통계가 표시됩니다. 두 번째에는 각 브라우저별로 정확한 숫자와 백분율이 표시됩니다.

![브라우저별 열기 분석 스크린샷](assets/reporting_email_13.2.png){zoomable="yes"}{align="center"}


## 핫클릭 {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="핫클릭 보고서"
>abstract="**핫클릭** 보고서는 이메일 콘텐츠(HTML 및/또는 텍스트)와 각 링크의 링크 클릭 비율을 제공합니다. 개인 맞춤화 블록, 구독 취소 링크, 미러 페이지 링크 및 오퍼 링크는 총 누적 클릭 수 계산에 포함되지만 보고서에는 표시되지 않습니다."

이 보고서에는 메시지 콘텐츠(HTML 및/또는 텍스트)와 각 링크의 링크 클릭 비율이 표시됩니다. 개인 맞춤화 블록, 구독 취소 링크, 미러 페이지 링크 및 오퍼 링크는 총 누적 클릭 수 계산에 포함되지만 보고서에는 표시되지 않습니다.

![Hotclicks 보고서의 스크린샷](assets/reporting11.png){zoomable="yes"}