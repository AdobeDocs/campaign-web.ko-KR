---
audience: end-user
title: SMS 워크플로우 활동 사용
description: SMS 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# SMS {#sms}

다음 **SMS** 활동은 워크플로우 내에서 SMS 메시지를 전송하는 기능을 제공합니다. 이를 통해 동일한 워크플로우 내에서 결정된 특정 타겟으로 SMS 전송을 자동화할 수 있습니다.

SMS 수신자를 정의하려면 대상자 작성 활동을 사용하여 워크플로우에서 SMS 게재 활동 전에 설정할 수 있습니다. 자세히 알아보기.

1. 새 워크플로우를 만들고 구성한 후 대상 작성 활동을 추가하여 기존 대상을 선택하거나 규칙 빌더를 사용하여 쿼리를 정의합니다.

1. SMS 채널 활동을 워크플로우에 추가합니다.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. 활동을 선택합니다. 게재 메뉴에서 이 게재에 사용할 템플릿을 선택합니다. 템플릿에 대해 자세히 알아보기

1. SMS 게재를 구성하려면 게재 만들기 를 클릭합니다. SMS 게재에 대한 자세한 내용은 이 페이지 를 참조하십시오.

1. 게재를 보낼 준비가 되면 워크플로우로 다시 이동하고 시작 을 클릭하여 워크플로우를 시작합니다.

1. 기본적으로 게재 워크플로우를 시작하면 메시지를 즉시 보내지 않고 메시지 준비 단계가 트리거됩니다.

   SMS 활동의 고급 메뉴에서 검토 및 보내기 를 클릭하여 전송을 확인합니다.

1. SMS 게재 대시보드에서 보내기를 클릭합니다.
