---
audience: end-user
title: 생성 콘텐츠
description: AI Assistant를 사용하여 이미지를 생성하는 방법 알아보기
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 2%

---

# AI Assistant를 사용하여 이미지 생성 {#generative-image}

>[!IMPORTANT]
>
>이 기능의 사용을 시작하기 전에 관련 [보호 기능 및 제한 사항](generative-gs.md#generative-guardrails)을 읽어 보십시오.
></br>
>
>Adobe Campaign 웹에서 AI Assistant를 사용하기 전에 [사용자 계약](https://www.adobe.com/kr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}에 동의해야 합니다. 자세한 내용은 Adobe 담당자에게 문의하세요.

Adobe Campaign 웹의 AI Assistant를 사용하여 이메일, 웹 페이지, 랜딩 페이지 및 푸시 알림 전반에서 메시지를 향상시키는 매력적인 시각적 컨텐츠를 만들 수 있습니다. AI Assistant를 사용하면 이미지를 생성하고 최적화할 수 있으므로 콘텐츠가 시각적으로 매력적이고 브랜드에 맞게 조정됩니다.

## 이메일 및 랜딩 페이지의 경우 {#email-web-channels}

AI Assistant는 이메일 캠페인 및 랜딩 페이지에 대한 완전한 시각적 경험을 생성할 수 있습니다. 이 기능을 사용하면 디지털 터치포인트에서 대상자와 공감하는 온브랜드, 주목을 끄는 이미지를 만들 수 있습니다.

### 액세스 및 구성 {#access-configure}

AI Assistant를 사용하여 이미지 생성을 시작하려면 먼저 게재를 설정하고 콘텐츠 편집기를 엽니다. 아래 단계에 따라 작업 영역을 준비하고 AI Assistant 패널에 액세스합니다.

1. 게재 만들기 및 구성:

   * **전자 메일**: 전자 메일 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요. [자세히 알아보기](../email/create-email-content.md)
   * **랜딩 페이지**: 랜딩 페이지를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요. [자세히 알아보기](../landing-pages/create-lp.md)

1. AI Assistant로 변경할 자산을 선택하고 **[!UICONTROL AI Assistant]** 메뉴에 액세스합니다.

   ![Adobe Campaign 웹에서 텍스트 구성 요소 선택을 보여 주는 스크린샷](assets/image-genai-1.png){zoomable="yes"}

### 콘텐츠 생성 {#generate-content}

1. AI Assistant가 선택한 콘텐츠를 기반으로 새 콘텐츠를 개인화하려면 **[!UICONTROL 참조 스타일]** 옵션을 활성화하십시오.

1. AI 생성 콘텐츠가 브랜드 사양에 맞게 조정되도록 하려면 **[!UICONTROL 브랜드]**&#x200B;를 선택하십시오. 브랜드에 대해 [자세히 알아보기](brands.md).

1. **[!UICONTROL Prompt]** 필드에 생성할 내용을 설명하여 내용을 미세 조정하십시오.

   프롬프트를 만드는 데 도움이 필요한 경우 게재를 개선하기 위한 다양한 프롬프트 아이디어를 제공하는 **[!UICONTROL 프롬프트 라이브러리]**&#x200B;에 액세스하십시오. [프롬프트 모범 사례에 대해 자세히 알아보기](ai-assistant-prompting-guide.md)

   ![Adobe Campaign 웹에서 이미지 생성을 위한 프롬프트 라이브러리를 보여 주는 스크린샷](assets/image-genai-2.png){zoomable="yes"}

1. **[!UICONTROL 이미지 설정]** 옵션을 사용하여 메시지를 사용자 지정합니다.

   * **[!UICONTROL 종횡비]**: 에셋의 너비와 높이를 결정합니다. 16:9, 4:3, 3:2 또는 1:1과 같은 일반적인 비율 중에서 선택하거나 사용자 지정 크기를 입력합니다.
   * **[!UICONTROL 콘텐츠 형식]**: 시각적 요소의 특성을 분류하여 사진, 그래픽 또는 미술과 같은 다양한 시각적 표현 형식을 구분합니다.
   * **[!UICONTROL 시각적 강도]**: 이미지의 강도를 조정하여 이미지의 영향을 제어합니다. 낮은 설정(2)은 더 부드러운 모양을 만들고 높은 설정(10)은 더 밝은 이미지를 만듭니다.
   * **[!UICONTROL 색상 및 색조]**: 전체 색상 모양과 전달한 분위기 또는 분위기를 조정합니다.
   * **[!UICONTROL 조명]**: 이미지의 조명을 수정하여 분위기를 만들고 특정 요소를 강조 표시합니다.
   * **[!UICONTROL 컴포지션]**: 이미지의 프레임 내에 요소를 정렬합니다.

     ![Adobe Campaign 웹에서 이미지 설정 옵션을 보여 주는 스크린샷](assets/image-genai-4.png){zoomable="yes"}

1. **[!UICONTROL 참조 콘텐츠]** 메뉴에서 **[!UICONTROL 파일 업로드]**&#x200B;를 클릭하여 추가 컨텍스트 AI 도우미를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 추가하거나 이전에 업로드한 콘텐츠를 선택합니다.

   이전에 업로드한 파일은 **[!UICONTROL 업로드된 참조 콘텐츠]** 드롭다운에서 사용할 수 있습니다. 세대에 포함할 자산을 전환하기만 하면 됩니다.

1. 프롬프트 구성에 만족하면 **[!UICONTROL 생성]**&#x200B;을 클릭합니다.

### 세분화 및 완료 {#refine-finalize}

1. 생성된 **[!UICONTROL 변형]**&#x200B;을 검색합니다.

1. 백분율 아이콘을 클릭하여 **[!UICONTROL 브랜드 맞춤 점수]**&#x200B;를 보고 브랜드에 대한 모든 오정렬을 식별합니다.

   [브랜드 정렬 점수](../content/brands-score.md)에 대해 자세히 알아보세요.

   ![](assets/image-genai-3.png){zoomable="yes"}

1. 선택한 변형의 전체 화면 버전을 보려면 **[!UICONTROL 미리 보기]**&#x200B;를 클릭하고 현재 콘텐츠를 바꾸려면 **[!UICONTROL 적용]**&#x200B;을 클릭하십시오.

1. 이 변형과 관련된 이미지를 보려면 **[!UICONTROL 유사 항목 생성]**&#x200B;을 선택하십시오.

1. **[!UICONTROL 브랜드 정렬]** 탭을 열어 콘텐츠가 [브랜드 지침](../content/brands.md)에 어떻게 적합한지 확인합니다.

1. 적절한 콘텐츠를 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭합니다.

1. 메시지 콘텐츠를 정의한 후 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인합니다. [자세히 알아보기](../preview-test/preview-content.md)

1. 콘텐츠를 검토하고 활성화합니다.
   * **전자 메일**: 콘텐츠, 대상자 및 일정을 정의했으면 전자 메일 게재를 준비할 준비가 되었습니다. [자세히 알아보기](../monitor/prepare-send.md)
   * **랜딩 페이지**: 랜딩 페이지가 준비되면 이를 게시하여 메시지에 사용할 수 있도록 할 수 있습니다. [자세히 알아보기](../landing-pages/create-lp.md)

## 모바일 채널용 {#mobile-channels}

AI Assistant를 사용하면 푸시 알림 및 SMS 메시지에 대한 매력적인 텍스트를 생성할 수 있으므로 모든 모바일 터치포인트에서 시선을 사로잡으며 대상자와 공감하는 모바일 커뮤니케이션을 생성할 수 있습니다.

### 액세스 및 구성 {#mobile-access-configure}

AI Assistant를 사용하여 모바일 채널에 대한 텍스트 생성을 시작하려면 먼저 게재를 설정하고 AI Assistant를 엽니다. AI Assistant에 액세스하는 단계는 푸시 알림으로 작업하는지 SMS 메시지로 작업하는지에 따라 약간 다릅니다.

1. 모바일 게재를 만들고 구성합니다.

   * **푸시 알림**: 푸시 알림 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요. [자세히 알아보기](../push/create-push.md)
   * **SMS**: SMS 게재를 만들고 구성한 후 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요. [자세히 알아보기](../sms/create-sms.md)

1. 게재할 **[!UICONTROL 기본 세부 정보]**&#x200B;를 입력하십시오. 완료되면 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하세요.

1. 필요에 따라 메시지를 개인화합니다.

   * **푸시 알림**: [자세히 알아보기](../push/content-push.md)
   * **SMS**: [자세히 알아보기](../sms/content-sms.md)

1. **[!UICONTROL AI Assistant 표시]** 메뉴에 액세스합니다.

   ![AI Assistant 메뉴 표시를 보여주는 스크린샷](assets/push-img-1.png){zoomable="yes"}

### 콘텐츠 생성 {#mobile-generate-content}

AI Assistant에 액세스한 후 생성 설정을 조정하여 내 브랜드에 맞는 이미지를 만들고 목표를 지원할 수 있습니다.

1. AI 생성 콘텐츠가 브랜드 사양에 맞게 조정되도록 하려면 **[!UICONTROL 브랜드]**&#x200B;를 선택하십시오. 브랜드에 대해 [자세히 알아보기](brands.md).

1. **[!UICONTROL 프롬프트]** 필드에 생성할 내용을 설명하여 내용을 미세 조정하십시오.

   프롬프트 작성에 도움이 필요한 경우 캠페인을 개선하기 위한 다양한 프롬프트 아이디어를 제공하는 **[!UICONTROL 프롬프트 라이브러리]**&#x200B;에 액세스하십시오. [프롬프트 모범 사례에 대해 자세히 알아보기](ai-assistant-prompting-guide.md)

   ![프롬프트 필드 및 옵션이 있는 AI 길잡이](assets/push-img-2.png){zoomable="yes"}

1. 에셋만 생성하려면 **[!UICONTROL 이미지]**&#x200B;를 선택하십시오.

1. **[!UICONTROL 이미지 설정]** 선택:

   * **[!UICONTROL 콘텐츠 형식]**: 시각적 요소의 특성을 분류하여 사진, 그래픽 또는 미술과 같은 다양한 시각적 표현 형식을 구분합니다.
   * **[!UICONTROL 시각적 강도]**: 이미지의 강도를 조정하여 이미지의 영향을 제어합니다. 낮은 설정 (2)는 부드럽고 절제된 모양을 만들고, 높은 설정 (10)은 이미지를 더 생동감 있고 시각적으로 강력하게 만듭니다.
   * **[!UICONTROL 조명]**: 이미지의 조명을 조정하여 분위기를 만들고 특정 요소를 강조 표시합니다.
   * **[!UICONTROL 컴포지션]**: 이미지의 프레임 내에 요소를 정렬합니다.

     ![이미지 설정 옵션을 보여 주는 스크린샷](assets/push-img-3.png){zoomable="yes"}

1. **[!UICONTROL 참조 콘텐츠]** 메뉴에서 **[!UICONTROL 파일 업로드]**&#x200B;를 클릭하여 추가 컨텍스트 AI 도우미를 제공할 수 있는 콘텐츠가 포함된 브랜드 자산을 추가하거나 이전에 업로드한 콘텐츠를 선택합니다.

   이전에 업로드한 파일은 **[!UICONTROL 업로드된 참조 콘텐츠]** 드롭다운에서 사용할 수 있습니다. 세대에 포함할 자산을 전환하기만 하면 됩니다.

1. 메시지가 준비되면 **[!UICONTROL 생성]**&#x200B;을 클릭합니다.

### 세분화 및 완료 {#mobile-refine-finalize}

모바일 메시지에 대한 이미지 변형을 생성한 후 결과를 미세 조정하여 정확한 요구 사항을 충족할 수 있습니다.

1. 생성 후 **[!UICONTROL 변형]**&#x200B;을 살펴보십시오.

1. 백분율 아이콘을 클릭하여 **[!UICONTROL 브랜드 맞춤 점수]**&#x200B;를 보고 브랜드에 대한 모든 오정렬을 식별합니다.

   [브랜드 정렬 점수](../content/brands-score.md)에 대해 자세히 알아보세요.

   ![](assets/push-img-4.png){zoomable="yes"}

1. **[!UICONTROL 미리 보기]**&#x200B;를 클릭하여 **[!UICONTROL 변형]**&#x200B;을(를) 살펴봅니다.

1. **[!UICONTROL 브랜드 정렬]** 탭을 열어 콘텐츠가 [브랜드 지침](brands.md)에 어떻게 적합한지 확인합니다.

1. 적절한 콘텐츠를 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭합니다.

콘텐츠, 대상 및 일정을 정의했으면 푸시 게재를 준비합니다. [자세히 알아보기](../monitor/prepare-send.md)
