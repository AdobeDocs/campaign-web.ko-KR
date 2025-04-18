---
audience: end-user
title: 게재 전송 예약
description: 게재 예약 방법 알아보기
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 6%

---

# 게재 전송 예약 {#schedule-sending}

게재 전송을 예약할 수 있습니다. 단계는 독립 실행형(일회성) 게재인지 또는 캠페인 워크플로우의 컨텍스트에서 작업 중인지 여부에 따라 다릅니다.

## 독립형 게재

독립형 게재의 경우 게재의 날짜 및 시간을 직접 예약합니다. 각 게재 유형에 대한 아래 예(이메일, SMS 및 푸시 알림)를 참조하십시오.

### 이메일 {#schedule-email-standalone}

이메일 게재 전송을 예약하려면 다음 단계를 따르십시오.

1. 게재 속성의 **[!UICONTROL 예약]** 섹션에서 **[!UICONTROL 예약 사용]** 토글을 활성화합니다.

1. 원하는 전송 날짜와 시간을 설정하고 **[!UICONTROL 검토 및 보내기]** 단추를 클릭합니다.

   ![일정 활성화 및 날짜 및 시간 설정](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>기본적으로 **[!UICONTROL 전송 전에 확인 활성화]** 옵션이 활성화되어 있습니다. 이 옵션을 활성화하면 게재가 예약된 날짜 및 시간에 전송되기 전에 전송을 확인해야 합니다. 예약된 날짜 및 시간에 자동으로 게재를 전송해야 하는 경우 이 옵션을 비활성화합니다.
>

1. 일정이 올바른지 확인하고 **[!UICONTROL 준비]** 단추를 클릭합니다.

![일정 확인 및 게재 준비](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. 준비가 완료되면 메시지를 보낼 준비가 되었습니다. 총 대상 모집단, 게재할 메시지 수 및 제외된 수신자 수를 포함한 게재의 주요 지표가 표시됩니다. **[!UICONTROL 일정대로 보내기]** 단추를 클릭하여 예약된 날짜와 시간에 게재가 기본 대상으로 전송되는지 확인합니다.

![일정에 따라 보내기 확인](assets/schedule-email-standalone-send.png){zoomable="yes"}

### SMS

특정 날짜 및 시간에 SMS 게재를 예약하려면 이메일 게재와 동일한 단계를 수행합니다. [위의 내용을 참조하십시오](#schedule-email-standalone).

![SMS 게재 예약](assets/schedule-sms-standalone.png){zoomable="yes"}

일정이 적용되었는지 확인할 수도 있습니다.

![SMS 일정 확인](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### 푸시 알림

특정 날짜 및 시간에 대해 독립 실행형 푸시 게재를 예약하려면 이메일 게재와 동일한 단계를 따릅니다. [위의 내용을 참조하십시오](#schedule-email-standalone).

![푸시 알림 배달 예약](assets/schedule-push-standalone.png){zoomable="yes"}

일정이 적용되었는지 확인할 수도 있습니다.

![푸시 알림 일정 확인](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### 캠페인의 독립 실행형 게재

워크플로우를 사용하지 않고 캠페인 내에서 독립형 게재를 만들 수 있습니다. 위에서 설명한 대로 이 게재의 날짜 및 시간 일정을 설정합니다. 캠페인에는 시작일과 종료일을 포함한 자체 일정이 있을 수 있습니다. 이 일정은 게재 일정에 영향을 주지 않습니다.

![캠페인의 독립 실행형 게재](assets/schedule-delivery-standalone.png){zoomable="yes"}

## 캠페인 워크플로우에서 게재 예약

캠페인 워크플로우의 맥락에서 가장 좋은 방법은 **[!UICONTROL 스케줄러]** 활동을 사용하여 게재를 보내는 것과 같은 워크플로우를 시작하는 날짜와 시간을 적용하는 것입니다. [스케줄러에 대해 자세히 알아보기](../workflows/activities/scheduler.md).

![캠페인 워크플로우에서 게재 예약](assets/schedule-workflow.png){zoomable="yes"}

**[!UICONTROL 스케줄러]** 활동에서 날짜 및 시간을 구성하십시오.

![스케줄러 활동 구성](assets/schedule-workflow-scheduler.png){zoomable="yes"}

>[!NOTE]
>
>**[!UICONTROL 스케줄러]** 활동을 사용하여 워크플로우에서 게재 전송을 예약하는 경우 **[!UICONTROL 게재]** 활동 설정에서 **[!UICONTROL 예약 사용]** 토글을 활성화하지 마십시오. 게재가 자동으로 전송됩니다.
>

**[!UICONTROL 게재]** 활동 설정에서 **[!UICONTROL 예약 사용]** 토글을 활성화하고 날짜와 시간을 설정하면 이 날짜 및 시간에 게재가 전송될 때까지 대기합니다. 즉, 워크플로우 시작 날짜와 전송 날짜 사이에 지연이 있을 경우 대상자가 최신 상태가 아닐 수 있습니다.