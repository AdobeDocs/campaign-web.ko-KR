---
audience: end-user
title: 게재 워크플로우 활동 사용
description: 게재 워크플로우 활동(이메일, 푸시, SMS)을 추가하는 방법을 알아봅니다
badge: label="알파"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 12%

---


# 이메일, SMS, 푸시 {#channel}

Adobe Campaign 웹을 사용하면 이메일, SMS 및 푸시 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. 채널 활동을 워크플로우 캔버스에 결합하여 고객 행동 및 데이터에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로우를 만들 수 있습니다.

예를 들어 이메일, SMS 및 푸시 등 여러 채널에서 일련의 메시지를 포함하는 시작 이메일 캠페인을 만들 수 있습니다. 고객이 구매를 완료한 후 후속 이메일을 보내거나 SMS를 통해 고객에게 개인화된 생일 메시지를 보낼 수도 있습니다.

채널 활동을 사용하면 여러 접점에서 고객을 참여시키고 전환을 유도하는 종합적이고 개인화된 캠페인을 만들 수 있습니다.

을(를) 추가하는 단계는 다음과 같습니다 **채널** 워크플로우의 활동:

1. 을(를) 추가했는지 확인 **대상자 작성** 활동. 대상자는 게재의 주요 타겟인 메시지를 받는 수신자입니다. 캠페인 워크플로우의 컨텍스트에서 메시지를 보낼 때 메시지 대상자는 채널 활동에 정의되지 않고 **대상자 작성** 활동. [이 섹션](build-audience.md)을 참조하십시오.

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 게재 활동 선택: **[!UICONTROL 이메일]**, **[!UICONTROL SMS]**, **[!UICONTROL 푸시 알림(Android)]** 또는 **[!UICONTROL 푸시 알림(iOS)]**.

1. 게재 선택 **템플릿**. 템플릿은 채널별로 사전 구성된 게재 설정입니다. 기본 제공 템플릿은 각 채널에 대해 사용할 수 있으며 기본적으로 미리 채워져 있습니다. [자세히 알아보기](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   채널 활동 구성 왼쪽 창에서 다른 템플릿을 선택할 수 있습니다. 이전에 선택한 대상자가 채널과 호환되지 않는 경우 템플릿을 선택할 수 없습니다. 이 문제를 해결하려면 **대상자 작성** 활동을 통해 올바른 대상 매핑이 있는 대상을 선택할 수 있습니다. 다음에서 대상 매핑에 대해 자세히 알아보기: [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

1. 클릭 **게재 만들기**. 독립형 게재를 만드는 것과 동일한 방법으로 메시지 설정 및 콘텐츠를 정의합니다. 콘텐츠를 예약하고 시뮬레이션할 수도 있습니다. [자세히 알아보기](../../msg/gs-messages.md)

1. 워크플로우로 돌아가서 변경 사항을 저장합니다.

1. 클릭 **시작** 워크플로우를 시작합니다.

   기본적으로 워크플로우를 시작하면 메시지를 즉시 보내지 않고 메시지 준비 단계가 트리거됩니다.

1. 게재 활동을 열어 (으)로부터의 전송을 확인합니다. **검토 및 보내기** 단추를 클릭합니다.

1. 게재 대시보드에서 **보내기**.

## 예제

다음은 세그먼테이션 및 두 개의 게재가 있는 크로스 채널 워크플로우 예입니다. 이 워크플로우는 Paris에 거주하며 커피 머신에 관심이 있는 모든 고객을 대상으로 합니다. 이 모집단 중 일반 고객에게 이메일이 전송되고 VIP 클라이언트에게 SMS가 전송됩니다.

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
