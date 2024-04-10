---
audience: end-user
title: Campaign에서 AI 도우미를 사용한 푸시 알림
description: Campaign에서 AI Assistant 시작
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 886fd47b52d08b0a1bfcbeca03929d48b5bc2a3f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 7%

---

# AI Assistant를 사용하여 푸시 알림 생성 {#generative-push}

>[!BEGINSHADEBOX]

**목차**

* [AI 어시스턴트 시작하기](generative-gs.md)
* [AI Assistant를 사용하여 이메일 생성](generative-content.md)
* [AI Assistant를 사용하여 SMS 생성](generative-sms.md)
* **[AI Assistant를 사용하여 푸시 알림 생성](generative-push.md)**

>[!ENDSHADEBOX]

이메일을 만들고 개인화한 후에는 생성 AI에서 제공하는 Campaign의 AI Assistant를 사용하여 콘텐츠를 한 차원 끌어올리십시오.

AI 도우미는 대상자에게 반향을 일으킬 가능성이 높은 다양한 콘텐츠를 제안하여 게재의 영향을 최적화하는 데 도움이 됩니다.

>[!NOTE]
>
>이 기능의 사용을 시작하기 전에 관련 항목을 읽어 보십시오. [보호 및 제한 사항](generative-gs.md#guardrails-and-limitations).

1. 푸시 알림 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**.

   푸시 게재를 구성하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [이 페이지](../push/create-push.md).

1. 다음을 입력합니다. **[!UICONTROL 기본 세부 정보]** 게재를 위해. 완료되면 다음을 클릭합니다. **[!UICONTROL 콘텐츠 편집]**.

1. 필요에 따라 푸시 알림을 개인화합니다. [자세히 알아보기](../push/content-push.md)

1. 액세스 **[!UICONTROL AI Assistant 표시]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. 에서 생성하려는 내용을 설명하여 콘텐츠를 미세 조정합니다. **[!UICONTROL 프롬프트]** 필드.

   메시지를 작성하는 데 도움이 필요한 경우 **[!UICONTROL 프롬프트 라이브러리]** 게재를 개선하기 위한 다양한 신속한 아이디어를 제공합니다.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. 활성화 **[!UICONTROL 현재 컨텍스트로 개선]** ai 비서가 게재, 게재명 및 선택한 대상자를 기반으로 새 콘텐츠를 개인화할 수 있는 옵션.

   >[!IMPORTANT]
   >
   > 브랜드 자산을 업로드하거나 를 활성화하여 프롬프트를 항상 특정 컨텍스트에 연결해야 합니다. **[!UICONTROL 현재 콘텐츠 향상]** 옵션을 선택합니다.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. 선택 **[!UICONTROL 브랜드 자산 업로드]** 추가 컨텍스트를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 AI Assistant에 추가합니다.

1. 생성할 필드 선택: **[!UICONTROL 제목]**, **[!UICONTROL 부제]** 또는 **[!UICONTROL 메시지]**.

1. 다음 항목 선택 **[!UICONTROL 커뮤니케이션 전략]** 그것은 너의 요구에 가장 잘 맞는다. 생성된 텍스트의 색조와 스타일에 영향을 줍니다.

1. 다음을 선택합니다. **[!UICONTROL 언어]** 및 **[!UICONTROL 톤]** 생성된 텍스트에 포함할 텍스트입니다. 이렇게 하면 텍스트가 대상자와 목적에 맞게 조정됩니다.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. 프롬프트가 준비되면 다음을 클릭합니다. **[!UICONTROL 생성]**.

1. 생성된 를 통해 찾아보기 **[!UICONTROL 변형]** 및 클릭 **[!UICONTROL 적용]** 적절한 콘텐츠를 찾았으면

   클릭 **[!UICONTROL 미리 보기]** 선택한 변형의 전체 화면 버전을 보려면 다음과 같이 하십시오.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. 개인화 필드를 삽입하여 프로필 데이터를 기반으로 푸시 콘텐츠를 사용자 지정합니다. [콘텐츠 개인화에 대해 자세히 알아보기](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. 메시지 콘텐츠를 정의한 후 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다. [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. 콘텐츠, 대상 및 일정을 정의했으면 푸시 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)
