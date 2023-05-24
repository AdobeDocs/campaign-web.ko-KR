---
audience: end-user
title: 오퍼 전송
description: 오퍼 전송
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 100%

---


# 오퍼 전송 {#offers-content}

Adobe Campaign v8 Web에서는 **[!UICONTROL 상호 작용]** 모듈을 사용하여 콘솔에서 생성된 오퍼를 이메일과 함께 전송할 수 있습니다. 상호 작용 정보 및 콘솔에서 오퍼 카탈로그를 관리하는 방법에 대한 자세한 내용은 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html)를 참조하십시오{target="_blank"}.

이메일로 오퍼를 전송하는 단계는 다음과 같습니다.

1. [제안할 오퍼 구성](#configure)
1. [이메일에 오퍼 삽입](#insert)

## 제안할 오퍼 구성 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="오퍼 설정"
>abstract="수신자에게 제안할 오퍼를 구성합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="오퍼 고급 설정"
>abstract="오퍼에 대한 고급 옵션을 구성합니다."

1. 이메일에서 제안할 오퍼를 선택하려면 이메일 콘텐츠 편집 화면에서 **[!UICONTROL 오퍼]** 버튼을 클릭합니다.

   ![](assets/setup-offers.png)

1. 수신자에게 제안할 오퍼를 구성합니다. 먼저 오퍼 환경과 일치하는 **[!UICONTROL 오퍼 공간]**&#x200B;을 선택합니다.

   ![](assets/create-content-offers.png)

1. 엔진의 오퍼 선택을 세분화하려면 오퍼가 정렬되어 있는 특정 **[!UICONTROL 오퍼 범주]**&#x200B;를 선택합니다.

   범주를 지정하지 않는 경우 **[!UICONTROL 오퍼 테마]**&#x200B;가 선택되어 있지 않으면 오퍼 엔진에서 환경에 포함된 모든 오퍼가 고려됩니다.

   >[!NOTE]
   >
   >테마는 범주에서 업스트림으로 정의된 키워드입니다. 필터와 같은 역할을 하며, 범주 세트에서 테마를 선택하여 표시할 오퍼 수를 세분화할 수 있습니다.

1. **[!UICONTROL 제안]** 필드를 사용하면 이메일에 삽입할 오퍼 수를 지정할 수 있습니다.

1. 필요한 경우 **[!UICONTROL 부적격 수신자 제외]** 옵션을 선택하십시오.

   이 옵션을 사용하면 적격 제안이 충분하지 않은 수신자를 제외하는 기능을 활성화하거나 비활성화할 수 있습니다.

   * 옵션을 활성화하면 제안이 충분하지 않은 수신자는 게재에서 제외됩니다.
   * 옵션을 비활성화하면 이러한 수신자가 제외되지는 않지만 요청된 제안 수를 가질 수 없습니다.

1. 필요한 경우 **[!UICONTROL 오퍼가 선택되지 않은 경우 모두 숨기기]** 옵션을 선택하십시오.

   이 옵션을 사용하면 제안 중 하나가 존재하지 않는 경우 메시지 처리 방법을 선택할 수 있습니다.

   * 이 옵션을 활성화하면 누락된 제안의 표현식이 표시되지 않으며 이 제안에 대한 메시지에 콘텐츠가 표시되지 않습니다.
   * 옵션을 비활성화하면 메시지 자체가 전송 중에 취소되며 수신자는 더 이상 메시지를 받을 수 없게 됩니다.

이메일에 제안할 오퍼를 구성한 후에는 표현식 편집기를 사용하여 이메일에 해당 오퍼를 삽입할 수 있습니다. [이메일에 오퍼를 삽입하는 방법 알아보기](#insert)

## 이메일에 오퍼 삽입 {#insert}

표현식 편집기를 사용하여 이메일에 오퍼를 추가할 수 있습니다. 콘텐츠 구성 요소에서 개인화를 허용하여

* 이메일 제목 줄과
* 이메일 본문에 오퍼를 삽입할 수 있습니다. [콘텐츠 구성 요소 추가 방법 알아보기](content-components.md)

>[!NOTE]
>
>오퍼를 삽입하기 전에 [이메일로 제안할 오퍼를 구성](#configure)했는지 확인해야 합니다.

표현식 편집기를 사용하여 오퍼를 삽입하려면 다음 단계를 따르십시오.

1. 표현식 편집기를 연 다음 **[!UICONTROL 제안]** 메뉴를 선택합니다.

   사용 가능한 제안이 목록에 표시됩니다. 제안 수는 제안할 오퍼를 구성할 때 정의됩니다.

   ![](assets/offer-insertion.png)

1. 각 제안에 사용할 수 있는 개인화 필드, 렌더링 기능 또는 오퍼 속성을 사용하여 이메일 제목 또는 본문에 제안을 추가합니다.

   ![](assets/offer-inserted.png)
