---
audience: end-user
title: 구독 서비스 작업
description: Adobe Campaign 웹에서 구독 서비스에 액세스하고, 만들고, 관리하는 방법을 알아봅니다
badge: label="Beta"
source-git-commit: 5125de258edd4e3eda9a8507228156ee40215532
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 3%

---


# 구독 서비스 작업 {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="서비스 만들기 및 관리"
>abstract="Adobe Campaign을 사용하여 뉴스레터와 같은 서비스를 만들고 모니터링하며 이러한 서비스에 대한 구독 또는 구독 취소를 확인합니다. 구독은 이메일 및 SMS 게재에만 적용됩니다."

Adobe Campaign 웹을 사용하여 뉴스레터와 같은 서비스를 관리 및 생성하고, 이러한 서비스에 대한 구독 또는 구독 취소를 확인하십시오.

>[!NOTE]
>
>구독은 이메일 및 SMS 게재에만 적용됩니다.

예를 들어 특정 제품 카테고리에 대한 뉴스레터, 웹 사이트의 테마 또는 영역, 다양한 유형의 경고 메시지 구독 및 실시간 알림과 같은 여러 서비스를 동시에 정의할 수 있습니다.

구독 및 구독 취소 관리에 대한 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## 구독 서비스 액세스 {#access-services}

플랫폼에서 사용할 수 있는 구독 서비스에 액세스하려면 아래 단계를 따르십시오.

1. 다음으로 이동 **[!UICONTROL 구독 서비스]** 메뉴 아래의 왼쪽 탐색 레일에서 사용할 수 있습니다.

   ![](assets/service-list.png)

1. 모든 기존 구독 서비스 목록이 표시됩니다. 채널, 폴더에서 서비스 및 필터를 검색하거나 고급 필터를 사용할 수 있습니다.

   ![](assets/service-filters.png)

1. 기존 서비스를 편집하려면 해당 이름을 클릭합니다.

1. 이 서비스 이름 옆에 있는 세 점 아이콘을 사용하여 서비스를 삭제하거나 복제할 수 있습니다.<!--so all subscribers are unsuibscribed - need to mention?-->

## 첫 번째 구독 서비스 만들기 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="서비스 속성 정의"
>abstract="구독 서비스 레이블을 입력하고 서비스 유효 기간과 같은 추가 옵션을 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="확인 메시지 선택"
>abstract="사용자가 서비스를 구독하거나 구독 취소하면 확인 메시지를 보낼 수 있습니다. 해당 메시지에 사용할 템플릿을 선택합니다."

구독 서비스를 만들려면 아래 단계를 수행하십시오.

1. 다음 항목 선택 **[!UICONTROL 구독 서비스 만들기]** 단추를 클릭합니다.

   ![](assets/service-create-button.png)

1. 채널 선택: **[!UICONTROL 이메일]** 또는 **[!UICONTROL SMS]**.

1. 서비스 속성에서 레이블을 입력하고 원하는 대로 추가 옵션을 정의합니다.

   ![](assets/service-create-properties.png)

1. 기본적으로 구독은 무제한입니다. 다음을 비활성화할 수 있습니다. **[!UICONTROL 무제한 유효 기간]** 서비스의 유효 기간을 정의하는 옵션.

   아래 예에서는 20일 후입니다.
   * 더 이상 이 서비스에 가입할 수 있는 수신자가 없습니다.
   * 이 서비스의 모든 구독자는 20일 후에 자동으로 구독 취소됩니다. [자세히 알아보기](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. 사용자가 서비스를 구독하거나 구독 취소하면 확인 메시지를 보낼 수 있습니다. 사용 사례에 따라 해당 메시지에 사용할 템플릿을 선택합니다. 이러한 템플릿은 **[!UICONTROL 구독]** 대상 매핑. [자세히 알아보기](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. 클릭 **[!UICONTROL 저장 및 검토]**. 새 서비스가 다음에 추가됩니다. **[!UICONTROL 구독 서비스]** 목록을 표시합니다.

## 확인 메시지 만들기 {#create-confirmation-message}

서비스를 구독하거나 구독 취소하는 사용자에게 확인 메시지를 보내려면 **[!UICONTROL 구독]** 정의된 대상 없이 대상 매핑. 이렇게 하려면 아래 단계를 수행합니다.

1. 구독 확인을 위한 게재 템플릿을 만듭니다. [방법 알아보기](../msg/delivery-template.md)

1. 이 게재의 대상자를 선택하지 마십시오. 대신, **[!UICONTROL 게재 설정]**&#x200B;로 이동합니다. [대상자](../advanced-settings/delivery-settings.md#audience) 탭을 클릭하고 다음을 선택합니다. **[!UICONTROL 구독]** 목록에서 대상 매핑입니다.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >을(를) 선택하지 않으면  **[!UICONTROL 구독]** 대상 매핑에서 구독자가 확인 메시지를 받지 못합니다. 대상 매핑은 Campaign v8 콘솔에서 정의됩니다. 자세히 알아보기 [Adobe Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

1. 게재 템플릿의 콘텐츠를 편집하고 저장하고 닫습니다.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >게재 채널 및 에서 게재 콘텐츠를 정의하는 방법에 대해 자세히 알아보기 [이메일 채널](../email/create-email.md) 및 [SMS 채널](../sms/create-sms.md) 섹션.

1. 구독 취소 확인을 위한 게재 템플릿을 만들려면 위의 단계를 반복하십시오.

이제 다음과 같은 경우에 이러한 메시지를 선택할 수 있습니다. [구독 서비스 만들기](#create-service). 해당 서비스를 구독하거나 구독 취소하는 사용자는 선택한 확인 메시지를 받게 됩니다.

## 구독 서비스 로그 및 보고서 {#logs-and-reports}

SMS 및 이메일 채널에 대한 구독 서비스의 효과를 측정하기 위해 주어진 서비스에 대한 로그 및 보고서에 액세스할 수 있습니다.

1. 에서 기존 서비스 선택 **[!UICONTROL 구독 서비스]** 목록을 표시합니다. 클릭 **[!UICONTROL 계산]** 총 구독자 수를 가져옵니다.

   ![](assets/service-logs-reports-buttons.png)

1. 서비스 대시보드에서 을(를) 선택합니다 **[!UICONTROL 로그]** 이 서비스의 구독자 목록을 봅니다. 전체 가입자 수, 각 수신자의 이름 및 주소, 가입 또는 가입 해지 시점을 확인할 수 있다. 필터링할 수도 있습니다.

   ![](assets/service-logs.png)

1. 서비스 대시보드에서 을(를) 선택합니다 **[!UICONTROL 보고서]**. 다음 지표를 확인하십시오.

   * 다음 **[!UICONTROL 총 구독자 수]** 이 표시됩니다.

   * 선택한 기간 동안의 구독 및 구독 취소 수를 볼 수 있습니다. 드롭다운 목록을 사용하여 시간 범위를 변경합니다.

     ![](assets/service-reports.png)

   * 다음 **[!UICONTROL 구독의 전반적인 발전]** 그래프는 구독, 구독 취소, 숫자 진화 및 충성도 비율을 포함하여 기간별 분류를 보여 줍니다.<!--what is Registered?-->

1. 사용 **[!UICONTROL 다시 로드]** 추적 워크플로우의 실행 및 일정에서 마지막 값을 검색하는 단추입니다.








