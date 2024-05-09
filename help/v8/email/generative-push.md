---
audience: end-user
title: Campaign에서 AI 도우미를 사용한 푸시 알림
description: Campaign에서 AI Assistant 시작
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 10%

---

# AI 어시스턴트로 푸시 알림 생성 {#generative-push}

>[!BEGINSHADEBOX]

**목차**

* [AI 어시스턴트 시작하기](generative-gs.md)
* [AI 어시스턴트로 이메일 생성](generative-content.md)
* [AI 어시스턴트와 함께하는 SMS 세대](generative-sms.md)
* AI 어시스턴트로 푸시 알림 생성

>[!ENDSHADEBOX]

AI 도우미는 대상자에게 반향을 일으킬 가능성이 높은 다양한 콘텐츠를 제안하여 게재의 영향을 최적화하는 데 도움이 됩니다.

>[!NOTE]
>
>이 기능의 사용을 시작하기 전에 관련 항목을 읽어 보십시오. [보호 및 제한 사항](generative-gs.md#generative-guardrails).

다음 예에서는 AI Assistant를 활용하여 보다 매력적인 고객 경험을 구축하기 위해 매력적인 메시지를 작성하겠습니다.

1. 푸시 알림 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**.

   푸시 게재를 구성하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [이 페이지](../push/create-push.md).

1. 다음을 입력합니다. **[!UICONTROL 기본 세부 정보]** 게재를 위해. 완료되면 다음을 클릭합니다. **[!UICONTROL 콘텐츠 편집]**.

1. 필요에 따라 푸시 알림을 개인화합니다. [자세히 알아보기](../push/content-push.md)

1. 액세스 **[!UICONTROL AI Assistant 표시]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. 활성화 **[!UICONTROL 원본 컨텐츠 사용]** ai 비서가 게재, 게재명 및 선택한 대상자를 기반으로 새 콘텐츠를 개인화할 수 있는 옵션.

   >[!IMPORTANT]
   >
   > 프롬프트는 항상 현재 콘텐츠에 연결되어야 합니다.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. 에서 생성하려는 내용을 설명하여 콘텐츠를 미세 조정합니다. **[!UICONTROL 프롬프트]** 필드.

   메시지를 작성하는 데 도움이 필요한 경우 **[!UICONTROL 프롬프트 라이브러리]** 게재를 개선하기 위한 다양한 신속한 아이디어를 제공합니다.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. 선택 **[!UICONTROL 브랜드 자산 업로드]** 추가 컨텍스트를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 AI Assistant에 추가합니다.

1. 생성할 필드 선택: **[!UICONTROL 제목]**, **[!UICONTROL 부제]** 또는 **[!UICONTROL 메시지]**.

1. 프롬프트를 다음과 같은 다양한 옵션으로 사용자 지정합니다.

   * **[!UICONTROL 커뮤니케이션 전략]**: 생성된 텍스트에 가장 적합한 커뮤니케이션 스타일을 선택합니다.
   * **[!UICONTROL 언어]**: 콘텐츠를 생성할 언어를 선택합니다.
   * **[!UICONTROL 톤]**: 이메일의 톤은 대상자에게 울려 퍼져야 합니다. AI 어시스턴트는 여러분이 유익하거나, 장난스럽거나, 설득력 있게 들리기를 원하든 상관없이 메시지를 그에 따라 조정할 수 있습니다.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. 프롬프트가 준비되면 다음을 클릭합니다. **[!UICONTROL 생성]**.

1. 생성된 를 통해 찾아보기 **[!UICONTROL 변형]** 및 클릭 **[!UICONTROL 미리 보기]** 선택한 변형의 전체 화면 버전을 보려면 다음과 같이 하십시오.

1. 다음 위치로 이동 **[!UICONTROL 세부 조정]** 내의 옵션 **[!UICONTROL 미리 보기]** 추가 사용자 지정 기능에 액세스하기 위한 창:

   * **[!UICONTROL 참조 콘텐츠로 사용]**: 선택한 변형은 다른 결과를 생성하기 위한 참조 콘텐츠 역할을 합니다.

   * **[!UICONTROL 구문 변경]**: AI Assistant는 다양한 방식으로 메시지를 고쳐 써서 다양한 대상자를 유혹할 수 있습니다.

   * **[!UICONTROL 더 간결한 언어 사용]**: AI Assistant를 사용하여 언어를 단순화함으로써, 보다 많은 대상자가 명확하고 쉽게 사용할 수 있습니다.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. 클릭 **[!UICONTROL 선택]** 적절한 콘텐츠를 찾았으면

1. 개인화 필드를 삽입하여 프로필 데이터를 기반으로 이메일 콘텐츠를 사용자 정의합니다. 그런 다음 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다. [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

콘텐츠, 대상 및 일정을 정의했으면 푸시 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)

