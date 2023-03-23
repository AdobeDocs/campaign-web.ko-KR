---
audience: end-user
title: 이메일 디자이너 콘텐츠 구성 요소 사용
description: 이메일에서 콘텐츠 구성 요소를 사용하는 방법을 알아봅니다
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 8%

---

# 이메일 디자이너 콘텐츠 구성 요소 사용 {#content-components}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="콘텐츠 구성 요소 정보"
>abstract="콘텐츠 구성 요소는 이메일 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="콘텐츠 구성 요소 정보"
>abstract="콘텐츠 구성 요소는 랜딩 페이지 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="콘텐츠 구성 요소 정보"
>abstract="콘텐츠 구성 요소는 조각 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="콘텐츠 구성 요소 정보"
>abstract="콘텐츠 구성 요소는 템플릿 레이아웃 제작에 사용할 수 있는 빈 콘텐츠 플레이스홀더입니다."

## 콘텐츠 구성 요소 추가 {#add-content-components}

전자 메일에 컨텐츠 구성 요소를 추가하고 필요에 따라 조정하려면 아래 단계를 따르십시오.

1. 이메일 디자이너에서 기존 콘텐츠를 사용하거나 끌어서 놓습니다 **[!UICONTROL 구조 구성 요소]** 빈 컨텐츠에 추가하여 전자 메일 레이아웃을 정의합니다. [방법 알아보기](create-email-content.md)

1. 에 액세스하려면 **[!UICONTROL 컨텐츠 구성 요소]** 섹션의 왼쪽 창에서 해당 버튼을 선택합니다.

   ![](assets/email_designer_content_components.png)

1. 관련 구조 구성 요소 내에서 원하는 컨텐츠 구성 요소를 드래그하여 놓습니다.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >여러 구성 요소를 단일 구조 구성 요소와 구조 구성 요소의 각 열에 추가할 수 있습니다.

