---
audience: end-user
title: SMS 게재 보고서
description: sms 게재 보고서에 액세스하고 사용하는 방법을 알아봅니다
exl-id: 153d3a85-0d39-42db-9906-1e7f2d1d5bae
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 32%

---

# SMS 게재 보고서 {#sms-report}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_sms"
>title="보고 전송"
>abstract="보고서 내의 **전송** 탭은 방문자와 게재 간의 상호 작용 및 방문자가 경험할 수 있는 잠재적인 오류에 대한 심층적인 인사이트를 제공합니다."

**SMS 게재 개요**&#x200B;에서는 SMS 게재의 자세한 요약을 제공하여 광범위한 통찰력과 특정 데이터를 제공합니다. 여기에는 게재의 성능, 효율성 및 결과에 대한 포괄적인 정보가 포함됩니다.

## 게재 요약 {#delivery-summary}

### 게재 개요 {#sms-delivery-overview}

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="SMS 게재 개요"
>abstract="**SMS 게재 요약**&#x200B;은 SMS 게재에 대한 포괄적인 개요를 제공하여 광범위한 인사이트와 특정 데이터를 얻을 수 있습니다. 성과, 효율성 및 게재 결과에 대해 포괄적인 정보를 제공합니다."

**[!UICONTROL 게재 개요]** 보고서는 성공 및 오류율과 방문자의 SMS 메시지 참여 방법에 대한 자세한 정보를 제공하는 주요 성과 지표(KPI)를 제공합니다.

![설명: 이 그림에서는 성공률, 오류율 및 방문자 참여와 같은 KPI가 포함된 게재 개요 보고서를 보여 줍니다.](assets/reporting_sms_3.png){zoomable="yes"}

+++SMS 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 보낸 총]**: 게재를 준비하는 동안 처리된 총 메시지 수 및 비율입니다.

* **[!UICONTROL 성공]**: 보낸 총 메시지 수와 관련하여 성공적으로 보낸 메시지 수 및 비율입니다.

* **[!UICONTROL 클릭스루 비율]**: SMS 게재에 포함된 링크와 상호 작용한 사용자의 비율 및 수입니다.

* **[!UICONTROL 오류]**: 게재 중에 발생한 오류의 비율과 총 개수로 프로필로 전송되지 않습니다.

+++

### 대상 모집단 {#sms-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_targeted_population"
>title="SMS 대상 모집단"
>abstract="**대상 모집단** 그래프와 테이블은 SMS 대상자(게재할 메시지 및 제외)와 관련된 데이터가 표시됩니다."

대상자와 관련된 **대상 모집단** 그래프 및 표에 데이터가 표시됩니다. 지표는 아래에 자세히 설명되어 있습니다.

![설명: 이 그림에서는 배달할 메시지 및 제외 메시지와 같은 지표를 포함하는 타깃팅된 모집단 그래프와 표를 보여 줍니다.](assets/reporting_sms_4.png){zoomable="yes"}

+++SMS 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 게재]**: 게재를 준비하는 동안 처리된 총 메시지 수 및 비율입니다.

* **[!UICONTROL 제외]**: 분석에서 제외된 프로필 수 및 비율입니다.
+++

### 전체 통계 {#sms-delivery-overall}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_overall_stats"
>title="SMS 전체 통계"
>abstract="**전체 통계** 보고서는 보낸 SMS에 대한 데이터(성공, 오류 및 격리)를 제공합니다."

**전체 통계** 보고서는 보낸 SMS 메시지에 대한 데이터를 제공합니다. 지표는 아래에 자세히 설명되어 있습니다.

![설명: 이 그림에서는 성공률, 오류 및 격리 등의 지표가 포함된 전체 통계 보고서를 보여 줍니다.](assets/reporting_sms_5.png){zoomable="yes"}

+++SMS 게재 보고서 지표에 대해 자세히 알아보십시오.

* **[!UICONTROL 성공]**: 성공적으로 처리된 메시지 수 및 비율입니다.

* **[!UICONTROL 오류]**: 게재 중에 발생한 총 오류 수 및 백분율로, 특정 프로필로 메시지를 보낼 수 없습니다.

* **[!UICONTROL 새 격리]**: 제외되어 격리에 추가된 프로필의 수와 백분율 비율입니다.
+++

### 제외 {#sms-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_exclusions"
>title="SMS 제외"
>abstract="**제외** 그래프와 테이블에 대상 프로필에서 제외된 사용자 프로필이 메시지를 받지 못하는 다양한 이유가 표시됩니다."

**[!UICONTROL 제외]** 그래프 및 표에는 대상 프로필에서 제외된 사용자 프로필이 메시지를 받지 못하는 이유가 표시됩니다. 제외 규칙은 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){_blank}에 자세히 설명되어 있습니다.

![설명: 이 그림에서는 사용자 프로필을 메시지 수신에서 제외하는 이유를 자세히 설명하는 제외 그래프와 표를 보여 줍니다.](assets/reporting_sms_6.png){zoomable="yes"}

## 게재 처리량 {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_sms"
>title="SMS 게재 처리량"
>abstract="**게재 처리량** 보고서는 지정된 기간 내 게재 처리량에 대한 자세한 정보를 제공합니다. 메시지 게재 속도를 측정하는 데 사용되는 주요 지표는 시간당 전송된 메시지 수입니다."

이 보고서는 지정된 기간 내의 게재 처리량에 대한 자세한 정보를 제공합니다. 메시지 게재 속도를 측정하는 데 사용되는 주요 지표는 시간당 전송된 메시지 수입니다.

![설명: 이 그림에서는 지정된 기간 내에 시간당 보낸 메시지 수와 같은 지표를 포함하는 게재 처리량 보고서를 보여 줍니다.](assets/reporting_sms_2.png){zoomable="yes"}