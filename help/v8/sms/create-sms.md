---
audience: end-user
title: SMS 게재 만들기
description: Adobe Campaign Web을 사용하여 SMS를 만들고 전송하는 방법 알아보기
badge: label="Beta"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: a67a692cf9b74015323954eca5b4c554f7fe8eb6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 72%

---

# SMS 게재 만들기 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS 게재 속성"
>abstract="속성에는 게재 이름을 지정하고 분류하는 데 도움이 되는 일반적인 게재 매개변수가 포함됩니다. 확장된 스키마를 기반으로 하는 게재인 경우, 특정 사용자 정의 옵션 필드를 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="SMS 대상자 정의"
>abstract="SMS 메시지에 적합한 대상자를 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="SMS 템플릿 선택"
>abstract="SMS 게재를 시작하려면 미리 정의된 템플릿을 선택합니다."

독립형 SMS 게재를 만들거나 캠페인 워크플로우의 컨텍스트에서 SMS를 만들 수 있습니다. 아래 단계에서는 독립 실행형(일회성) SMS 게재 절차를 자세히 설명합니다. 캠페인 워크플로우의 컨텍스트에서 작업 중인 경우 만들기 단계는 의 세부 정보입니다. [이 섹션](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


새 독립 실행형 SMS 게재를 만들려면 다음 단계를 수행합니다.

1. 다음으로 이동 **[!UICONTROL 게재]** 왼쪽 레일에서 메뉴를 클릭하고  **[!UICONTROL 게재 만들기]** 단추를 클릭합니다.

1. **[!UICONTROL 채널]** 섹션 아래에서 SMS를 채널로 선택하고 템플릿을 선택합니다. [템플릿에 대해 자세히 알아보기](../msg/delivery-template.md)

1. **[!UICONTROL 게재 만들기]** 버튼을 클릭하여 확인합니다.

   ![](assets/sms_create_1.png)

1. 게재용 **[!UICONTROL 레이블]**&#x200B;을 입력하고 **[!UICONTROL 추가 옵션]** 드롭다운에 액세스합니다.

   +++요구 사항에 따라 다음 설정을 구성합니다.
   * **[!UICONTROL 내부 이름]**: 게재에 고유 식별자를 할당합니다.
   * **[!UICONTROL 폴더]**: 게재를 특정 폴더에 저장합니다.
   * **[!UICONTROL 게재 코드]**: 고유한 명명 규칙을 사용하여 게재를 구성합니다.
   * **[!UICONTROL 설명]**: 게재에 대한 설명을 입력합니다.
   * **[!UICONTROL 특성]**: 분류 목적으로 이메일의 특성을 지정합니다.
+++

1. **[!UICONTROL 대상자 선택]** 버튼을 클릭하여 기존 대상자를 타겟팅하거나 나만의 대상자를 만듭니다. [자세히 알아보기](../audience/about-audiences.md)

   ![](assets/sms_create_2.png)

1. **[!UICONTROL 컨트롤 그룹 활성화]** 옵션을 켜서 게재의 영향을 측정하는 컨트롤 그룹을 설정하고 메시지를 수신한 모집단 비헤이비어와 메시지를 수신하지 않은 연락처 비헤이비어를 비교할 수 있습니다. [자세히 알아보기](../audience/control-group.md)

1. **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하여 SMS 메시지의 콘텐츠 디자인을 시작합니다. [자세히 알아보기](content-sms.md)

   ![](assets/sms_create_4.png)

   이 화면에서 다음을 수행할 수도 있습니다. [콘텐츠 시뮬레이션](../preview-test/preview-test.md) 및 [오퍼 설정](../content/offers.md).

1. 특정 일자 및 시간에 게재를 예약하려면 **[!UICONTROL 예약 활성화]** 옵션을 켭니다. 게재를 시작하면 수신자에 대해 정의한 정확한 일자와 시간에 메시지가 자동으로 전송됩니다. 에서 게재 예약에 대해 자세히 알아보기 [이 섹션](../msg/gs-messages.md#gs-schedule).

1. 클릭 **[!UICONTROL 게재 설정 구성]** 게재 템플릿과 관련된 고급 옵션에 액세스 [자세히 알아보기](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
