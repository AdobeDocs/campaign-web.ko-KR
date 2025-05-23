---
solution: Campaign, Campaign v8 Web User Interface
title: 랜딩 페이지 사용 사례
description: Campaign 웹 사용자 인터페이스의 랜딩 페이지에서 가장 일반적인 사용 사례를 살펴봅니다
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: 랜딩, 랜딩 페이지, 사용 사례
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 9%

---

# 랜딩 페이지 사용 방법 {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="URL 복사 시 주의"
>abstract="랜딩 페이지를 완전히 테스트하거나 활용하려는 경우, 이 링크를 웹 브라우저나 게재에 직접 복사하여 붙여넣을 수 없습니다. 대신 **콘텐츠 시뮬레이션** 기능을 사용하여 랜딩 페이지를 테스트하고 설명서에 기재된 단계에 따라 랜딩 페이지를 적절하게 활용하면 됩니다."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="URL 복사 시 주의"
>abstract="랜딩 페이지를 생성할 때 기본으로 제공되는 4가지 템플릿을 사용하면 Campaign 데이터베이스에 프로필을 추가 &#x200B;&#x200B;또는 업데이트하고, 고객을 서비스에 구독시키고, 고객의 서비스 구독을 취소하고, 사용자를 옵트아웃하는 등 다양한 사용 사례를 구현할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=ko#create-landing-page" text="랜딩 페이지 만들기"

랜딩 페이지를 적절하게 사용하려면 전용 옵션을 사용하여 메시지의 링크로 참조합니다. 게시된 게재 대시보드에 표시된 링크를 게재 또는 웹 페이지에 직접 복사하여 붙여넣을 수 없습니다. 대신 **콘텐츠 시뮬레이션** 기능을 사용하여 테스트하십시오.

[!DNL Adobe Campaign Web] 인터페이스에서 네 개의 기본 템플릿을 사용하여 다양한 사용 사례를 구현할 수 있습니다. 그러나 주요 단계는 동일하게 유지되며 아래에 자세히 설명되어 있습니다.

