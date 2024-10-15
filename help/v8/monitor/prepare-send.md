---
audience: end-user
title: 이메일 준비 및 전송
description: Campaign 웹 사용자 인터페이스를 사용하여 이메일을 준비하고 보내는 방법 알아보기
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: c3148c9593aa4d323097135601616b9c43bae378
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 38%

---


# 이메일 준비 및 전송 {#prepare-send}

## 전송 준비 {#prepare}

[콘텐츠](../email/edit-content.md), [대상자](../audience/add-audience.md) 및 [일정](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule)을(를) 정의하면 전자 메일 게재를 준비할 준비가 된 것입니다.

게재를 준비하는 동안 대상 모집단을 계산하고 대상에 포함된 각 프로필에 대해 생성된 메시지 콘텐츠를 계산합니다. 준비가 완료되면 메시지를 즉시 또는 예약된 날짜와 시간에 보낼 수 있습니다.

게재를 준비하는 동안 사용되는 유효성 검사 규칙은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html){target="_blank"}에 설명되어 있습니다.

전송을 준비하는 주요 단계는 아래에 나와 있습니다.

1. 게재 대시보드에서 **[!UICONTROL 검토 및 보내기]**&#x200B;를 클릭합니다.

   ![](assets/email-review-and-send.png){zoomable="yes"}


