---
audience: end-user
title: 게재 경고
description: 게재 경고 작업 방법을 알아봅니다.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 2%

---

# 게재 경고 시작 {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="게재 경고"
>abstract="이제 Campaign에서 게재 알림을 사용할 수 있습니다. 이 기능은 사용자 그룹이 게재 실행에 대한 정보가 포함된 이메일 알림을 자동으로 수신할 수 있도록 하는 경고 관리 시스템입니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko-KR" text="릴리스 정보 참조"

게재 경고는 사용자 그룹이 게재 실행에 대한 정보가 포함된 이메일 알림을 자동으로 수신할 수 있는 경고 관리 시스템입니다. 수신자는 Adobe Campaign에서 처리하는 진행 중인 게재를 모니터링하고 문제가 발생하는 경우 적절한 조치를 취할 수 있습니다.

Adobe Campaign 웹 사용자 인터페이스를 통해 정의된 특정 경고 기준에 따라 알림을 사용자 지정할 수 있습니다.

게재 실패를 관리하는 방법에 대한 자세한 내용은 [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## 이메일 알림 콘텐츠 {#content}

이메일 알림에는 다음 섹션이 포함됩니다.

* **요약**: 정의된 기준을 충족하는 게재 수를 각 기준에 대한 레이블과 색상으로 표시합니다.
* **세부 사항**: 대시보드에 대해 정의된 모든 게재 기준과 각 기준에 대한 해당 게재를 나열합니다.

![](assets/alerting-email.png)

## 게재 경고 설정 {#set-up}

이러한 경고를 설정하는 데 도움이 되도록 Campaign 웹 사용자 인터페이스를 사용하여 다음을 만들고 관리할 수 있습니다.

* **게재 경고 대시보드**: 수신자를 지정하고, 대시보드에 포함할 경고 기준을 설정하고, 전송된 경고 기록에 액세스합니다. [대시보드 작업 방법 알아보기](../msg/delivery-alerting-dashboards.md)
* **게재 경고 기준**: Campaign 웹 사용자 인터페이스는 대시보드에 추가할 수 있는 사전 정의된 경고 기준(낮은 처리량을 가진 게재, 준비에 실패한 게재...)을 제공합니다. 필요에 따라 고유한 기준을 만들 수도 있습니다. [기준 작업 방법 알아보기](../msg/delivery-alerting-criteria.md)

관리 권한이 있는 사용자에게 실패한 게재에 대해서만 알리고 마케팅 사용자에게 소프트 바운스 오류 비율이 높은 게재에 대해 알린다고 가정합니다. 이렇게 하려면 각 수신자 그룹에 대해 적절한 기준을 사용하여 두 개의 별도 대시보드를 만듭니다.

>[!NOTE]
>
>대시보드 및 경고 기준에 액세스하고 구성하려면 다음을 수행해야 합니다. **관리 권한** 또는 의 일부여야 함 **게재 감독자** 보안 그룹입니다. 표준 사용자는 Adobe Campaign 인터페이스의 대시보드에 액세스할 수 없지만 경고 알림을 받을 수 있습니다. [액세스 및 권한에 대한 자세한 정보](../get-started/permissions.md)
