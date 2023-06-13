---
audience: end-user
title: 푸시 알림 워크플로우 활동 사용
description: 푸시 알림 워크플로우 활동을 사용하는 방법 알아보기
badge: label="알파"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 4%

---


# 푸시 알림 {#push-activity}

다음 **푸시 알림** 게재 활동을 사용하면 워크플로우에서 푸시 알림 전송을 구성할 수 있습니다.

>[!BEGINTABS]

>[!TAB 푸시 알림 (Android)]

1. 새 워크플로우를 만들고 구성한 후 대상 작성 활동을 추가하여 기존 대상을 선택하거나 규칙 빌더를 사용하여 쿼리를 정의합니다.

1. 푸시 알림(Android) 채널 활동을 워크플로우에 추가합니다.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. 활동을 선택합니다. 게재 메뉴에서 이 게재에 사용할 템플릿을 선택합니다. 템플릿에 대해 자세히 알아보기

1. 푸시 알림 게재를 구성하려면 게재 만들기 를 클릭합니다. 푸시 알림(Android) 전달에 대한 자세한 내용은 이 페이지 를 참조하십시오.

1. 게재를 보낼 준비가 되면 워크플로우로 다시 이동하고 시작 을 클릭하여 워크플로우를 시작합니다.

1. 기본적으로 게재 워크플로우를 시작하면 메시지를 즉시 보내지 않고 메시지 준비 단계가 트리거됩니다.

   푸시 알림(Android) 채널 활동의 고급 메뉴에서 검토 및 보내기 를 클릭하여 전송을 확인합니다.

1. 푸시 알림 게재 대시보드에서 전송을 클릭합니다.

>[!TAB 푸시 알림 (iOS)]

1. 새 워크플로우를 만들고 구성한 후 대상 작성 활동을 추가하여 기존 대상을 선택하거나 규칙 빌더를 사용하여 쿼리를 정의합니다.

1. 푸시 알림(iOS) 채널 활동을 워크플로우에 추가합니다.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. 활동을 선택합니다. 게재 메뉴에서 이 게재에 사용할 템플릿을 선택합니다. 템플릿에 대해 자세히 알아보기

1. 푸시 알림 게재를 구성하려면 게재 만들기 를 클릭합니다. 푸시 알림(iOS) 전달에 대한 자세한 내용은 이 페이지 를 참조하십시오.

1. 게재를 보낼 준비가 되면 워크플로우로 다시 이동하고 시작 을 클릭하여 워크플로우를 시작합니다.

1. 기본적으로 게재 워크플로우를 시작하면 메시지를 즉시 보내지 않고 메시지 준비 단계가 트리거됩니다.

   푸시 알림(iOS) 채널 활동의 고급 메뉴에서 검토 및 보내기 를 클릭하여 전송을 확인합니다.

1. 푸시 알림 게재 대시보드에서 전송을 클릭합니다.

>[!ENDTABS]