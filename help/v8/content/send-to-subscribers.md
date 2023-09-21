---
audience: end-user
title: 서비스 구독자에게 메시지 보내기
description: 서비스 구독자에게 메시지를 보내는 방법 알아보기
badge: label="Beta"
source-git-commit: 073fc1ca89e5f76dfbac00db7b3d76801635dcc3
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 4%

---


# 서비스 구독자에게 메시지 보내기

Adobe Campaign에서 구독 서비스를 만들고 구독자에게 메시지를 보낼 수 있습니다. 에서 구독 서비스를 만드는 방법 알아보기 [이 페이지](../audience//manage-services.md#create-service).

구독자에게 메시지를 보내려면 특정 대상을 만들어 구독자를 식별한 다음 아래에 설명된 대로 게재를 만듭니다.

1. 대상자 만들기. 에서 대상자에 대해 자세히 알아보기 [이 페이지](../audience/create-audience.md).

1. 다음에서 **[!UICONTROL 대상자 작성]** 활동, 고급 속성 표시 및 선택 **[!UICONTROL 수신자]** > **[!UICONTROL 구독]** > **[!UICONTROL 서비스]**.

   이 예에서는 다음과 같은 서비스를 구독한 사용자를 선택합니다. **Luma 뉴스레터** 레이블.

   ![](assets/service-audience-subscribers.png)

1. 대상자를 저장합니다.
1. 게재 만들기. 게재를 만드는 단계는에 자세히 설명되어 있습니다. [이 페이지](../msg/gs-messages.md#create-delivery).
1. 위에서 만든 대상자를 선택합니다.

   ![](assets/service-delivery-targeting-subscribers.png)

1. 에 자세히 설명된 대로 메시지 콘텐츠를 만들고 게재를 테스트하고 전송합니다. [이 섹션](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

게재는 해당 서비스 가입자에게만 전송됩니다.
