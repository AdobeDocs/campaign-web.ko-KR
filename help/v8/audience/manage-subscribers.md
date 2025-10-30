---
audience: end-user
title: 구독자 관리
description: Adobe Campaign 웹에서 서비스 구독자를 관리하고 제공하는 방법에 대해 알아봅니다
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# 구독자 관리 {#manage-subscribers}

[서비스를 만든](manage-services.md#create-service)후에는 구독자를 추가하고, 수신자의 구독을 취소하며, 해당 서비스의 구독자에게 메시지를 보낼 수 있습니다.

구독자 관리는 이 페이지에 자세히 설명되어 있습니다. 구독자에게 메시지를 보내는 방법에 대해 알아보려면 [이 섹션](../msg/send-to-subscribers.md)을 참조하세요.

## 서비스에 구독자 추가 {#add-subscribers}

가입자를 수동으로 추가하려면 아래 단계를 따르십시오.

1. **[!UICONTROL 구독 서비스]** 목록에서 기존 서비스를 선택하십시오.

1. **[!UICONTROL 구독자]** 탭으로 이동한 다음 **[!UICONTROL 구독자 추가]**&#x200B;를 클릭합니다.

   ![구독 서비스 인터페이스의 구독자 탭을 표시하는 스크린샷입니다.](assets/service-subscribers-tab.png){zoomable="yes"}

1. 목록에서 추가할 프로필을 선택하고 **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

   구독자를 추가하기 위한 프로필 선택 인터페이스를 보여 주는 ![스크린샷입니다.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. **[!UICONTROL 서비스를 만들 때]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->정의한 [확인 메시지](manage-services.md#create-confirmation-message)을(를) 선택한 수신자가 받도록 하려면 [보내기](manage-services.md#create-service)를 클릭하십시오.

   구독자를 추가하기 위한 확인 메시지 인터페이스를 보여 주는 ![스크린샷입니다.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >**[!UICONTROL 취소]**&#x200B;를 선택하면 선택한 프로필에 확인 메시지가 전송되지 않지만 구독됩니다.

추가된 프로필은 **[!UICONTROL 구독자]** 탭에 표시됩니다. 이제 서비스를 구독합니다.

## 서비스에서 구독자 제거 {#remove-subscribers}

### 수동으로 프로필 구독 취소 {#manual-unsubscription}

서비스에 [구독자를 추가](#add-subscribers)하면 각 구독자의 구독을 수동으로 취소할 수 있습니다. 아래 단계를 수행합니다.

1. **[!UICONTROL 구독 서비스]** 목록에서 기존 서비스를 선택하십시오.

1. 원하는 받는 사람 이름 옆에 있는 세 점 아이콘을 클릭하고 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

   ![프로필 구독 취소를 위한 삭제 옵션을 보여 주는 스크린샷입니다.](assets/service-subscribers-delete.png){zoomable="yes"}

1. 삭제를 확인합니다.

1. **[!UICONTROL 서비스를 만들 때]**&#x200B;정의한 구독 취소 [확인 메시지](manage-services.md#create-confirmation-message)를 선택한 수신자가 받게 하려면 [보내기](manage-services.md#create-service)를 클릭하십시오.

   ![프로필 구독 취소에 대한 확인 메시지 인터페이스를 보여주는 스크린샷입니다.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

받는 사람이 **[!UICONTROL 구독자]** 탭에서 제거되어 더 이상 서비스를 구독하지 않습니다.

### 수신자 자동 구독 취소 {#automatic-unsubscription}

구독 서비스의 기간은 제한될 수 있습니다. 유효 기간이 만료되면 프로필의 가입이 자동으로 취소됩니다.

이 기간은 [서비스를 만드는 중](manage-services.md#create-service)에 지정됩니다. **[!UICONTROL 추가 옵션]**&#x200B;에서 **[!UICONTROL 무제한 유효 기간]** 옵션을 비활성화하고 서비스 유효 기간을 정의하십시오.

![구독 서비스에 대한 유효 기간 구성을 보여 주는 스크린샷입니다.](assets/service-create-validity-period.png){zoomable="yes"}

지정된 기간이 만료되면 모든 구독자는 해당 서비스에서 자동으로 구독 취소됩니다.