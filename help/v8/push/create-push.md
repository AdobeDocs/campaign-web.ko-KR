---
audience: end-user
title: 푸시 알림 게재 만들기
description: Adobe Campaign 웹을 사용하여 푸시 알림 게재를 만드는 방법을 알아봅니다
badge: label="알파"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 67%

---

# 푸시 알림 게재 만들기 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="푸시 대상자 정의"
>abstract="푸시 메시지에 적합한 대상자를 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="푸시 알림 템플릿"
>abstract="푸시 게재를 시작하려면 푸시 알림 템플릿을 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="게재 속성 푸시"
>abstract="게재 속성을 관리합니다."

1. **[!UICONTROL 게재]** 홈 페이지에서 **[!UICONTROL 게재 만들기]**&#x200B;를 클릭합니다.

1. 아래 **[!UICONTROL 채널]** 섹션에서 푸시 알림을 채널로 선택하고 선택한 운영 체제에 따라 템플릿을 선택합니다. Android 또는 iOS. [템플릿에 대해 자세히 알아보기](../msg/delivery-template.md)

1. **[!UICONTROL 게재 만들기]** 버튼을 클릭하여 확인합니다.

   ![](assets/push_create_1.png)

1. 게재용 **[!UICONTROL 레이블]**&#x200B;을 입력하고 **[!UICONTROL 추가 옵션]** 드롭다운에 액세스합니다.

   +++요구 사항에 따라 다음 설정을 구성합니다.
   * **[!UICONTROL 내부 이름]**: 게재에 고유 식별자를 할당합니다.
   * **[!UICONTROL 폴더]**: 게재를 특정 폴더에 저장합니다.
   * **[!UICONTROL 게재 코드]**: 고유한 명명 규칙을 사용하여 게재를 구성합니다.
   * **[!UICONTROL 설명]**: 게재에 대한 설명을 입력합니다.
   * **[!UICONTROL 특성]**: 분류 목적으로 이메일의 특성을 지정합니다.
+++

1. 다음에서 **[!UICONTROL 대상자]** 메뉴에서 이 게재에 사용할 애플리케이션을 선택합니다.

1. **[!UICONTROL 대상자 선택]** 버튼을 클릭하여 기존 대상자를 타겟팅하거나 나만의 대상자를 만듭니다. [자세히 알아보기](../audience/about-audiences.md)

   기본적으로 푸시 알림은 애플리케이션의 모든 구독자에게 전송됩니다.

   ![](assets/push_create_2.png)

1. **[!UICONTROL 컨트롤 그룹 활성화]** 옵션을 켜서 게재의 영향을 측정하는 컨트롤 그룹을 설정하고 메시지를 수신한 모집단 비헤이비어와 메시지를 수신하지 않은 연락처 비헤이비어를 비교할 수 있습니다. [자세히 알아보기](../audience/control-group.md)

1. 클릭 **[!UICONTROL 콘텐츠 편집]** 푸시 알림의 콘텐츠 디자인을 시작합니다.

1. 특정 일자 및 시간에 게재를 예약하려면 **[!UICONTROL 예약 활성화]** 옵션을 켭니다. 게재를 시작하면 수신자에 대해 정의한 정확한 일자와 시간에 메시지가 자동으로 전송됩니다.

   ![](assets/push_create_3.png)

1. 클릭 **[!UICONTROL 게재 설정 구성]** 게재 템플릿과 관련된 고급 옵션에 액세스 [자세히 알아보기](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