1. 오른쪽 상단의 **[!UICONTROL 준비]** 단추를 클릭하여 확인합니다.

   ![](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >게재를 예약하고 **[!UICONTROL 전송 전 확인 사용]** 옵션을 사용하지 않도록 설정한 경우, 준비 및 전송 단계는 **[!UICONTROL 준비 및 보내기]** 단추 아래에 함께 그룹화됩니다. [예약에 대해 자세히 알아보기](../msg/gs-deliveries.md#gs-schedule)

1. 준비 진행률이 표시됩니다. 대상 모집단의 크기에 따라 약간의 시간이 소요될 수 있습니다.

   언제든지 **[!UICONTROL 준비 중지]** 단추를 사용하여 준비를 중지할 수 있습니다.

   ![](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >준비 단계 중에는 메시지가 전송되지 않습니다. 따라서 영향을 미칠 위험 없이 준비를 시작하거나 중지할 수 있습니다.

1. 준비가 끝나면 KPI를 확인합니다. 전송할 메시지 수가 예상과 일치하지 않으면 대상자를 수정하고 준비를 다시 시작하십시오.

   ![](assets/email-preparation-complete.png){zoomable="yes"}

   표시되는 다양한 KPI는 다음과 같습니다.

   * **[!UICONTROL 타깃팅]**: 타깃팅된 수신자 수.
   * **[!UICONTROL 게재할]**: 전송할 메시지 수.
   * **[!UICONTROL 제외하기]**: [유형화 규칙에 의해 제외된 메시지 수](../advanced-settings/delivery-settings.md#typology).

1. **[!UICONTROL 로그]** 버튼을 클릭하고 오류가 없는지 확인하십시오. 마지막 로그 메시지에는 오류 메시지와 오류 수가 표시됩니다. [자세히 알아보기](delivery-logs.md)

   ![](assets/email-prepare-logs.png){zoomable="yes"}

1. 준비 과정에서 게재 전송을 방해하는 심각한 오류가 감지되면 게재 대시보드에 준비 상태가 실패로 표시됩니다.

   ![](assets/email-prepare-error.png){zoomable="yes"}

1. 준비 후 게재를 변경하는 경우 이러한 변경 사항을 고려하기 위해 준비를 다시 시작해야 합니다.

오류 없이 준비가 완료되면 메시지를 보낼 준비가 되었습니다.

## 메시지 전송 {#send}


[준비](#prepare)가 완료되면 이제 전자 메일을 보낼 수 있습니다.

메시지가 예약된 경우 정의된 날짜 및 시간에 전송됩니다. [자세히 알아보기](../msg/gs-deliveries.md#gs-schedule)

### 즉시 전송 {#send-immediately}

이메일을 즉시 보내려면 아래 단계를 따르십시오.

1. 게재 대시보드에서 오른쪽 상단의 **[!UICONTROL 보내기]** 단추를 클릭합니다.

   ![](assets/email-send.png){zoomable="yes"}

1. 메시지를 기본 타겟에게 즉시 보내려면 이 작업을 확인하십시오.

1. 전송 진행률이 표시됩니다.

### 전송 예약 {#schedule-the-send}

이메일을 나중 날짜 및 시간에 전송하도록 예약한 경우 아래 단계를 따르십시오.

1. **[!UICONTROL 검토 및 보내기]** 단추를 누르기 전에 전자 메일에 대한 일정을 정의했는지 확인하세요. [자세히 알아보기](../msg/gs-deliveries.md#gs-schedule)

1. 게재 대시보드에서 오른쪽 상단 모서리에 있는 **[!UICONTROL 일정대로 보내기]** 단추를 클릭합니다.

   ![](assets/email-send-as-scheduled.png){zoomable="yes"}

1. **[!UICONTROL 전송 확인]**&#x200B;을 클릭합니다. 게재는 예약된 날짜에 주요 타겟에게 전송됩니다.

   >[!NOTE]
   >
   >**[!UICONTROL 전송 전에 확인 사용]** 옵션을 사용하지 않도록 설정한 경우 준비 및 전송 단계는 **[!UICONTROL 준비 및 보내기]** 단추 아래에 함께 그룹화됩니다. [예약에 대해 자세히 알아보기](../msg/gs-deliveries.md#gs-schedule)

## 전송 일시 중지 또는 중지 {#pause-stop-sending}

게재 예약 여부에 관계없이 <!--TBC--> 전송 프로세스 중 언제든지 두 가지 작업을 수행할 수 있습니다.

* 메시지 전송을 중단하려면 **[!UICONTROL 전송 일시 중지]**&#x200B;를 클릭하세요. 언제든지 전송을 재개할 수 있습니다.

* 즉시 전송을 중단하려면 **[!UICONTROL 전송 중지]**&#x200B;를 클릭하십시오. 일단 중지되면 준비나 전송을 재개할 수 없습니다.

![](assets/email-send-pause-or-stop.png){zoomable="yes"}

## KPI 확인 {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="게재됨"
>abstract="정상적으로 게재된 메시지 수. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 전송된 총 메시지 수를 기준으로 합니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/reports/kpis" text="KPI 이해"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="열람수"
>abstract="열린 메시지 수입니다. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 열람 수의 비율입니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/reports/kpis" text="KPI 이해"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="클릭수"
>abstract="이메일에서 최소 한 번 클릭한 수신자 수입니다. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 클릭 수의 비율입니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/reports/kpis" text="KPI 이해"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="전송된 지표"
>abstract="게재 분석 시 처리된 총 메시지 수입니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/reports/kpis" text="KPI 이해"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="오류 지표"
>abstract="총 전송된 총 메시지 수와 관련하여 게재 및 자동 반환 처리 시 누적된 오류의 총계입니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/reports/kpis" text="KPI 이해"


전송이 완료되면 표시된 KPI를 확인할 수 있습니다.

![](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL 전송됨]**: 배달된 메시지 수 표시되는 비율은 게재할 총 메시지 수를 기반으로 합니다.

* **[!UICONTROL 게재됨]**: 정상적으로 게재된 메시지 수입니다. 표시되는 백분율은 전송된 총 메시지 수를 기준으로 합니다.

* **[!UICONTROL 열람 수]**: 열린 메시지 수입니다. 표시되는 백분율은 게재된 메시지 수와 비교하여 고유 열람 수입니다.

* **[!UICONTROL 클릭 수]**: 전자 메일에서 최소 한 번 이상 클릭한 수신자 수입니다. 표시되는 백분율은 게재된 메시지 수와 비교한 고유 클릭 수입니다.

* **[!UICONTROL 오류]**: 오류 상태의 전자 메일 수입니다. 표시되는 백분율은 전송된 총 메시지 수를 기준으로 합니다.

>[!NOTE]
>
>모든 지표는 게재 시작 후 5분마다 업데이트됩니다. 게재 준비 지표는 실시간으로 표시됩니다.

[이 페이지](../reporting/kpis.md)에서 KPI에 대해 자세히 알아보세요.

로그를 확인할 수도 있습니다. [자세히 알아보기](delivery-logs.md)