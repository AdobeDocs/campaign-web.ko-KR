---
audience: end-user
title: SMS 채널에 대한 캠페인 보고서
description: SMS 채널에 대한 캠페인 보고서 이해
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 20%

---

# SMS 채널에 대한 캠페인 보고서 {#campaign-reports-sms-channel}

각 캠페인 보고서는 캠페인의 성공 및 오류를 자세히 설명하는 다양한 위젯으로 나뉩니다. SMS 채널의 경우 보고서 및 지표가 아래에 자세히 설명되어 있습니다. 에서 캠페인 보고서에 액세스하는 방법 알아보기 [이 페이지](campaign-reports.md).

## 게재 요약 {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="게재 개요"
>abstract="**게재 개요** 보고서는 방문자가 SMS 게재에 참여하는 방식에 대한 자세한 정보를 포함하는 주요 성과 지표(KPI)를 제공합니다."


다음 **[!UICONTROL 게재 개요]** 보고서는 방문자의 SMS 게재 방법에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_sms_1.png){zoomable=&quot;yes&quot;}

+++SMS 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 총 전송됨]**: 게재를 준비하는 동안 처리된 총 메시지 수입니다.

* **[!UICONTROL 전달됨]**: 성공적으로 전송된 메시지 수와 총 전송된 메시지 수

* **[!UICONTROL 오류]**: 총 보낸 메시지 수와 관련하여 게재 및 자동 반환 처리 중에 누적된 총 오류.

* **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

+++


### 초기 타깃 대상자 통계 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="초기 타깃 대상자 통계"
>abstract="**초기 타깃 대상자 통계** 테이블에는 수신자와 관련된 데이터가 표시됩니다."

다음 **[!UICONTROL 초기 타겟 대상 통계]** 테이블에는 수신자와 관련된 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.


![](assets/campaign_report_sms_2.png){zoomable=&quot;yes&quot;}

+++SMS 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 초기 대상자]**: 타겟팅된 총 수신자 수.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 규칙에 의해 거부됨]**&#x200B;차단 목록에 추가하다 : 분석 중에 무시된 총 주소 수: 격리된 주소, 격리된 주소 수 등 규칙 적용 시

+++


### 실행 통계 {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="실행 통계"
>abstract="**실행 통계** 테이블에는 전달할 메시지, 성공, 오류, 새 격리 등 게재 성공에 대한 자세한 내용이 나와 있습니다."


다음 **[!UICONTROL 실행 통계]** 게재의 성공 여부를 표로 자세히 설명합니다. 지표는 아래에 자세히 설명되어 있습니다.


![](assets/campaign_report_sms_3.png){zoomable=&quot;yes&quot;}

+++SMS 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재할 메시지]**: 게재를 준비한 후 게재할 총 메시지 수

* **[!UICONTROL 성공]**: 배달할 메시지 수와 관련하여 성공적으로 처리된 메시지 수입니다.

* **[!UICONTROL 오류]**: 게재할 메시지 수와 관련하여 게재 및 자동 반동 처리 중에 누적된 총 오류 수입니다.

* **[!UICONTROL 새로운 격리]**: 배달할 메시지 수와 관련하여 배달 실패 후 격리된 총 주소 수(사용자 알 수 없음, 잘못된 도메인)입니다.

  SMS 오류 유형은 [Adobe Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### 생성된 클릭스트림 {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="생성된 클릭스트림"
>abstract="**생성된 클릭스트림** 테이블에는 수신자가 게재된 내용과 상호 작용한 방식과 관련하여 이용 가능한 데이터가 표시됩니다."

다음 **[!UICONTROL 생성된 클릭 스트림]** 테이블에는 수신자와 게재의 상호 작용 방식에 따른 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![](assets/campaign_report_sms_4.png){zoomable=&quot;yes&quot;}

+++SMS 캠페인 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 고유 클릭 수]**: 한 번 이상 게재를 클릭한 총 고유 수신자 수입니다.

* **[!UICONTROL 클릭수]**: 게재의 총 링크 클릭 수입니다.

* **[!UICONTROL 반응성]**: 게재를 연 예상 대상 수신자 수와 관련하여 게재에서 클릭한 대상 수신자 수의 비율입니다.

+++
