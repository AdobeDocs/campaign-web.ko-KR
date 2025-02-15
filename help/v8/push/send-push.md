---
audience: end-user
title: 푸시 알림 게재 보내기
description: Adobe Campaign 웹을 사용하여 푸시 알림 게재를 보내는 방법 알아보기
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 2%

---

# 푸시 게재 미리 보기 및 보내기 {#send-push-delivery}

## 푸시 알림 게재 미리 보기 {#preview-push}

메시지 콘텐츠를 정의했으면 테스트 구독자를 활용하여 메시지를 미리 보고 테스트할 수 있습니다. 개인화된 콘텐츠를 포함한 경우 테스트 프로필 데이터를 사용하여 이 콘텐츠가 메시지에 어떻게 표시되는지 검사할 수 있습니다. 이렇게 하면 메시지가 올바르게 렌더링되고 개인화된 요소가 적절하게 통합되는지 확인할 수 있습니다.

푸시 알림을 미리 보는 주요 단계는 다음과 같습니다. 게재 미리 보기 방법에 대한 자세한 내용은 [이 섹션](../preview-test/preview-content.md)에서 확인할 수 있습니다.

1. 게재 콘텐츠 페이지에서 **[!UICONTROL 콘텐츠 시뮬레이션]**&#x200B;을 사용하여 개인화된 콘텐츠를 미리 봅니다.

   ![](assets/push_send_1.png){zoomable="yes"}

1. 푸시 알림 콘텐츠에서 데이터를 미리 볼 하나 이상의 프로필을 선택하려면 **[!UICONTROL 구독자 추가]**&#x200B;를 클릭하십시오.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. 오른쪽 창에는 개인화된 요소가 선택한 프로필의 데이터로 동적으로 대체되는 푸시 알림의 미리보기가 있습니다.

   ![](assets/push_send_7.png){zoomable="yes"}

이제 푸시 알림을 검토하여 대상자에게 전송할 수 있습니다.

## 푸시 알림 게재 테스트 {#test-push}

**Adobe Campaign**&#x200B;을(를) 사용하면 증명을 주요 대상자에게 보내기 전에 보낼 수 있습니다. 이 단계는 게재의 유효성을 검사하고 문제를 식별하는 데 중요합니다.

테스트 프로필은 증명 수신자입니다. 구성 요소와 링크, 이미지 및 개인화와 같은 설정을 검토하고 유효성을 검사하여 최적의 성능을 보장하고 오류를 감지할 수 있습니다. 이 프로세스는 주요 대상에게 도달하기 전에 푸시 알림을 세분화하고 최적화하는 데 도움이 됩니다. [증명을 보내는 방법 알아보기](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable="yes"}

## 푸시 알림 게재 보내기 {#send-push}

1. 푸시 알림 콘텐츠를 개인화한 후 **[!UICONTROL 게재]** 페이지에서 **[!UICONTROL 검토 및 보내기]**&#x200B;를 클릭하세요.

   ![](assets/push_send_2.png){zoomable="yes"}

1. **[!UICONTROL 준비]**&#x200B;를 클릭하고 제공된 진행률과 통계를 모니터링합니다.

   오류가 발생하는 경우 오류에 대한 자세한 내용은 로그 메뉴를 참조하십시오.

   ![](assets/push_send_3.png){zoomable="yes"}

1. 마지막 전송 프로세스를 진행하려면 **[!UICONTROL 보내기]**&#x200B;를 클릭하여 메시지를 보냅니다.

1. **[!UICONTROL 보내기]**&#x200B;를 클릭하여 보내기 작업을 확인합니다.

   푸시 게재가 예약된 경우 **[!UICONTROL 예약된 대로 보내기]** 단추를 클릭합니다. [이 섹션](../msg/gs-messages.md#schedule-the-delivery-sending)에서 게재 예약에 대해 자세히 알아보세요.

   ![](assets/push_send_4.png){zoomable="yes"}

게재가 전송되면 게재 페이지에서 KPI(주요 성능 지표) 데이터와 **[!UICONTROL 로그]** 메뉴의 데이터를 추적할 수 있습니다.

이제 기본 제공 보고서를 통해 메시지의 영향을 측정할 수 있습니다. [자세히 알아보기](../reporting/push-report.md)
