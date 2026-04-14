---
audience: end-user
title: WhatsApp 게재 만들기
description: Adobe Campaign 웹 사용자 인터페이스에서 WhatsApp 게재를 만드는 방법을 알아봅니다
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
source-git-commit: aa1a7c48d1708e73e4d6c6bbe4decd2e5ca69102
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 3%

---


# WhatsApp 메시지 만들기 {#create-whatsapp}

**Adobe Campaign 웹 사용자 인터페이스**&#x200B;를 통해 Meta에서 승인한 템플릿을 사용하는 WhatsApp 메시지를 디자인하고 각 프로필에 맞게 개인화하고 보내기 전에 테스트해 볼 수 있습니다.


+++ 지원되는 메시지 요소 및 작업에 대한 호출에 대해 자세히 알아보기

WhatsApp에서는 다음 메시지 유형이 지원됩니다.

| 메시지 기능 | 설명 |
|-|-|
| 헤더 | 메시지 본문 위에 표시되는 선택적 텍스트입니다. |
| 텍스트 | 매개 변수를 통해 다이내믹 콘텐츠를 지원합니다. |
| 헤더 이미지 | 메시지 본문 위에 표시되는 선택적 이미지입니다. |
| 본문 | 매개 변수를 통해 다이내믹 콘텐츠를 지원합니다. |
| 바닥글 텍스트 | 매개 변수를 통해 다이내믹 콘텐츠를 지원합니다. |

+++


## WhatsApp 게재 만들기 {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>WhatsApp 메시지 피드백은 현재 지원되지 않습니다.

Adobe Campaign 웹 사용자 인터페이스에서 아래 단계에 따라 독립 실행형 WhatsApp 게재를 만듭니다.

1. **[!UICONTROL 게재]** 메뉴로 이동한 다음 **[!UICONTROL 게재 만들기]**&#x200B;를 클릭합니다.

   ![](assets/whatsapp-create-1.png)

1. **[!UICONTROL WhatsApp]**&#x200B;을(를) 선택하고 게재 템플릿을 선택하십시오. [템플릿에 대해 자세히 알아보기](../msg/delivery-template.md).

   ![](assets/whatsapp-create-2.png)

1. 확인하려면 **[!UICONTROL 게재 만들기]**&#x200B;를 클릭하세요.

1. 템플릿에 연결된 고급 옵션을 보려면 **[!UICONTROL 설정]**&#x200B;을 클릭하세요. [자세히 알아보기](../advanced-settings/delivery-settings.md)

   ![](assets/whatsapp-create-3.png)

1. 게재할 **[!UICONTROL 레이블]**&#x200B;을(를) 입력하십시오. 내부 이름, 폴더, 게재 코드, 설명 또는 특성, 다른 채널과 동일한 패턴이 필요한 경우 **[!UICONTROL 추가 옵션]**&#x200B;을 사용하십시오.

1. 기존 대상을 타깃팅하거나 만들려면 **[!UICONTROL 대상 선택]**&#x200B;을 클릭하세요. [대상자에 대해 자세히 알아보기](../audience/about-recipients.md).

1. **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하여 WhatsApp 콘텐츠 편집기를 엽니다. [WhatsApp 콘텐츠 정의](#whatsapp-content)를 참조하십시오.

   ![](assets/whatsapp-create-4.png)

1. 특정 날짜 및 시간에 보낼 수 있도록 **[!UICONTROL 일정 조정 사용]**&#x200B;을 설정할 수 있습니다. [자세히 알아보기](../msg/gs-deliveries.md#gs-schedule).


## WhatsApp 콘텐츠 정의{#whatsapp-content}

>[!BEGINSHADEBOX]

Adobe Campaign 웹 사용자 인터페이스에서 WhatsApp 메시지를 디자인하기 전에 Meta에서 템플릿을 만들고 제출하십시오. [자세히 알아보기](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

사용하기 전에 Meta에서 WhatsApp 템플릿을 승인해야 합니다. 승인은 종종 몇 시간이 걸리지만 최대 24시간이 소요될 수 있습니다. [자세히 알아보기](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. Adobe Campaign 웹 사용자 인터페이스의 게재 구성 페이지에서 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하여 WhatsApp 메시지를 구성합니다.

1. 마케팅을 **템플릿 범주**(으)로 선택:

   [템플릿 범주에 대해 자세히 알아보기](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

   ![](assets/whatsapp-design-1.png)

1. **WhatsApp 템플릿** 드롭다운에서 Meta 승인 템플릿을 선택합니다.

   [WhatsApp 템플릿을 만드는 방법에 대해 자세히 알아보기](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

   ![](assets/whatsapp-design-2.png)

1. Meta 승인 템플릿에 이미지가 포함된 경우 **[!UICONTROL 이미지 URL]**&#x200B;을(를) 제공하십시오.

   ![](assets/whatsapp-design-3.png)

1. **Personalization 자리 표시자** 필드에서 개인화 편집기를 사용하여 프로필 필드 및 표현식을 템플릿 매개 변수에 매핑합니다. [자세히 알아보기](../personalization/personalize.md).

   ![](assets/whatsapp-design-4.png)

메시지가 준비되면:

* **독립 실행형 또는 캠페인 게재**: 게재 대시보드에서 **[!UICONTROL 검토 및 보내기]** 및 **[!UICONTROL 보내기]**&#x200B;를 사용합니다.

* **워크플로우**: 실행에서 게재를 사용할 수 있게 되면 워크플로우 활동에서 게재를 연 다음 동일한 방식으로 게재 대시보드를 사용합니다. [자세히 알아보기](../workflows/start-monitor-workflows.md)

그런 다음 게재 **[!UICONTROL 보고서]** 진입점 및 [게재 보고](../reporting/delivery-reports.md)의 결과를 추적할 수 있습니다.
