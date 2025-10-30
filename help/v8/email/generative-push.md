---
audience: end-user
title: AI Assistant를 사용하여 푸시 알림
description: AI 어시스턴트 시작
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 2%

---

# AI Assistant를 사용하여 푸시 알림 생성 {#generative-push}

>[!IMPORTANT]
>
>이 기능의 사용을 시작하기 전에 관련 [보호 기능 및 제한 사항](generative-gs.md#generative-guardrails)을 읽어 보십시오.
>></br>
>
>Adobe Campaign 웹에서 AI Assistant를 사용하기 전에 [사용자 계약](https://www.adobe.com/kr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)에 동의해야 합니다. 자세한 내용은 Adobe 담당자에게 문의하세요.

AI Assistant는 대상자에게 반향을 일으키는 다양한 콘텐츠를 제안하여 게재의 영향을 최적화하는 데 도움이 됩니다.

다음 예에서는 AI Assistant를 활용하여 보다 매력적인 고객 경험을 구축하기 위해 매력적인 메시지를 작성합니다.

1. 푸시 알림 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭합니다.

   푸시 게재 구성에 대한 자세한 내용은 [이 페이지](../push/create-push.md)를 참조하세요.

1. **[!UICONTROL AI Assistant 표시]** 메뉴에 액세스합니다.

   ![AI Assistant 메뉴 표시를 보여주는 스크린샷](assets/push-genai-1.png){zoomable="yes"}

1. AI 관리자가 선택한 콘텐츠를 기반으로 새 콘텐츠를 개인화하려면 **[!UICONTROL 원본 콘텐츠 사용]** 옵션을 사용하도록 설정하십시오.

1. **[!UICONTROL Prompt]** 필드에 생성할 내용을 설명하여 내용을 미세 조정하십시오.

   프롬프트를 만드는 데 도움이 필요한 경우 게재를 개선하기 위한 다양한 프롬프트 아이디어를 제공하는 **[!UICONTROL 프롬프트 라이브러리]**&#x200B;에 액세스하십시오.

   ![프롬프트 라이브러리 인터페이스를 보여주는 스크린샷](assets/push-genai-2.png){zoomable="yes"}

1. 생성할 필드 선택: **[!UICONTROL 제목]**, **[!UICONTROL 자막]**, **[!UICONTROL 메시지]** 및/또는 **[!UICONTROL 이미지]**.

1. **[!UICONTROL 텍스트 설정]** 옵션을 사용하여 메시지를 사용자 지정합니다.

   * **[!UICONTROL 커뮤니케이션 전략]**: 생성된 텍스트에 가장 적합한 커뮤니케이션 스타일을 선택합니다.
   * **[!UICONTROL 음색]**: 대상자와 공감할 수 있도록 전자 메일의 음색을 조정합니다. AI Assistant는 유익하거나, 유쾌하거나, 설득력 있게 들리고자 할 때 메시지를 적절히 조정합니다.

   ![텍스트 설정 옵션을 보여 주는 스크린샷](assets/push-genai-3.png){zoomable="yes"}

1. **[!UICONTROL 이미지 설정]** 선택:

   * **[!UICONTROL 콘텐츠 형식]**: 시각적 요소의 특성을 분류하여 사진, 그래픽 또는 미술과 같은 다양한 시각적 표현 형식을 구분합니다.
   * **[!UICONTROL 시각적 강도]**: 이미지의 강도를 조정하여 이미지의 영향을 제어합니다. 낮은 설정 (2)는 부드럽고 절제된 모양을 만들고, 높은 설정 (10)은 이미지를 더 생동감 있고 시각적으로 강력하게 만듭니다.
   * **[!UICONTROL 조명]**: 이미지의 조명을 조정하여 분위기를 만들고 특정 요소를 강조 표시합니다.
   * **[!UICONTROL 컴포지션]**: 이미지의 프레임 내에 요소를 정렬합니다.

   ![이미지 설정 옵션을 보여 주는 스크린샷](assets/push-genai-4.png){zoomable="yes"}

1. **[!UICONTROL 브랜드 에셋]** 메뉴에서 **[!UICONTROL 브랜드 에셋 업로드]**&#x200B;를 클릭하여 추가 컨텍스트를 제공하는 콘텐츠가 포함된 브랜드 에셋을 AI Assistant에 추가하거나 이전에 업로드한 에셋을 선택합니다.

   이전에 업로드한 파일은 **[!UICONTROL 업로드된 브랜드 자산]** 드롭다운에서 사용할 수 있습니다. 세대에 포함할 자산을 전환합니다.

1. 메시지가 준비되면 **[!UICONTROL 생성]**&#x200B;을 클릭합니다.

1. 생성된 **[!UICONTROL 변형]**&#x200B;을 찾은 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭하여 선택한 변형의 전체 화면 버전을 보거나 **[!UICONTROL 적용]**&#x200B;을 클릭하여 현재 콘텐츠를 바꿉니다.

1. 백분율 아이콘을 클릭하여 **[!UICONTROL 브랜드 맞춤 점수]**&#x200B;를 보고 브랜드에 대한 모든 오정렬을 식별합니다.

   [브랜드 정렬 점수](../content/brands-score.md)에 대해 자세히 알아보세요.

   ![](assets/push-genai-6.png){zoomable="yes"}

1. 추가 사용자 지정 기능에 액세스하려면 **[!UICONTROL 미리 보기]** 창 내에서 **[!UICONTROL 다시 정의]** 옵션으로 이동하십시오.

   * **[!UICONTROL 참조 콘텐츠로 사용]**: 다른 결과를 생성하기 위해 선택한 변형을 참조 콘텐츠로 사용합니다.
   * **[!UICONTROL 구문 변경]**: 다양한 대상자가 쉽고 재미있게 쓸 수 있도록 메시지를 다른 방법으로 다시 기술합니다.
   * **[!UICONTROL 더 간단한 언어 사용]**: 언어를 단순화하여 더 많은 대상자가 명확하고 쉽게 사용할 수 있도록 합니다.

   텍스트의 **[!UICONTROL 색조]** 및 **[!UICONTROL 통신 전략]**&#x200B;을 변경할 수도 있습니다.

   ![세부 조정 옵션을 보여 주는 스크린샷](assets/push-genai-5.png){zoomable="yes"}

1. **[!UICONTROL 브랜드 정렬]** 탭을 열어 콘텐츠가 [브랜드 지침](../content/brands.md)에 어떻게 적합한지 확인합니다.

1. 적절한 콘텐츠를 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭합니다.

1. 개인화 필드를 삽입하여 프로필 데이터를 기반으로 이메일 콘텐츠를 사용자 지정합니다. 그런 다음 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다. [자세히 알아보기](../preview-test/preview-content.md)

콘텐츠, 대상 및 일정을 정의하면 푸시 게재를 준비합니다. [자세히 알아보기](../monitor/prepare-send.md)