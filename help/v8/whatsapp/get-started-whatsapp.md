---
audience: end-user
title: WhatsApp 메시지 시작
description: Adobe Campaign 웹 사용자 인터페이스를 사용하여 WhatsApp 메시지를 만들고 보내는 방법을 알아봅니다
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---

# WhatsApp 메시지 시작 {#get-started-whatsapp}

Meta의 **Cloud API**&#x200B;를 사용하여 [Adobe Campaign 웹 사용자 인터페이스](https://developers.facebook.com/docs/whatsapp/cloud-api/)에서 WhatsApp 메시지를 보낼 수 있습니다. 다른 채널과 함께 독립 실행형 게재, 캠페인 워크플로우 또는 마케팅 캠페인 내에서 WhatsApp을 사용합니다.

* **[!UICONTROL 게재]**: Adobe Campaign 웹 사용자 인터페이스에서 왼쪽 레일의 **[!UICONTROL 게재]** 메뉴에서 독립 실행형 WhatsApp 게재를 만듭니다(SMS 또는 푸시와 유사). [자세히 알아보기](create-whatsapp.md).

* **[!UICONTROL 캠페인]**: Adobe Campaign 웹 사용자 인터페이스에서 캠페인을 열고 **[!UICONTROL 게재]** 탭에서 WhatsApp 게재를 추가하거나 캠페인에 연결된 워크플로우로 전송을 오케스트레이션합니다. [자세히 알아보기](../campaigns/create-campaigns.md).

* **[!UICONTROL 워크플로]**: Adobe Campaign 웹 사용자 인터페이스의 워크플로 캔버스에서 **[!UICONTROL WhatsApp]** 채널 활동을 추가하고 게재 템플릿을 선택한 다음 게재 대시보드에서 콘텐츠 및 설정을 정의합니다. [이 섹션](../workflows/activities/channels.md)에서 채널 활동에 대해 자세히 알아보세요.

## 전제 조건 {#prereq}

WhatsApp을 통합하려면 다음 요구 사항이 있습니다.

* Meta Business Manager 계정
* [보낸 사람 이름과 전화 번호가 확인된 WhatsApp 비즈니스 계정](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [적절한 권한이 있는 사용자 인증 토큰](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [승인된 Meta 템플릿](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

계속하기 전에 다음 사항을 확인해야 합니다.

* [WhatsApp 콘텐츠 규칙](https://www.whatsapp.com/legal/messaging-guidelines)
* [Meta 정책 준수](https://www.whatsapp.com/legal)
* [24시간 대화 제한](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


