---
audience: end-user
title: 서비스 구독자에게 메시지 보내기
description: 서비스 구독자에게 메시지를 보내는 방법 알아보기
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# 서비스 구독자에게 메시지 보내기 {#send-to-subscribers}

Adobe Campaign에서 구독 서비스를 만들고 구독자에게 메시지를 보낼 수 있습니다. [이 페이지](../audience//manage-services.md#create-service)에서 구독 서비스를 만드는 방법을 알아보세요.

구독자에게 메시지를 보내려면 특정 대상을 만들어 구독자를 식별한 다음 아래에 설명된 대로 게재를 만듭니다.

1. 대상자를 만듭니다. 새 워크플로우는 자동으로 만들어집니다. [대상자에 대해 자세히 알아보기](../audience/create-audience.md).

1. 가독성을 향상시키려면 워크플로 설정의 **레이블** 필드에서 워크플로 이름을 변경하십시오. [워크플로 설정을 구성하는 방법을 알아보세요](../workflows/workflow-settings.md).

1. **[!UICONTROL 대상자 만들기]** 활동을 열고 **[!UICONTROL 대상자 만들기]**&#x200B;를 선택합니다. [대상 만들기 활동을 구성하는 방법을 알아봅니다](../workflows/activities/build-audience.md).

   ![Adobe Campaign에서 대상 만들기 활동 구성을 보여 주는 스크린샷입니다.](assets/service-create-audience.png){zoomable="yes"}

1. 대상 만들기 흐름에서 다음 사용자 지정 조건을 선택합니다. **[!UICONTROL 구독]**&#x200B;이(가) 있음, 예: **[!UICONTROL 서비스]**&#x200B;이(가) 정의한 서비스와 같음. 이 예제에서는 **Luma 요가 뉴스레터**&#x200B;를 선택합니다.

   ![Adobe Campaign에서 구독에 대한 사용자 지정 조건을 사용하는 대상 만들기 흐름을 보여 주는 스크린샷입니다.](assets/service-audience-subscribers.png){zoomable="yes"}

1. **[!UICONTROL 확인]**&#x200B;을 선택하고 **[!UICONTROL 시작]**&#x200B;을 클릭하여 워크플로우를 실행합니다.

1. 게재를 만듭니다. 게재를 만드는 단계는 [이 페이지](../msg/gs-messages.md#create-delivery)에 자세히 설명되어 있습니다.

1. 게재 설정을 찾아보고 기본 대상 매핑을 **구독(nms:subscriptions)**(으)로 변경합니다.

   ![대상 매핑이 Adobe Campaign의 구독으로 변경된 게재 설정을 보여 주는 스크린샷](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. 게재의 기본 타겟 섹션에서 위에서 만든 대상자를 선택합니다.

   ![Adobe Campaign에서 선택한 대상이 있는 게재의 주요 대상 섹션을 보여 주는 스크린샷입니다.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. [이 섹션](../preview-test/preview-test.md)에 자세히 설명된 대로 메시지 콘텐츠를 만들고 테스트하고 게재를 보냅니다.

   ![Adobe Campaign에서 전송할 준비가 된 게재를 보여 주는 스크린샷입니다.](assets/service-delivery-ready.png){zoomable="yes"}

게재는 해당 서비스 가입자에게만 전송됩니다.