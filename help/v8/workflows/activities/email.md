---
audience: end-user
title: 이메일 워크플로우 활동 사용
description: 이메일 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 6af0b460a3c81f063a855b2fabba221b43e4ebb9
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 10%

---


# 이메일 {#email}

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow

-->


이메일 게재 활동을 사용하면 워크플로우에서 이메일 전송을 구성할 수 있습니다.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

이메일 수신자는 대상자 타겟팅 활동을 통해 동일한 워크플로우에서 활동의 업스트림으로 정의됩니다.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