1. [랜딩 페이지를 만들고](create-lp.md#create-landing-page) 사용 사례에 따라 선택한 템플릿을 선택합니다.

1. 랜딩 페이지 속성 및 설정을 정의합니다.

   ![랜딩 페이지 속성 및 설정 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-properties.png){zoomable="yes"}

1. 차단 목록에 추가하다 경우에 따라 **[!UICONTROL 획득]**, **[!UICONTROL 구독]**, **[!UICONTROL 구독 취소]** 또는 **[!UICONTROL 구독 취소]** 페이지를 선택하십시오.

1. 페이지의 콘텐츠가 표시됩니다. 랜딩 페이지 양식에 해당하는 부분을 선택합니다.

   ![랜딩 페이지 양식 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-form.png){zoomable="yes"}

1. 선택한 템플릿에 따라 콘텐츠를 편집합니다.

   * [획득](#lp-acquisition)
   * [구독](#lp-subscription)
   * [구독 취소](#lp-unsubscription)
   * [차단 목록에 추가](#lp-denylist)

1. 필요에 따라 나머지 콘텐츠를 수정하고 변경 사항을 저장한 다음 닫습니다.

1. 필요에 따라 **[!UICONTROL 확인]** 페이지와 **[!UICONTROL 오류]** 및 **[!UICONTROL 만료]** 페이지를 편집합니다. 양식을 제출하면 받는 사람에게 **[!UICONTROL 확인]** 페이지가 표시됩니다.

   ![확인 페이지 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. 랜딩 페이지를 [테스트](create-lp.md#test-landing-page) 및 [게시](create-lp.md#publish-landing-page)합니다.

1. [전자 메일](../email/create-email.md) 게재를 만들어 랜딩 페이지로 트래픽을 유도합니다.

1. 메시지 콘텐츠에 [링크 삽입](../email/message-tracking.md#insert-links) **[!UICONTROL 랜딩 페이지]**&#x200B;을(를) **[!UICONTROL 링크 형식]**(으)로 선택하고 만든 랜딩 페이지를 선택합니다.

   ![전자 메일 링크 삽입 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >메시지를 보내려면 선택한 랜딩 페이지가 아직 만료되지 않았는지 확인하십시오. [자세히 알아보기](create-lp.md#create-landing-page)

이메일을 수신하면 수신자가 랜딩 페이지 링크를 클릭하고 양식을 제출하는 경우:

* 확인 페이지로 이동합니다.
* 랜딩 페이지에 정의된 다른 모든 작업이 적용됩니다. 예를 들어 사용자가 서비스에 가입되거나 사용자로부터 더 이상 커뮤니케이션을 받지 않습니다.

다음은 여러 사용 사례에서 [!DNL Adobe Campaign] 랜딩 페이지를 사용하는 방법의 몇 가지 예입니다.

## 프로필 획득 {#lp-acquisition}

첫 번째 템플릿을 사용하면 Campaign 데이터베이스에 프로필을 추가하거나 업데이트할 수 있습니다.

1. [랜딩 페이지를 만들](create-lp.md#create-landing-page) 때 **[!UICONTROL 획득]** 템플릿을 선택합니다.

1. 랜딩 페이지 속성에서 **[!UICONTROL 양식에 참조된 데이터로 미리 채우기]** 옵션을 선택하여 프로필에서 기존 정보를 미리 로드하고 중복을 만들지 않도록 합니다.

1. 콘텐츠를 편집하려면 **[!UICONTROL 획득]** 페이지를 선택하십시오.

1. 프로필에서 수집하려는 정보에 따라 필요에 따라 텍스트 필드를 편집합니다.

1. 고객을 뉴스레터 서비스에 가입하도록 초대하는 확인란을 추가합니다. [서비스를 만드는 방법 알아보기](../audience/manage-services.md)

   ![뉴스레터 구독 확인란이 포함된 획득 페이지 인터페이스를 표시하는 스크린샷입니다.](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. 필요에 따라 콘텐츠를 조정하고 변경 사항을 저장합니다.

1. 랜딩 페이지를 검토하고 [게시](create-lp.md#publish-landing-page)합니다.

1. [이메일](../email/create-email.md)을(를) 만들고 [랜딩 페이지에 링크를 추가](../email/message-tracking.md#insert-links)합니다.

이메일을 수신하면 수신자가 랜딩 페이지 링크를 클릭하고 양식을 제출하면 프로필이 Campaign 데이터베이스에 추가되거나 제공된 정보로 업데이트됩니다.

![Campaign 데이터베이스에서 업데이트된 프로필을 표시하는 스크린샷입니다.](assets/lp-uc-profile-updated.png){zoomable="yes"}

고객이 뉴스레터를 수신하도록 옵트인한 경우 해당 서비스를 구독하게 됩니다.

![뉴스레터 구독 확인을 보여 주는 스크린샷](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## 서비스 구독 {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="구독 랜딩 페이지 설정"
>abstract="고객은 구독 페이지를 통해 서비스를 구독할 수 있습니다."

가장 일반적인 사용 사례 중 하나는 랜딩 페이지를 통해 고객을 [서비스 구독](../audience/manage-services.md)(예: 뉴스레터 또는 이벤트)으로 초대하는 것입니다. 아래 단계를 수행합니다.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. 서비스를 만들 때 이벤트를 쉽게 선택할 수 있도록 이벤트를 구독하는 사용자에 대한 확인 템플릿을 만듭니다. [자세히 알아보기](../audience/manage-services.md#create-confirmation-message)

   ![확인 전자 메일 템플릿 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. 이벤트에 대해 등록된 사용자를 저장하는 구독 서비스를 만듭니다. [서비스를 만드는 방법 알아보기](../audience/manage-services.md)

1. 구독 시 사용자가 받게 되는 확인 이메일로 만든 템플릿을 선택합니다.

   ![구독 서비스 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. 받는 사람이 이벤트에 등록할 수 있도록 [랜딩 페이지를 만듭니다](create-lp.md#create-landing-page). **[!UICONTROL 구독]** 템플릿을 선택하십시오.

1. 콘텐츠를 편집하려면 **[!UICONTROL 구독]** 페이지를 선택하십시오.

1. 페이지의 콘텐츠가 표시됩니다. 랜딩 페이지 양식에 해당하는 부분을 선택하고 **[!UICONTROL 확인란 1]** 섹션을 확장합니다.

1. **[!UICONTROL 구독 및 서비스]** 필드에서 이벤트에 대해 만든 서비스를 선택합니다. **[!UICONTROL 선택한 경우 가입]** 옵션을 사용하도록 설정합니다.

   ![구독 확인란 인터페이스를 표시하는 스크린샷입니다.](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. 필요에 따라 콘텐츠를 조정하고 변경 사항을 저장합니다.

1. 랜딩 페이지를 검토하고 [게시](create-lp.md#publish-landing-page)합니다.

1. 등록 랜딩 페이지로 트래픽을 유도하려면 [전자 메일](../email/create-email.md)을 만들고 [링크를 추가](../email/message-tracking.md#insert-links)하십시오.

1. 이제 이벤트에 대한 등록이 열렸음을 알리는 이메일을 디자인합니다.

이메일을 수신하면 수신자가 랜딩 페이지 링크를 클릭하고 양식을 제출하면 확인 페이지로 이동하여 구독 목록에 추가됩니다.

## 구독 취소 {#lp-unsubscription}

고객은 랜딩 페이지를 사용하여 서비스 구독을 취소할 수 있습니다.

1. 서비스를 만들 때 쉽게 선택할 수 있도록 서비스에서 구독 취소하는 사용자에 대한 확인 템플릿을 만듭니다. [자세히 알아보기](../audience/manage-services.md#create-confirmation-message)

1. [구독 서비스](../audience/manage-services.md)에서 사용자가 구독 취소 시 받게 되는 확인 전자 메일로 만든 템플릿을 선택합니다.

1. [랜딩 페이지 만들기](create-lp.md#create-landing-page). **[!UICONTROL 구독 취소]** 템플릿을 선택하십시오.

1. 콘텐츠를 편집하려면 **[!UICONTROL 구독 취소]** 페이지를 선택하십시오.

1. 페이지의 콘텐츠가 표시됩니다. 랜딩 페이지 양식에 해당하는 부분을 선택합니다.

1. **[!UICONTROL 확인란]** 섹션을 추가하고 서비스를 선택한 다음 **[!UICONTROL 선택한 경우 구독 취소]** 옵션을 선택하십시오.

   ![구독 취소 확인란 인터페이스를 표시하는 스크린샷입니다.](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. **[!UICONTROL 콜 투 액션]** 섹션을 확장하고 **[!UICONTROL 추가 업데이트]** 옵션을 선택합니다. 서비스를 선택하고 **[!UICONTROL 옵트아웃]** 옵션을 선택하십시오.

   ![구독 취소를 위한 call-to-action 인터페이스를 보여주는 스크린샷입니다.](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. 필요에 따라 콘텐츠를 조정하고 변경 사항을 저장합니다.

1. 랜딩 페이지를 검토하고 [게시](create-lp.md#publish-landing-page)합니다.

1. [이메일](../email/create-email.md)을(를) 만들고 [랜딩 페이지에 링크를 추가](../email/message-tracking.md#insert-links)합니다.

이메일을 수신하면 수신자가 랜딩 페이지 링크를 클릭하고 양식을 제출하면 구독 취소 확인 페이지로 이동되고 해당 구독 서비스에서 제거됩니다.

## 차단 목록에 추가 {#lp-denylist}

수신자가 브랜드로부터 커뮤니케이션 수신을 거부할 수 있는 기능을 제공하는 것은 법적 요구 사항입니다. 따라서 수신자에게 보내는 모든 이메일에 항상 **구독 취소 링크**&#x200B;를 포함해야 합니다. 이 링크를 클릭하면 수신자는 옵트아웃을 확인하는 버튼이 포함된 랜딩 페이지로 이동합니다.

사용자가 모든 게재에서 옵트아웃할 수 있도록 **[!UICONTROL 차단 목록]** 랜딩 페이지를 설정할 수 있습니다.

1. [랜딩 페이지를 만들](create-lp.md#create-landing-page) 때 **[!UICONTROL 차단 목록]** 템플릿을 선택합니다.

1. 차단 목록에 추가하다 콘텐츠를 편집하려면 **[!UICONTROL 페이지]**&#x200B;를 선택하십시오.

1. **[!UICONTROL 콜 투 액션]** 섹션을 확장하고 **[!UICONTROL 추가 업데이트]** 옵션을 선택합니다.

1. 해당 드롭다운 목록에서 **[!UICONTROL 채널(이메일)]**&#x200B;을 선택하여 수신자가 이메일 통신에서만 옵트아웃하도록 합니다. 모든 채널의 모든 통신에서 옵트아웃하도록 **[!UICONTROL 모든 채널별]**&#x200B;을 선택할 수도 있습니다.

   차단 목록에 추가하다 ![call-to-action 인터페이스를 보여주는 스크린샷](assets/lp-uc-denylist.png){zoomable="yes"}

1. 필요에 따라 콘텐츠를 조정하고 변경 사항을 저장합니다.

1. 랜딩 페이지를 검토하고 [게시](create-lp.md#publish-landing-page)합니다.

1. 사용자가 커뮤니케이션 수신을 거부할 수 있도록 [이메일](../email/create-email.md)을(를) 만들고 [랜딩 페이지에 링크를 추가](../email/message-tracking.md#insert-links)합니다.

이메일을 수신하면 수신자가 랜딩 페이지 링크를 클릭하고 양식을 제출하면 차단 목록에 추가하다 확인 페이지로 이동되고 프로필이 제공된 정보로 업데이트됩니다.

해당 프로필의 선택 사항이 업데이트되었는지 확인하려면 **[!UICONTROL 프로필]** 메뉴를 찾아 해당 프로필을 선택하십시오.

예를 들어 랜딩 페이지에서 **[!UICONTROL 채널(이메일)]** 옵션을 업데이트하도록 선택한 경우 **[!UICONTROL 더 이상 이메일로 연락하지 않음]** 옵션이 선택됩니다.

차단 목록에 추가하다 ![프로필 기본 설정을 업데이트한 스크린샷 표시](assets/lp-uc-denylist-profile.png){zoomable="yes"}

이 프로필은 다시 구독하지 않으면 브랜드로부터 이메일 통신을 받지 않습니다.