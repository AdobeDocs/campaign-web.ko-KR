---
title: Campaign에서 콘텐츠 개인화
description: Adobe Campaign 웹 UI에서 콘텐츠를 개인화하는 방법을 알아봅니다
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 0d74cababf2b4d66d3b2ce9b0ae2a0f00cb1cdef
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 콘텐츠 개인화{#add-personalization}

![](../assets/do-not-localize/badge.png)

다음을 수행하여 메시지 콘텐츠를 개인화할 수 있습니다.

* 동적 삽입 **개인화 필드**

   개인화 필드는 메시지의 첫 번째 수준 개인화에 사용됩니다. 개인화 편집기에서 데이터베이스에서 사용할 수 있는 필드를 선택할 수 있습니다. 게재의 경우 수신자, 메시지 또는 게재와 관련된 필드를 선택할 수 있습니다. 이러한 개인화 속성은 제목 줄이나 메시지 본문에 삽입할 수 있습니다.

   ![](assets/perso-subject-line.png)

   다음 구문은 콘텐츠에 수신자의 도시를 삽입합니다. &lt;%= recipient.location.city %>.

* 사전 정의된 삽입 **콘텐츠 블록**

   Campaign에는 게재에 삽입할 수 있는 특정 렌더링을 포함하는 개인화 블록 세트가 포함되어 있습니다. 예를 들어 메시지의 미러 페이지에 로고, 인사말 또는 링크를 추가할 수 있습니다. 콘텐츠 블록은 개인화 편집기의 전용 항목에서 사용할 수 있습니다.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## 이메일 제목란 개인화 {#personalize-subject-line}

에서 개인화를 추가하려면 **[!UICONTROL 제목 줄]** 메시지 필드를 보려면 아래 단계를 수행하십시오.

1. 을(를) 클릭합니다. **개인화 대화 상자 열기** 아이콘 을 클릭하여 제품에서 사용할 수 있습니다. **제목 줄** 필드.
1. 제목 줄 컨텐츠를 입력하고 추가할 개인화 속성을 선택합니다.
1. 클릭 **확인** 유효성을 검사하려면 다음을 수행하십시오. 개인화 속성이 제목 줄에 추가됩니다.

![](assets/perso-subject.png)

## 이메일 콘텐츠 개인화 {#personalize-emails}

이메일 콘텐츠를 개인화하려면 이메일 디자이너에서 메시지를 열고 다음을 수행합니다.

1. 텍스트 블록 내부를 클릭합니다.
1. 상황별 도구 모음에서 를 선택합니다 **개인화 추가**.

   ![](assets/perso-add-to-content.png)

1. 개인화 편집기에서 수신자 이름을 삽입하고 확인합니다.

   ![](assets/perso-add-name.png)

   개인화 속성이 전자 메일 콘텐츠에 추가됩니다.

   컨텐츠를 시뮬레이션하여 렌더링을 확인할 수 있습니다. [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## 이메일에서 링크 개인화 {#personalize-links}

개인화하려면 **링크**:

1. 텍스트 블록 또는 이미지를 선택합니다.
1. 상황별 도구 모음에서 를 선택합니다 **개인화 추가**.

   ![](assets/perso-link.png)

1. 개인화 편집기를 사용하여 링크를 정의하고 개인화합니다.

## 오퍼 개인화 {#personalize-offers}

오퍼 표현에 텍스트 유형 컨텐츠를 추가할 때 개인화 편집기에 액세스할 수도 있습니다. 추가 정보 [이 섹션](../content/offers.md).