1. 다음 아이콘을 사용하여 각 구성 요소의 스타일링 속성을 조정합니다 **[!UICONTROL 구성 요소 설정]** 오른쪽 창입니다. 예를 들어 각 구성 요소의 텍스트 스타일, 패딩 또는 여백을 변경할 수 있습니다. [정렬 및 패딩에 대해 자세히 알아보기](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

이메일 콘텐츠를 처음부터 만드는 경우, **[!UICONTROL 컨텐츠 구성 요소]** 이메일에 배치되면 사용할 수 있는 비어 있는 원시 구성 요소를 사용하여 이메일을 추가로 개인화할 수 있습니다.
추가할 수 있는 수만큼 **[!UICONTROL 컨텐츠 구성 요소]** 필요할 때 **[!UICONTROL 구조 구성 요소]** 은 전자 메일의 레이아웃을 정의합니다.

## 컨테이너 {#container}

내에 다른 컨텐츠 구성 요소를 추가하는 간단한 컨테이너를 추가할 수 있습니다. 컨테이너에 특정 스타일을 적용할 수 있도록 해줍니다. 이 스타일은 내부에 사용된 구성 요소와 다릅니다.

예를 들어 **[!UICONTROL 컨테이너]** 구성 요소를 추가한 다음 [단추](#button) 구성 요소를 생성하지 않습니다. 특정 컨테이너 배경을 사용할 수도 있고 단추에 다른 배경을 사용할 수도 있습니다.

![](assets/email_designer_container_component.png)

## 버튼 {#buttons}

를 사용하십시오 **[!UICONTROL 단추]** 이메일에 하나 이상의 단추를 삽입하고 이메일 대상자를 다른 페이지로 리디렉션하는 구성 요소입니다.

1. From **[!UICONTROL 컨텐츠 구성 요소]**&#x200B;을(를) 끌어다 놓습니다. **[!UICONTROL 단추]** 구성 요소를 **[!UICONTROL 구조 구성 요소]**.

   ![](assets/email_designer_13.png)

1. 새로 추가한 버튼을 클릭하여 텍스트를 개인화하고 **[!UICONTROL 구성 요소 설정]** 전자 메일 디자이너 오른쪽 창에서 클릭합니다.

   ![](assets/email_designer_14.png)

1. 에서 **[!UICONTROL 링크]** 필드에서 버튼을 클릭할 때 리디렉션할 URL을 추가합니다.

1. 컨텐츠가 과 함께 표시되는 방식을 선택합니다. **[!UICONTROL Target]** 드롭다운 목록:

   * **[!UICONTROL 없음]**: 클릭한 것과 동일한 프레임에서 링크를 엽니다(기본값).
   * **[!UICONTROL 비어 있음]**: 새 창이나 탭에서 링크를 엽니다.
   * **[!UICONTROL 자체]**: 클릭한 것과 동일한 프레임에서 링크를 엽니다.
   * **[!UICONTROL 상위]**: 상위 프레임에서 링크를 엽니다.
   * **[!UICONTROL 상단]**: 창의 전체 본문에 링크를 엽니다.

   ![](assets/email_designer_15.png)

1. 다음과 같은 스타일 속성을 변경하여 단추를 추가로 개인화할 수 있습니다 **[!UICONTROL 테두리]**, **[!UICONTROL 크기]**, **[!UICONTROL 여백]**&#x200B;등 에서 **[!UICONTROL 구성 요소 설정]** 창

## 텍스트 {#text}

를 사용하십시오 **[!UICONTROL 텍스트]** 텍스트를 전자 메일에 삽입하고 스타일(테두리, 크기, 패딩 등)을 조정할 수 있는 구성 요소입니다 사용 **[!UICONTROL 구성 요소 설정]** 창

1. From **[!UICONTROL 컨텐츠 구성 요소]**, 드래그 앤 드롭 **[!UICONTROL 텍스트]** 에서 **[!UICONTROL 구조 구성 요소]**.

   ![](assets/email_designer_11.png)

1. 새로 추가된 구성 요소를 클릭하여 텍스트를 개인화하고 **[!UICONTROL 구성 요소 설정]** 전자 메일 디자이너의 오른쪽 창에서 클릭합니다.

1. 도구 모음에서 사용할 수 있는 다음 옵션을 사용하여 텍스트를 변경합니다.

   ![](assets/email_designer_27.png)

   * **[!UICONTROL 텍스트 스타일 변경]**: 텍스트에 굵게, 기울임체, 밑줄 또는 취소선을 적용합니다.
   * **정렬 변경**: 텍스트의 왼쪽, 오른쪽, 가운데 또는 좌우 정렬 중에서 선택합니다.
   * **[!UICONTROL 목록 만들기]**: 텍스트에 글머리 기호 또는 번호 목록을 추가합니다.
   * **[!UICONTROL 제목 설정]**: 텍스트에 최대 6개의 제목 수준을 추가합니다.
   * **글꼴 크기**: 텍스트의 글꼴 크기를 픽셀 단위로 선택합니다.
   * **[!UICONTROL 이미지 편집]**: 텍스트 구성 요소에 이미지나 자산을 추가합니다.
   * **[!UICONTROL 소스 코드 표시]**: 텍스트의 소스 코드를 표시합니다. 수정할 수 없습니다.
   * **[!UICONTROL 복제]**: 텍스트 구성 요소의 사본을 추가합니다.
   * **[!UICONTROL 삭제]**: 이메일에서 선택한 텍스트 구성 요소를 삭제합니다.
   * **[!UICONTROL 개인화 추가]**: 프로필 데이터의 콘텐츠를 사용자 지정하려면 개인화 필드를 추가합니다.
   * **[!UICONTROL 조건부 콘텐츠 활성화]**: 조건부 컨텐츠를 추가하여 구성 요소의 컨텐츠를 타깃팅된 프로필에 적용합니다.

1. 텍스트 색상, 글꼴 패밀리, 테두리, 패딩, 여백 등과 같은 기타 스타일 속성을 조정합니다. 에서 **[!UICONTROL 구성 요소 설정]** 창

   ![](assets/email_designer_12.png)

## 분할자 {#divider}

를 사용하십시오 **[!UICONTROL 구분선]** 전자 메일의 레이아웃과 콘텐츠를 구성하는 분할 라인을 삽입하는 구성 요소입니다.

선 색상, 스타일 및 높이와 같은 스타일 속성을 **[!UICONTROL 구성 요소 설정]** 창

![](assets/email_designer_16.png)

## HTML {#HTML}

를 사용하십시오 **[!UICONTROL HTML]** 구성 요소를 복사하여 기존 HTML의 다른 부분을 붙여넣습니다. 이를 통해 일부 외부 컨텐츠를 재사용할 수 있도록 무료 모듈식 HTML 구성 요소를 만들 수 있습니다.

1. From **[!UICONTROL 컨텐츠 구성 요소]**&#x200B;을(를) 끌어다 놓습니다. **[!UICONTROL HTML]** 구성 요소를 **[!UICONTROL 구조 구성 요소]**.

   ![](assets/email_designer_22.png)

1. 새로 추가된 구성 요소를 클릭한 다음, 을 선택합니다 **[!UICONTROL 소스 코드 표시]** 상황별 도구 모음에서 HTML을 추가합니다.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>이메일 디자이너와 호환되는 외부 콘텐츠를 만들고자 하는 경우, Adobe은 메시지를 처음부터 만들고 기존 이메일의 콘텐츠를 구성 요소로 복사하는 것을 권장합니다.

## 이미지 {#image}

를 사용하십시오 **[!UICONTROL 이미지]** 구성 요소를 사용하여 컴퓨터의 이미지 파일을 전자 메일에 삽입합니다.

1. in **[!UICONTROL 컨텐츠 구성 요소]**, 드래그 앤 드롭 **[!UICONTROL 이미지]** 에서 **[!UICONTROL 구조 구성 요소]**.

   ![](assets/email_designer_9.png)

1. 클릭 **[!UICONTROL 찾아보기]** 자산에서 이미지 파일을 선택하려면 다음을 수행하십시오.

1. 새로 추가한 구성 요소를 클릭하고 **[!UICONTROL 구성 요소 설정]** 창:

   * **[!UICONTROL 이미지 제목]** 이미지에 제목을 정의할 수 있습니다.
   * **[!UICONTROL 대체 텍스트]** 이미지에 연결된 캡션을 정의할 수 있습니다. 이것은 대체 HTML 속성에 해당합니다.

   ![](assets/email_designer_10.png)

1. 여백, 테두리 등과 같은 다른 스타일 속성을 조정합니다. 또는 링크를 추가하여 대상자를 **[!UICONTROL 구성 요소 설정]** 창

## 소셜 {#social}

를 사용하십시오 **[!UICONTROL Social]** 소셜 미디어 페이지에 대한 링크를 이메일 콘텐츠에 삽입하는 구성 요소입니다.

1. From **[!UICONTROL 컨텐츠 구성 요소]**&#x200B;을(를) 끌어다 놓습니다. **[!UICONTROL Social]** 구성 요소를 **[!UICONTROL 구조 구성 요소]**.

1. 새로 추가한 구성 요소를 클릭합니다.

1. 에서 **[!UICONTROL Social]** 필드 **[!UICONTROL 구성 요소 설정]** 창에서 추가하거나 제거할 소셜 미디어를 선택합니다.

   ![](assets/email_designer_20.png)

1. 에서 아이콘 크기를 선택합니다 **[!UICONTROL 이미지 크기]** 필드.

1. 각 소셜 미디어 아이콘을 클릭하여 를 구성합니다 **[!UICONTROL URL]** 대상 을 리디렉션합니다.

   ![](assets/email_designer_21.png)

1. 필요한 경우, 각 소셜 미디어의 아이콘을 변경할 수도 있습니다 **[!UICONTROL 이미지]** 필드.

1. 스타일, 여백, 테두리 등과 같은 다른 스타일 속성을 조정합니다. 에서 **[!UICONTROL 구성 요소 설정]** 창
