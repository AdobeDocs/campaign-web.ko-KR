---
audience: end-user
title: Campaign의 AI Assistant를 사용한 SMS
description: Campaign에서 AI Assistant 시작
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 9%

---

# AI 어시스턴트와 함께하는 SMS 세대 {#generative-sms}

>[!BEGINSHADEBOX]

**목차**

* [AI 어시스턴트 시작하기](generative-gs.md)
* [AI 어시스턴트로 이메일 생성](generative-content.md)
* AI 어시스턴트와 함께하는 SMS 세대
* [AI 어시스턴트로 푸시 알림 생성](generative-push.md)

>[!ENDSHADEBOX]

대상자에 맞게 SMS 메시지를 만들고 개인화한 후에는 혁신적인 AI 기술을 기반으로 하는 Campaign의 AI Assistant를 통해 다음 단계로 커뮤니케이션을 수행합니다.

이 편리한 도구는 콘텐츠를 세분화하기 위한 지능적인 제안을 제공하여 메시지가 효과적으로 울리고 참여를 극대화할 수 있도록 합니다.

>[!NOTE]
>
>이 기능의 사용을 시작하기 전에 관련 [보호 기능 및 제한 사항](generative-gs.md#generative-guardrails)을 읽어 보십시오.

1. SMS 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요.

   SMS 게재를 구성하는 방법에 대한 자세한 내용은 [이 페이지](../sms/create-sms.md)를 참조하세요.

1. 게재할 **[!UICONTROL 기본 세부 정보]**&#x200B;를 입력하십시오. 완료되면 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요.

1. 필요에 따라 SMS 메시지를 개인화합니다. [자세히 알아보기](../sms/content-sms.md)

1. **[!UICONTROL AI Assistant 표시]** 메뉴에 액세스합니다.

   ![](assets/sms-genai-1.png){zoomable="yes"}

1. AI 관리자가 **[!UICONTROL 원본 콘텐츠 사용]** 옵션을 사용하여 게재, 게재 이름 및 선택한 대상을 기반으로 새 콘텐츠를 개인화할 수 있습니다.

   >[!IMPORTANT]
   >
   > 프롬프트는 항상 현재 콘텐츠에 연결되어야 합니다.

1. **[!UICONTROL 프롬프트]** 필드에 생성할 내용을 설명하여 내용을 미세 조정하십시오.

   프롬프트 작성에 도움이 필요한 경우 게재 개선을 위한 다양한 프롬프트 아이디어를 제공하는 **[!UICONTROL 프롬프트 라이브러리]**&#x200B;에 액세스하십시오.

   ![](assets/sms-genai-2.png){zoomable="yes"}

1. AI Assistant에 추가 컨텍스트를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 추가하려면 **[!UICONTROL 브랜드 자산 업로드]**&#x200B;를 선택하십시오.

1. 프롬프트를 다음과 같은 다양한 옵션으로 사용자 지정합니다.

   * **[!UICONTROL 통신 전략]**: 생성된 텍스트에 대해 원하는 통신 접근 방식을 선택하십시오.
   * **[!UICONTROL 언어]**: 변형 콘텐츠의 언어를 선택하십시오.
   * **[!UICONTROL 색조]**: 텍스트가 대상자와 목적에 적합한지 확인하십시오.
   * **[!UICONTROL 길이]**: 범위 슬라이더를 사용하여 콘텐츠의 길이를 선택합니다.

   ![](assets/sms-genai-3.png){zoomable="yes"}

1. 메시지가 준비되면 **[!UICONTROL 생성]**&#x200B;을 클릭합니다.

1. 생성된 **[!UICONTROL 변형]**&#x200B;을 찾은 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭하여 선택한 변형의 전체 화면 버전을 봅니다.

1. **[!UICONTROL 미리 보기]** 창 내에서 **[!UICONTROL 세분화]** 옵션으로 이동하여 추가 사용자 지정 기능에 액세스하고 변형을 환경 설정에 맞게 세부 조정하십시오.

   * **[!UICONTROL 참조 콘텐츠로 사용]**: 선택한 변형이 다른 결과를 생성하기 위한 참조 콘텐츠로 사용됩니다.

   * **[!UICONTROL 간단한 언어 사용]**: AI 도우미는 모든 사람이 이해할 수 있는 명확하고 간결한 메시지를 작성할 수 있도록 도와줍니다.

   * **[!UICONTROL 구문 바꾸기]**: AI 도우미는 다른 대상자에게 흥미를 계속 주기 위해 메시지를 다시 구문 분석합니다.

   ![](assets/sms-genai-4.png){zoomable="yes"}

1. 적절한 콘텐츠를 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭합니다.

1. 개인화 필드를 삽입하여 프로필 데이터를 기반으로 SMS 콘텐츠를 사용자 지정합니다. [콘텐츠 개인화에 대해 자세히 알아보기](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable="yes"}

1. 메시지 콘텐츠를 정의한 후 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다. [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable="yes"}

콘텐츠, 대상자 및 일정을 정의했으면 SMS 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)
