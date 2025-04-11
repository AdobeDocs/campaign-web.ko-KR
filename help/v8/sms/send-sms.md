---
audience: end-user
title: SMS 게재 보내기
description: Adobe Campaign 웹으로 SMS를 보내는 방법 알아보기
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 11%

---

# SMS 게재 미리보기 및 전송 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="새 격리 지표"
>abstract="게재할 메시지 수와 관련하여 게재 실패(알 수 없는 사용자, 잘못된 도메인) 후 격리된 총 주소 수입니다."

## SMS 게재 미리 보기 {#preview-sms}

메시지 콘텐츠를 정의하고 나면 테스트 프로필을 사용하여 미리 보고 테스트합니다. 개인화된 콘텐츠가 포함된 경우 테스트 프로필 데이터를 사용하여 이 콘텐츠가 메시지에 어떻게 표시되는지 확인하십시오. 이렇게 하면 메시지가 의도한 대로 표시되고 개인화된 정보가 올바르게 표시됩니다.

SMS 게재를 미리 보는 주요 단계는 다음과 같습니다. 게재 미리 보기 방법에 대한 자세한 내용은 [이 섹션](../preview-test/preview-content.md)에서 확인할 수 있습니다.

1. 게재 콘텐츠 페이지에서 **[!UICONTROL 콘텐츠 시뮬레이션]**&#x200B;을 사용하여 개인화된 콘텐츠를 미리 봅니다.

   ![개인화된 SMS 콘텐츠 미리 보기](assets/sms_send_1.png){zoomable="yes"}

1. **[!UICONTROL 테스트 프로필 추가]**&#x200B;를 클릭하여 하나 또는 여러 테스트 프로필 또는 프로필을 선택합니다.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 오른쪽 창에서 개인화된 요소가 선택한 프로필의 데이터로 동적으로 대체되는 SMS 게재의 미리보기를 확인합니다.

   ![개인화된 SMS 게재를 표시하는 미리 보기 창](assets/sms_send_3.png){zoomable="yes"}

SMS 메시지를 검토하고 대상자에게 보냅니다.

## SMS 게재 테스트 {#test-sms}

**Adobe Campaign**&#x200B;을(를) 사용하여 메시지를 기본 대상자에게 보내기 전에 테스트하십시오. 이 단계에서는 이메일 캠페인의 유효성을 검사하고 잠재적 문제를 식별합니다.

증명을 보내는 것은 게재의 품질과 효과를 확인하는 데 중요합니다. 증명 수신자는 링크, 옵트아웃 링크 및 이미지와 같은 다양한 요소를 검토하고, 렌더링, 콘텐츠, 개인화 설정 및 SMS 구성에서 발생하는 오류를 식별합니다. 이 프로세스는 주요 대상에게 도달하기 전에 SMS를 철저히 평가하고 최적화합니다.

![증명을 보내기 위한 책 모양 아이콘](../assets/do-not-localize/book.png) [이 섹션](../preview-test/test-deliveries.md)에서 증명을 보내는 방법을 알아봅니다.

![SMS 게재 테스트](assets/sms_send_6.png){zoomable="yes"}

## SMS 게재 보내기 {#send-sms}

1. SMS 콘텐츠를 개인화한 후 **[!UICONTROL 게재]** 페이지에서 **[!UICONTROL 검토 및 보내기]**&#x200B;를 클릭하세요.

   ![SMS 게재 검토 및 보내기](assets/sms_send_4.png){zoomable="yes"}

1. **[!UICONTROL 준비]**&#x200B;를 클릭하고 제공된 진행률과 통계를 모니터링합니다.

   오류가 발생하면 오류에 대한 자세한 내용은 로그 메뉴를 참조하십시오.

1. 마지막 전송 프로세스를 진행하려면 **[!UICONTROL 보내기]**&#x200B;를 클릭하여 메시지를 보냅니다.

   ![SMS 게재 보내기](assets/sms_send_5.png){zoomable="yes"}

   SMS 게재가 예약되어 있으면 **[!UICONTROL 일정대로 보내기]** 단추를 클릭하세요. [이 섹션](../msg/gs-messages.md#schedule-the-delivery-sending)에서 게재 예약에 대해 자세히 알아보세요.

1. **[!UICONTROL 보내기]** 단추를 클릭하여 보내기 작업을 확인합니다.

게재가 전송되면 게재 페이지에서 KPI(주요 성능 지표) 데이터와 **[!UICONTROL 로그]** 메뉴의 데이터를 추적합니다.

기본 제공 보고서를 통해 메시지의 영향을 측정하기 시작합니다. [자세히 알아보기](../reporting/sms-report.md)