---
audience: end-user
title: 구독 서비스 작업
description: Adobe Campaign 웹에서 서비스를 만드는 방법에 대해 알아봅니다.
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# 구독 서비스 작업 {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="서비스 만들기 및 관리"
>abstract="Adobe Campaign을 사용하여 뉴스레터와 같은 서비스를 만들고 모니터링하고 이러한 서비스에 대한 구독/구독 취소를 확인합니다. 구독은 이메일 및 SMS 게재에만 적용됩니다."

Adobe Campaign 웹을 사용하여 뉴스레터와 같은 서비스를 관리 및 생성하고 이러한 서비스에 대한 구독/구독 취소를 확인하십시오.

>[!NOTE]
>
>구독은 이메일 및 SMS 게재에만 적용됩니다.

예를 들어 특정 제품 카테고리에 대한 뉴스레터, 웹 사이트의 테마 또는 영역, 다양한 유형의 경고 메시지 구독 및 실시간 알림과 같은 여러 서비스를 동시에 정의할 수 있습니다.

구독 및 구독 취소 관리에 대한 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## 구독 서비스 액세스 {#access-services}

플랫폼에서 사용할 수 있는 구독 서비스에 액세스하려면 **[!UICONTROL 구독 서비스]** 메뉴 아래의 왼쪽 탐색 레일에서 사용할 수 있습니다.

![](assets/service-list.png)

모든 기존 구독 서비스 목록이 표시됩니다. 채널, 폴더에서 서비스 및 필터를 검색하거나 고급 필터를 사용할 수 있습니다.

![](assets/service-filters.png)

기존 서비스를 편집하려면 해당 이름을 클릭합니다.

## 첫 번째 구독 서비스 만들기 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="구독 서비스 속성"
>abstract="구독 서비스 레이블을 입력하고 추가 옵션을 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="구독 서비스 확인 메시지"
>abstract="사용자가 서비스에 가입하거나 서비스에서 가입을 해지할 때 확인 메시지를 보낼 수 있습니다. 이 메시지에 사용할 템플릿을 선택합니다."


구독 서비스를 만들려면 다음 단계를 수행하십시오.

1. 다음 항목 선택 **[!UICONTROL 구독 서비스 만들기]** 단추를 클릭합니다.

   ![](assets/service-create-button.png)

1. 채널 선택: **[!UICONTROL 이메일]** 또는 **[!UICONTROL SMS]**.

1. 서비스 속성에서 레이블을 입력하고 원하는 대로 추가 옵션을 정의합니다.

   ![](assets/service-create-properties.png)

1. 기본적으로 구독은 무제한입니다. 다음을 비활성화할 수 있습니다. **[!UICONTROL 무제한 유효 기간]** 서비스의 유효 기간을 정의하는 옵션. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. 사용자가 서비스를 구독하거나 구독 취소하면 확인 메시지를 보낼 수 있습니다. 사용 사례에 따라 해당 메시지에 사용할 템플릿을 선택합니다.

   ![](assets/service-create-confirmation-msg.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 새 서비스가 다음에 추가됩니다. **[!UICONTROL 구독 서비스]** 목록을 표시합니다.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


