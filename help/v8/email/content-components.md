---
audience: end-user
title: 이메일 디자이너 콘텐츠 구성 요소 사용
description: 이메일에 콘텐츠 구성 요소를 사용하는 방법 알아보기
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: 5b984089ea36b190cde1046c0d96734e848b5f67
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 64%

---

# 콘텐츠 구성 요소 사용 {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="콘텐츠 정보"
>abstract="콘텐츠 구성 요소는 이메일 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="콘텐츠 정보"
>abstract="콘텐츠 구성 요소는 랜딩 페이지 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="콘텐츠 정보"
>abstract="콘텐츠 구성 요소는 콘텐츠 조각 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="콘텐츠 정보"
>abstract="콘텐츠 구성 요소는 템플릿 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

전자 메일 콘텐츠를 만들 때 **[!UICONTROL 콘텐츠]** 구성 요소를 사용하면 전자 메일에 배치한 후 사용할 수 있는 비어 있는 원시 구성 요소를 사용하여 전자 메일을 추가로 개인화할 수 있습니다.

전자 메일 레이아웃을 정의하는 **[!UICONTROL 구조]** 내에 필요한 만큼 **[!UICONTROL 콘텐츠]**&#x200B;를 추가할 수 있습니다.

## 콘텐츠 구성 요소 추가 {#add-content-components}

이메일에 콘텐츠 구성 요소를 추가하고 필요에 맞게 조정하려면 아래 단계를 따르십시오.

1. 이메일 Designer에서 [기존 콘텐츠](existing-content.md)를 사용하거나 **[!UICONTROL 구조]**&#x200B;를 빈 콘텐츠로 끌어다 놓아 이메일 레이아웃을 정의합니다. [방법 알아보기](create-email-content.md)

