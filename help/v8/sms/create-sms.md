---
audience: end-user
title: SMS 게재 만들기
description: Adobe Campaign Web을 사용하여 SMS를 만들고 전송하는 방법 알아보기
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 43%

---

# SMS 게재 만들기 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS 게재 속성"
>abstract="속성에는 게재 이름을 지정하고 분류하는 데 도움이 되는 일반적인 게재 매개변수가 포함됩니다. 확장된 스키마를 기반으로 하는 게재인 경우, 특정 사용자 정의 옵션 필드를 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="SMS 대상자 정의"
>abstract="**대상자 선택** 버튼을 클릭하여 새 대상자를 만들거나 기존 대상자를 선택할 수 있습니다. 필요한 경우 컨트롤 그룹을 추가하여 게재의 영향을 측정할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=ko" text="컨트롤 그룹 설정"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="SMS 템플릿 선택"
>abstract="SMS 게재를 시작하려면 미리 정의된 템플릿을 선택합니다. 게재 템플릿을 사용하면 캠페인과 게재 전반에 걸쳐 사용자 정의 콘텐츠와 설정을 쉽게 재사용할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=ko" text="게재 템플릿 사용"


독립형 SMS 게재를 만들거나 캠페인 워크플로우의 컨텍스트에서 SMS를 만들 수 있습니다. 아래 단계에서는 독립 실행형(일회성) SMS 게재 절차를 자세히 설명합니다. 캠페인 워크플로우의 컨텍스트에서 작업 중인 경우 [이 섹션](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow)에 만들기 단계가 자세히 설명되어 있습니다.


새 독립 실행형 SMS 게재를 만들려면 다음 단계를 수행합니다.

1. 왼쪽 레일의 **[!UICONTROL 게재]** 메뉴로 이동한 다음 **[!UICONTROL 게재 만들기]** 단추를 클릭합니다.

1. **[!UICONTROL 채널]** 섹션에서 SMS를 채널로 선택하고 템플릿을 선택합니다. [템플릿에 대해 자세히 알아보기](../msg/delivery-template.md)

1. **[!UICONTROL 게재 만들기]** 버튼을 클릭하여 확인합니다.

   ![](assets/sms_create_1.png){zoomable="yes"}

1. 게재할 **[!UICONTROL 레이블]**&#x200B;을(를) 입력하고 **[!UICONTROL 추가 옵션]** 드롭다운에 액세스합니다. 게재가 확장된 스키마를 기반으로 하는 경우 특정 **사용자 지정 옵션** 필드를 사용할 수 있습니다.

   +++요구 사항에 따라 다음 설정을 구성합니다.
   * **[!UICONTROL 내부 이름]**: 게재에 고유 식별자를 할당합니다.
   * **[!UICONTROL 폴더]**: 게재를 특정 폴더에 저장합니다.
   * **[!UICONTROL 게재 코드]**: 고유한 명명 규칙을 사용하여 게재를 구성합니다.
   * **[!UICONTROL 설명]**: 게재에 대한 설명을 입력합니다.
   * **[!UICONTROL 특성]**: 분류 목적으로 게재 특성을 지정합니다.
+++

1. **[!UICONTROL 대상자 선택]** 버튼을 클릭하여 기존 대상자를 타겟팅하거나 나만의 대상자를 만듭니다. [대상자에 대해 자세히 알아보기](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable="yes"}

   [이 페이지](../audience/add-audience.md)에서 기존 대상자를 선택하는 방법을 알아보세요.

   [이 페이지](../audience/one-time-audience.md)에서 새 대상자를 만드는 방법을 알아봅니다.

1. 게재의 영향을 측정하는 컨트롤 그룹을 설정하려면 **[!UICONTROL 컨트롤 그룹 사용]** 옵션을 켜십시오. 메시지가 해당 컨트롤 그룹으로 전송되지 않으므로 메시지를 받은 모집단의 행동과 받지 않은 연락처의 행동을 비교할 수 있습니다. [자세히 알아보기](../audience/control-group.md)

1. SMS 메시지의 콘텐츠 디자인을 시작하려면 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요. [자세히 알아보기](content-sms.md)

   ![](assets/sms_create_4.png){zoomable="yes"}

   이 화면에서 [콘텐츠를 시뮬레이션](../preview-test/preview-test.md)하고 [오퍼를 설정](../msg/offers.md)할 수도 있습니다.

1. 특정 일자 및 시간에 게재를 예약하려면 **[!UICONTROL 예약 활성화]** 옵션을 켭니다. 게재를 시작하면 메시지가 수신자를 위해 정의한 정확한 날짜 및 시간에 자동으로 전송됩니다. [이 섹션](../msg/gs-deliveries.md#gs-schedule)에서 게재 예약에 대해 자세히 알아보세요.

   >[!NOTE]
   >
   >워크플로우의 컨텍스트에서 게재를 보낼 때는 **스케줄러** 활동을 사용해야 합니다. [이 페이지](../workflows/activities/scheduler.md)에서 자세히 알아보십시오.

1. **[!UICONTROL 설정]**&#x200B;을 클릭하여 게재 템플릿과 관련된 고급 옵션에 액세스합니다. [자세히 알아보기](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable="yes"}
