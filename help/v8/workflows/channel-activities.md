---
audience: end-user
title: 워크플로 채널 활동을 사용하여 작업
description: 채널 활동을 Adobe Campaign Web 워크플로에 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 26%

---

# 채널 활동 {#channel}

Adobe Campaign 웹을 사용하면 이메일, SMS 또는 푸시와 같은 여러 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. Adobe Campaign 워크플로우를 사용하면 채널 활동을 캔버스에 결합하여 고객 행동에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로우를 만들 수 있습니다.

예를 들어 이메일, SMS 및 푸시와 같은 다양한 채널에 걸친 일련의 메시지를 포함하는 환영 이메일 캠페인을 만들 수 있습니다. 또한 고객이 구매를 완료한 후 후속 이메일을 보내거나 SMS를 통해 고객에게 개인화된 생일 메시지를 보낼 수도 있습니다.

채널 활동을 사용하면 여러 접점에서 고객을 참여시키고 전환을 유도하는 종합적이고 개인화된 캠페인을 만들 수 있습니다.

채널 활동은 화면 왼쪽에 있는 팔레트의 채널 섹션에서 사용할 수 있습니다.

## 이메일 {#email}

설명, 수행할 수 있는 사용 사례 (활동 전후에 연결할 수 있는 일반적인 기타 활동)

활동 추가 및 구성 방법

워크플로 내에서 구성된 활동의 예


이메일 게재 활동을 사용하면 워크플로우에서 이메일 전송을 구성할 수 있습니다.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

이메일 수신자는 대상자 타겟팅 활동을 통해 동일한 워크플로우에서 활동의 업스트림으로 정의됩니다.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->