1. 선택한 **[!UICONTROL 콘텐츠]**&#x200B;를 관련 구조 내부에 끌어다 놓습니다.

   ![](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >여러 구성 요소를 단일 구조 및 구조의 각 열에 추가할 수 있습니다.

1. 상황별 **[!UICONTROL 설정]** 탭을 사용하여 각 구성 요소에 대한 옵션을 조정합니다. 예를 들어 데스크탑 또는 모바일 디바이스에만 표시하도록 선택하거나 둘 다에 표시하도록 선택할 수 있습니다. 이 탭에서 링크 옵션을 관리할 수도 있습니다. [링크 관리에 대해 자세히 알아보기](message-tracking.md)

1. **[!UICONTROL 스타일]** 탭을 사용하여 각 구성 요소의 스타일 특성을 조정합니다. 예를 들어 각 구성 요소의 텍스트 스타일, 패딩 또는 여백을 변경할 수 있습니다. [정렬 및 패딩에 대해 자세히 알아보기](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. 오른쪽 창에 있는 **[!UICONTROL 콘텐츠]**&#x200B;의 고급 메뉴에서 필요에 따라 콘텐츠 구성 요소를 쉽게 삭제하거나 복제할 수 있습니다.

## 컨테이너 {#container}

간단한 컨테이너를 추가하여 다른 콘텐츠 구성 요소를 추가할 수 있습니다. 이렇게 하면 내부에서 사용되는 구성 요소와 다른 특정 스타일을 컨테이너에 적용할 수 있습니다.

예를 들어 **[!UICONTROL 컨테이너]** 구성 요소를 추가한 다음 해당 컨테이너 내부에 [버튼](#button) 구성 요소를 추가하면 컨테이너에 특정 배경을 사용하고 버튼에 다른 배경을 사용할 수 있습니다.

![](assets/email_designer_container_component.png){zoomable="yes"}

## 버튼 {#buttons}

**[!UICONTROL 버튼]** 구성 요소를 사용하여 이메일에 하나 이상의 버튼을 삽입하고 이메일 대상자를 다른 페이지로 리디렉션할 수 있습니다.

1. **[!UICONTROL 콘텐츠]** 목록에서 **[!UICONTROL 버튼]** 구성 요소를 드래그하여 **[!UICONTROL 구조]** 구성 요소에 놓습니다.

   ![](assets/email_designer_13.png){zoomable="yes"}

1. 새로 추가된 버튼을 클릭하여 텍스트를 개인화하고 **[!UICONTROL 설정]** 및 **[!UICONTROL 스타일]** 탭에 액세스합니다.

   ![](assets/email_designer_14.png){zoomable="yes"}

1. **[!UICONTROL URL]** 필드의 **[!UICONTROL 설정]** 탭에서 버튼을 클릭할 때 리디렉션할 URL을 추가합니다.

1. **[!UICONTROL 대상]** 드롭다운 목록을 사용하여 콘텐츠가 표시되는 방식을 선택합니다.

   * **[!UICONTROL None]**: 링크를 클릭한 프레임과 동일한 프레임에서 링크를 엽니다(기본값).
   * **[!UICONTROL Blank]**: 새 창이나 탭에서 링크를 엽니다.
   * **[!UICONTROL Self]**: 링크를 클릭한 프레임과 동일한 프레임에서 링크를 엽니다.
   * **[!UICONTROL Parent]**: 상위 프레임에서 링크를 엽니다.
   * **[!UICONTROL Top]**: 최상위 창에서 링크를 엽니다.

   ![](assets/email_designer_15.png){zoomable="yes"}

1. 다음에서 **[!UICONTROL 테두리]**, **[!UICONTROL 크기]**, **[!UICONTROL 여백]** 등 스타일 속성을 변경하여 버튼을 추가로 개인화할 수 있습니다. **[!UICONTROL 스타일]** 탭에서

## 텍스트 {#text}

**[!UICONTROL Text]** 구성 요소를 사용하여 전자 메일에 텍스트를 삽입하고 **[!UICONTROL 설정]** 및 **[!UICONTROL 스타일]** 탭을 사용하여 스타일(테두리, 크기, 패딩 등)을 조정합니다.

1. **[!UICONTROL 콘텐츠]** 메뉴에서 **[!UICONTROL 텍스트]**&#x200B;을(를) **[!UICONTROL 구조]** 구성 요소로 끌어다 놓습니다.

   ![](assets/email_designer_11.png){zoomable="yes"}

1. 새로 추가된 구성 요소를 클릭하여 텍스트를 개인화하고 **[!UICONTROL 설정]** 및 **[!UICONTROL 스타일]** 탭에 액세스합니다.

1. 상황별 도구 모음에서 다음 옵션을 사용하여 텍스트를 변경합니다.

   ![](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL 텍스트 스타일 변경]**: 텍스트에 볼드체, 이탤릭체, 밑줄 또는 취소선을 적용합니다.
   * **정렬 변경**: 왼쪽, 오른쪽, 가운데 또는 양쪽 정렬 중에서 텍스트 정렬 방식을 선택합니다.
   * **[!UICONTROL 목록 만들기]**: 텍스트에 글머리 기호 또는 번호 목록을 추가합니다.
   * **[!UICONTROL 제목 설정]**: 텍스트에 최대 6개의 제목 수준을 추가합니다.
   * **글꼴 크기**: 텍스트의 글꼴 크기를 픽셀 단위로 선택합니다.
   * **[!UICONTROL 이미지 편집]**: 텍스트 구성 요소에 이미지 또는 자산을 추가합니다.
   * **[!UICONTROL 소스 코드 표시]**: 텍스트의 소스 코드를 표시합니다. 소스 코드는 수정할 수 없습니다.
   * **[!UICONTROL 복제]**: 텍스트 구성 요소의 복사본을 추가합니다.
   * **[!UICONTROL 삭제]**: 이메일에서 선택한 텍스트 구성 요소를 삭제합니다.
   * **[!UICONTROL 개인화 추가]**: 개인화 필드를 추가하여 프로필 데이터의 콘텐츠를 사용자 정의합니다.
   * **[!UICONTROL 조건부 콘텐츠 활성화]**: 조건부 콘텐츠를 추가하여 타겟팅된 프로필에 구성 요소의 콘텐츠를 적용합니다.

1. 다음에서 텍스트 색상, 글꼴 패밀리, 테두리, 패딩, 여백 등 다른 스타일 속성을 조정합니다. **[!UICONTROL 스타일]** 탭에서

   ![](assets/email_designer_12.png){zoomable="yes"}

## 구분선 {#divider}

**[!UICONTROL 구분선]** 구성 요소를 사용하여 이메일의 레이아웃과 콘텐츠를 구성하기 위한 구분선을 삽입할 수 있습니다.

**[!UICONTROL 스타일]** 탭에서 선 색, 스타일, 높이 등의 스타일 특성을 조정할 수 있습니다.

![](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

**[!UICONTROL HTML]** 구성 요소를 사용하여 기존 HTML의 다른 부분을 복사하고 붙여넣을 수 있습니다. 이렇게 하면 무료 모듈식 HTML 구성 요소를 만들어 일부 외부 콘텐츠를 재사용할 수 있습니다.

1. **[!UICONTROL 구성 요소]**&#x200B;에서 **[!UICONTROL HTML]** 구성 요소를 드래그하여 **[!UICONTROL 구조]** 구성 요소에 놓습니다.

   ![](assets/email_designer_22.png){zoomable="yes"}

1. 새로 추가된 구성 요소를 클릭한 다음 상황별 도구 모음에서 **[!UICONTROL 소스 코드 표시]**&#x200B;를 선택하여 HTML을 추가합니다.

   ![](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>외부 콘텐츠를 전자 메일 DesignerAdobe 을 준수하도록 하려면 [메시지를 처음부터 만들고](create-email-content.md) 기존 전자 메일의 콘텐츠를 구성 요소로 복사하는 것이 좋습니다.

## 이미지 {#image}

>[!IMPORTANT]
>
>Assets 메뉴에 대한 액세스는 활성 Adobe Experience Manager as a Cloud Service 라이선스가 있는 사용자로 제한됩니다. 이 라이선스가 없으면 자산 메뉴를 사용할 수 없습니다.

**[!UICONTROL 이미지]** 구성 요소를 사용하여 이메일에 컴퓨터의 이미지 파일을 삽입할 수 있습니다.

1. **[!UICONTROL 콘텐츠]** 메뉴에서 **[!UICONTROL 이미지]**&#x200B;를 드래그하여 **[!UICONTROL 구조]** 구성 요소에 놓습니다.

   ![](assets/email_designer_9.png){zoomable="yes"}

1. 에셋에서 이미지 파일을 선택하려면 **[!UICONTROL 찾아보기]**&#x200B;를 클릭하십시오. **[!UICONTROL 미디어 가져오기]**&#x200B;를 선택할 수도 있습니다.

   Adobe Experience Manager에서 에셋을 업로드하고 추가하는 방법에 대한 자세한 내용은 [Adobe Experience Manager as a Cloud Service 설명서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html)를 참조하세요.

   ![](assets/email_designer_28.png){zoomable="yes"}

1. 폴더를 탐색하여 필요한 특정 에셋을 찾거나 검색 창을 사용하여 에셋을 효율적으로 찾습니다.

   찾고 있는 자산을 찾으면 **[!UICONTROL 선택]**&#x200B;을 클릭하세요.

   ![](assets/email_designer_29.png){zoomable="yes"}

1. 새로 추가한 구성 요소를 클릭하고 **[!UICONTROL 설정]** 탭을 사용하여 이미지 속성을 설정합니다.

   * **[!UICONTROL 이미지 제목]** 속성을 사용하면 이미지의 제목을 정의할 수 있습니다.
   * **[!UICONTROL 대체 텍스트]** 속성을 사용하면 이미지에 연결된 캡션을 정의할 수 있습니다. 이는 대체 HTML 속성에 해당합니다.

   ![](assets/email_designer_10.png){zoomable="yes"}

1. 링크를 추가하여 대상자를 다른 콘텐츠로 리디렉션할 수 있습니다. [자세히 알아보기](message-tracking.md)

1. 여백, 테두리 등 다른 스타일 속성을 조정하거나 **[!UICONTROL 스타일]** 탭을 사용합니다.

## 소셜 {#social}

**[!UICONTROL 소셜]** 구성 요소를 사용하면 이메일 콘텐츠에 소셜 미디어 페이지에 대한 링크를 삽입할 수 있습니다.

1. **[!UICONTROL 구성 요소]** 메뉴에서 **[!UICONTROL 소셜]** 구성 요소를 드래그하여 **[!UICONTROL 구조]** 구성 요소에 놓습니다.

1. 새로 추가된 구성 요소를 클릭합니다.

1. **[!UICONTROL 설정]** 탭의 **[!UICONTROL 소셜]** 필드에서 추가 또는 제거할 소셜 미디어를 선택합니다.

   ![](assets/email_designer_20.png){zoomable="yes"}

1. **[!UICONTROL 이미지 크기]** 필드에서 아이콘의 크기를 선택합니다.

1. 각 소셜 미디어 아이콘을 클릭하여 대상자가 리디렉션되는 **[!UICONTROL URL]**&#x200B;을 구성합니다.

   ![](assets/email_designer_21.png){zoomable="yes"}

1. 필요한 경우 **[!UICONTROL Source]** 필드에서 각 소셜 미디어의 아이콘을 변경할 수도 있습니다.

1. 다음에서 스타일, 여백, 테두리 등 다른 스타일 속성을 조정합니다. **[!UICONTROL 스타일]** 탭에서
