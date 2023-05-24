---
audience: end-user
title: 이메일 준비 및 전송
description: Campaign Web UI를 사용하여 이메일을 준비하고 전송하는 방법 알아보기
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 100%

---


# 이메일 준비 및 전송 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="이메일 준비 및 전송"
>abstract="이메일을 준비하는 방법과 KPI 전송에 대해 자세히 알아봅니다."

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 전송 준비{#prepare}

콘텐츠, 대상자 및 일정을 정의한 다음에는 메시지를 준비할 수 있습니다. 준비하는 동안 대상 모집단이 계산되며 대상에 포함된 각 프로필에 대해 메시지 콘텐츠가 생성됩니다. 준비가 완료되면 즉시 또는 예정된 날짜 및 시간에 메시지를 전송할 수 있습니다. 분석 중에 사용되는 유효성 검사 규칙은 [Campaign Classic v7 설명서](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies)에 기술되어 있습니다{target="_blank"}.

아래의 단계를 수행하십시오.

1. 게재 대시보드에서 오른쪽 상단에 있는 **준비** 버튼을 클릭하고 확인합니다.

   ![](assets/prepare.png)

   준비 진행률이 표시됩니다. 대상 모집단의 크기에 따라 약간의 시간이 소요될 수 있습니다.

   >[!NOTE]
   >
   >**준비 중지** 버튼을 사용하여 언제든지 준비를 중지할 수 있습니다. 준비 단계 중에는 메시지가 전송되지 않습니다. 따라서 영향을 미칠 위험 없이 준비를 시작하거나 중지할 수 있습니다.

1. 준비가 끝나면 KPI를 확인합니다. 전송할 메시지 수가 예상과 일치하지 않으면 대상자를 수정하고 준비를 다시 시작하십시오.

   ![](assets/prepare2.png)

   표시되는 다양한 KPI는 다음과 같습니다.

   * **목표**: 대상 수신자 수
   * **게재 예정**: 전송할 메시지 수
   * **제외됨**: 유형화 규칙으로 제외된 메시지 수

1. **로그** 버튼을 클릭하고 오류가 없는지 확인하십시오. 마지막 로그 메시지에는 오류 메시지와 오류 수가 표시됩니다. 자세한 내용은 이 [섹션](delivery-logs.md)을 참조하십시오.

   ![](assets/prepare-logs.png)

준비 과정에서 게재 전송을 방해하는 심각한 오류가 감지되면 게재 대시보드에 준비 상태가 실패로 표시됩니다.

![](assets/prepare-error.png)

준비 후 게재를 변경해야 하는 경우 해당 변경 내용을 고려하려면 준비를 다시 시작해야 합니다.

오류 없이 준비가 완료되면 메시지를 전송할 수 있습니다. 자세한 내용은 이 [섹션](#send)을 참조하십시오.

## 메시지 전송{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="게재됨"
>abstract="정상적으로 게재된 메시지 수. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 전송된 총 메시지 수를 기준으로 합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="열람 수"
>abstract="열린 메시지 수입니다. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 열람 수의 비율입니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="클릭 수"
>abstract="이메일에서 최소 한 번 클릭한 수신자 수입니다. 이 표시기는 5분마다 업데이트됩니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 클릭 수의 비율입니다."


준비가 완료되었다면 이제 메시지를 전송할 수 있습니다. 이 단계는 즉시 전송된 메시지에만 필요합니다. 메시지가 예약된 경우에는 정의된 날짜에 전송됩니다.

다음 단계를 수행하십시오.

1. 게재 대시보드에서 오른쪽 상단에 있는 **전송** 버튼을 클릭하고 확인합니다.

   ![](assets/send.png)

1. 전송 진행률이 표시됩니다. 표시되는 KPI를 확인합니다. 로그를 확인할 수도 있습니다. 자세한 내용은 이 [섹션](delivery-logs.md)을 참조하십시오.

   ![](assets/send2.png)

   표시되는 다양한 KPI는 다음과 같습니다.

   * **게재됨**: 정상적으로 게재된 메시지 수입니다. 표시되는 백분율은 전송된 총 메시지 수를 기준으로 합니다.
   * **열람 수**: 열린 메시지 수입니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 열람 수의 비율입니다.
   * **클릭 수**: 이메일에서 최소 한 번 클릭한 수신자 수입니다. 표시되는 백분율은 게재된 메시지 수와 비교되는 고유 클릭 수의 비율입니다.

   >[!NOTE]
   >
   >모든 지표는 게재 시작 후 5분마다 업데이트됩니다. 게재 준비 지표는 실시간으로 업데이트됩니다.

   언제든지 전송을 일시 중지한 다음 다시 시작할 수 있습니다. 전송 도중 게재를 중지하면 다시 시작할 수 없습니다.
