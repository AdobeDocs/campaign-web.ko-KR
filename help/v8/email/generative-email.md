---
audience: end-user
title: Campaign에서 AI Assistant를 사용하여 이메일 생성
description: Campaign에서 AI Assistant 시작
badge: label="Alpha"
exl-id: f6c9c940-ae85-44e6-a23e-9133df87e67e
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 2%

---

# AI Assistant를 사용하여 이메일 생성 {#generative-email}

Campaign의 AI Assistant는 전체 이메일 콘텐츠를 자동으로 생성하여 시간을 절약하고 일관된 품질을 보장함으로써 커뮤니케이션의 영향을 강화합니다. 생성형 AI를 사용하면 대상자와 공감하는 매력적인 이메일을 손쉽게 제작하여 커뮤니케이션을 보다 효과적이고 효율적으로 수행할 수 있습니다.

>[!NOTE]
>
>이 기능의 사용을 시작하기 전에 관련 [보호 기능 및 제한 사항](generative-gs.md#guardrails-and-limitations)을 읽어 보십시오.


AI Assistant를 사용하여 이메일 콘텐츠를 생성하려면 아래 단계를 수행합니다. [이 페이지](generative-content.md)에 설명된 대로 AI 도우미를 사용하여 기존 콘텐츠를 개선할 수도 있습니다.

1. 전자 메일 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 만들기]**&#x200B;를 클릭합니다.

   전자 메일 게재를 구성하는 방법에 대한 자세한 내용은 [이 페이지](../email/create-email-content.md)를 참조하세요.

1. 게재할 **[!UICONTROL 기본 세부 정보]**&#x200B;를 입력하십시오. 완료되면 **[!UICONTROL 전자 메일 본문 편집]**&#x200B;을 클릭하세요.

1. 생성된 이메일의 기반으로 AI 비서가 사용할 디자인 템플릿을 선택합니다.

   HTML 파일을 가져올 수도 있습니다.

1. 오른쪽 메뉴에서 **[!UICONTROL 경험 생성]**&#x200B;을 선택합니다.

   ![](assets/email-genai-1.png){zoomable="yes"}

1. 생성하려는 내용을 설명하여 콘텐츠를 미세 조정합니다.

   다음은 몇 가지 프롬프트 예입니다.

   * 뉴스레터: 여행 기사, 목적지 하이라이트 및 전용 가입자 오퍼를 제공하는 월간 뉴스레터를 생성합니다.
   * 피드백 및 설문 조사: 고객이 최근 소프트웨어 경험에 대한 피드백을 제공하고 제품 개선 설문 조사에 참여할 수 있도록 초대하는 이메일을 만듭니다.
   * 기념일 또는 생일 이메일의 경우: 생일 이메일을 생성하여 고객의 특별한 날을 축하하고 생일 할인을 제공합니다.

   ![](assets/email-genai-2.png){zoomable="yes"}

1. AI Assistant에 추가 컨텍스트를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 추가하려면 **[!UICONTROL 파일 업로드]**&#x200B;를 선택하십시오.

   **[!UICONTROL 업로드된 콘텐츠]**&#x200B;를 클릭하여 이전에 업데이트된 파일을 찾을 수도 있습니다. 업로드된 콘텐츠는 현재 사용자만 재사용할 수 있습니다.

1. 필요에 가장 적합한 **[!UICONTROL 커뮤니케이션 전략]**&#x200B;을 선택하세요. 생성된 이메일의 색조와 스타일에 영향을 줍니다.

1. 생성된 텍스트에 포함할 **[!UICONTROL 언어]** 및 **[!UICONTROL 색조]**&#x200B;을(를) 선택하십시오. 이렇게 하면 텍스트가 대상자와 목적에 맞게 조정됩니다.

   ![](assets/email-genai-3.png){zoomable="yes"}

1. 원하는 자산 특성에 맞게 **[!UICONTROL 콘텐츠 형식]** 자산 설정을 사용자 지정합니다.

1. 메시지가 준비되면 **[!UICONTROL 생성]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 변형 제안]**&#x200B;을 찾아 원하는 전자 메일을 찾습니다. 선택한 변형의 전체 화면 버전을 보려면 **[!UICONTROL 미리 보기]**&#x200B;를 클릭하십시오.

   ![](assets/email-genai-4.png){zoomable="yes"}

1. 적절한 콘텐츠를 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭합니다.

   ![](assets/email-genai-5.png){zoomable="yes"}

1. 개인화 필드를 삽입하여 프로필 데이터를 기반으로 이메일 콘텐츠를 사용자 정의하거나 필요한 경우 콘텐츠를 추가로 개인화합니다. [콘텐츠 개인화에 대해 자세히 알아보기](../personalization/personalize.md)

1. 전자 메일 콘텐츠를 정의한 후 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다.  [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/email-genai-6.png){zoomable="yes"}

1. 콘텐츠, 대상자 및 일정을 정의했으면 이메일 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)
