---
audience: end-user
title: 오퍼 보내기
description: 오퍼 보내기
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 1%

---

# 오퍼 보내기 {#offers-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="오퍼 설정"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="오퍼 고급 설정"
>abstract="TBC"

Adobe Campaign v8 웹을 사용하면 콘솔에서 만든 이메일 오퍼와 함께 **[!UICONTROL 상호 작용]** 모듈. 상호 작용 및 콘솔에서 오퍼 카탈로그를 관리하는 방법에 대한 자세한 내용은 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

이메일을 사용하여 오퍼를 전송하는 단계는 다음과 같습니다.

1. [제안할 오퍼 구성](#configure),
1. [이메일에 오퍼를 삽입합니다](#insert).

## 제안할 오퍼 구성 {#configure}

1. 이메일에서 제안할 오퍼를 선택하려면 **[!UICONTROL 오퍼]** 이메일 콘텐츠 편집 화면의 단추.

   ![](assets/setup-offers.png)

1. 수신자에게 제안할 오퍼를 구성합니다. 먼저 을(를) 선택합니다 **[!UICONTROL 오퍼 공간]** 오퍼 환경과 일치합니다.

   ![](assets/create-content-offers.png)

1. 엔진의 오퍼 선택 사항을 세분화하려면 특정 오퍼를 선택합니다 **[!UICONTROL 오퍼 카테고리]** 오퍼가 정렬되는 위치.

   카테고리를 지정하지 않으면, **[!UICONTROL 오퍼 테마]** 이 선택되어 있습니다.

   >[!NOTE]
   >
   >테마는 카테고리에서 업스트림으로 정의된 주요 단어입니다. 오퍼는 필터 역할을 하며 카테고리 집합에서 오퍼를 선택하여 표시할 오퍼 수를 구체화할 수 있습니다.

1. 를 사용하십시오 **[!UICONTROL Proposition]** 필드에 전자 메일에 삽입할 오퍼 수를 지정합니다.

1. 을(를) 선택합니다 **[!UICONTROL 자격이 없는 수신자 제외]** 필요한 경우 옵션을 선택합니다.

   이 옵션을 사용하면 적합한 오퍼가 충분하지 않은 수신자의 제외를 활성화하거나 비활성화할 수 있습니다.

   * 이 옵션이 활성화되면 적절한 위치가 없는 수신자는 게재에서 제외됩니다.
   * 이 옵션을 비활성화하면 이러한 수신자는 제외되지 않지만 요청된 제안 수를 가질 수 없습니다.

1. 필요한 경우 **[!UICONTROL 오퍼를 선택하지 않은 경우 모든 것을 숨깁니다]** 선택 사항입니다.

   이 옵션을 사용하면 프로필 중 하나가 없는 경우 메시지가 처리되는 방식을 선택할 수 있습니다.

   * 옵션을 활성화하면 누락된 제안 표현이 표시되지 않고 이 제안에 대한 메시지에 콘텐츠가 표시되지 않습니다.
   * 이 옵션을 비활성화하면 전송 중에 메시지 자체가 취소되고 수신자는 더 이상 메시지를 받을 수 없습니다.

전자 메일에 오퍼를 제안하도록 구성한 후에는 표현식 편집기를 사용하여 전자 메일에 오퍼를 삽입할 수 있습니다. [이메일에 오퍼를 삽입하는 방법을 알아봅니다](#insert)

## 이메일에 오퍼 삽입 {#insert}

표현식 편집기를 사용하여 오퍼를 이메일에 추가할 수 있습니다. 다음 중 하나를 삽입할 수 있습니다.

* 이메일 제목 줄에서,
* 모든 컨텐츠 구성 요소에서 개인화를 허용하여 이메일 본문에 있는 경우를 설명합니다. [콘텐츠 구성 요소를 추가하는 방법을 알아봅니다](content-components.md)

>[!NOTE]
>
>오퍼를 삽입하기 전에 [이메일을 사용하여 제안할 오퍼를 구성했습니다](#configure).

표현식 편집기를 사용하여 오퍼를 삽입하려면 다음 단계를 수행합니다.

1. 표현식 편집기를 열고 **[!UICONTROL Proposition]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   사용 가능한 프로필이 목록에 표시됩니다. 제안할 오퍼를 구성할 때 제안 수가 정의됩니다.

   ![](assets/offer-insertion.png)

1. 각 제안을 위해 사용할 수 있는 개인화 필드, 렌더링 기능 또는 오퍼 속성을 사용하여 이메일 주체 또는 본문에 제안을 추가합니다.

   ![](assets/offer-inserted.png)
