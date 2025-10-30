---
audience: end-user
title: 게재 알림
description: 게재 경고 작업 방법을 알아봅니다.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 037b04475370b1a34ecec31ef2a774866278ce65
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 2%

---

# 게재 알림 시작하기 {#gs-delivery-alerting}

게재 경고는 사용자 그룹이 게재 실행에 대한 정보가 포함된 이메일 알림을 자동으로 수신할 수 있는 경고 관리 시스템입니다. 수신자는 Adobe Campaign에서 처리하는 진행 중인 게재를 모니터링하고 문제가 발생하는 경우 적절한 조치를 취합니다.

알림은 Adobe Campaign 웹 사용자 인터페이스를 통해 정의된 특정 경고 기준에 따라 사용자 정의됩니다.

게재 실패 관리에 대한 자세한 내용은 [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}를 참조하세요.

## 이메일 알림 콘텐츠 {#content}

이메일 알림에는 다음 섹션이 포함됩니다.

* **요약**: 정의된 기준을 충족하는 게재 수를 각 기준에 대한 레이블과 색상으로 표시합니다.
* **세부 정보**: 대시보드에 대해 정의된 모든 게재 기준과 각 기준에 해당하는 게재를 나열합니다.

![설명: 이 스크린샷은 요약 및 세부 정보 섹션을 포함하여 전자 메일 알림 레이아웃을 보여 줍니다.](assets/alerting-email.png)

## 게재 경고 설정 {#set-up}

이러한 경고를 설정하려면 Campaign 웹 사용자 인터페이스를 사용하여 다음을 만들고 관리할 수 있습니다.

* **게재 경고 대시보드**: 수신자를 지정하고 대시보드에 포함할 경고 기준을 설정하며 전송된 경고 기록에 액세스합니다. [대시보드를 사용하여 작업하는 방법을 알아봅니다](../msg/delivery-alerting-dashboards.md).
* **게재 경고 기준**: Campaign 웹 사용자 인터페이스는 처리량이 낮은 게재 또는 준비가 실패한 게재 등 사전 정의된 경고 기준을 제공합니다. 이러한 기준을 대시보드에 추가하거나 필요에 따라 고유한 기준을 만들 수 있습니다. [기준을 사용하여 작업하는 방법을 알아봅니다](../msg/delivery-alerting-criteria.md).

예를 들어 관리 권한이 있는 사용자에게 실패한 게재에 대해서만 알리고 마케팅 사용자에게 소프트 바운스 오류 비율이 높은 게재에 대해 알립니다. 이렇게 하려면 각 수신자 그룹에 대해 적절한 기준을 사용하여 두 개의 별도 대시보드를 만듭니다.

>[!NOTE]
>
>대시보드 및 경고 기준에 액세스하고 구성하려면 **관리 권한**&#x200B;이 있거나 **배달 관리자** 보안 그룹에 속해 있어야 합니다. 표준 사용자는 Adobe Campaign 인터페이스의 대시보드에 액세스할 수 없지만 경고 알림을 받을 수 있습니다. [액세스 및 사용 권한에 대해 자세히 알아보세요](../get-started/permissions.md).