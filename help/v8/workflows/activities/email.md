---
audience: end-user
title: 이메일 워크플로우 활동 사용
description: 이메일 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 262f3bbbacb7bf22fe288bbf65b84f544eedec3c
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 31%

---


# 이메일, SMS, 푸시 {#channel}

Adobe Campaign 웹을 사용하면 이메일, SMS 또는 푸시와 같은 여러 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. 채널 활동을 캔버스에 결합하여 고객 행동에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로우를 만들 수 있습니다.

예를 들어 이메일, SMS 및 푸시 등 여러 채널에서 일련의 메시지를 포함하는 시작 이메일 캠페인을 만들 수 있습니다. 고객이 구매를 완료하면 후속 이메일을 보내거나, SMS를 통해 고객에게 맞춤형 생일 메시지를 보낼 수도 있습니다.

채널 활동을 사용하면 여러 접점에서 고객을 참여시키고 전환을 유도하는 종합적이고 개인화된 캠페인을 만들 수 있습니다.

을(를) 추가하는 단계는 다음과 같습니다 **채널** 워크플로우의 활동:

1. 을(를) 추가했는지 확인 **대상자 작성** 활동. 대상자는 게재의 주요 타겟인 메시지를 받는 수신자입니다. 캠페인 워크플로우의 컨텍스트에서 메시지를 보낼 때 메시지 대상자는 채널 활동에 정의되지 않고 **대상자 작성** 활동. [이 섹션](build-audience.md)을 참조하십시오.

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 게재 활동 선택: **[!UICONTROL 이메일]**, **[!UICONTROL SMS]**, **[!UICONTROL 푸시 알림(Android)]** 또는 **[!UICONTROL 푸시 알림(iOS)]**.

1. 선택 **템플릿**. 템플릿은 나중에 사용할 수 있도록 미리 구성된 게재 설정입니다. [자세히 알아보기](../../msg/delivery-template.md)

1. 클릭 **게재 만들기** 독립형 게재를 만드는 것과 동일한 방법으로 메시지를 정의합니다. 여기에서 게재 설정을 정의하고 콘텐츠를 예약 및 시뮬레이션할 수도 있습니다. [자세히 알아보기](../../msg/gs-messages.md)

1. 워크플로우로 돌아가서 **시작** 워크플로우를 시작합니다.

   기본적으로 게재 워크플로우를 시작하면 메시지를 즉시 보내지 않고 메시지 준비 단계가 트리거됩니다.

1. 클릭 **검토 및 보내기** 을 클릭하여 전송을 확인합니다.

1. 게재 대시보드에서 **보내기**.

## 예제


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

When linked to a scheduler, you can define recurring emails.-->

이메일 수신자는 대상자 타겟팅 활동을 통해 동일한 워크플로의 활동 업스트림으로 정의됩니다.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
