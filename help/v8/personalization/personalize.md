---
title: Campaign에서 콘텐츠 개인화
description: Adobe Campaign 웹 UI에서 콘텐츠를 개인화하는 방법을 알아봅니다
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Advertising"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---


# 콘텐츠 개인화{#add-personalization}

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

전자 메일에 콘텐츠 블록을 추가하려면 동일한 단계를 적용하고 마지막 아이콘에서 콘텐츠 블록을 선택합니다.

![](assets/perso-insert-block.png)

콘텐츠 블록이 삽입되면 아래와 같이 이메일 콘텐츠에 추가됩니다. 게재 준비 단계에서 개인화가 생성되면 수신자 프로필에 자동으로 조정됩니다.

![](assets/perso-content-block-in-email.png)


내장 콘텐츠 블록은 다음과 같습니다.

* **[!UICONTROL Adobe Campaign에서 사용]**: &quot;Enabled by Adobe Campaign&quot; 로고를 삽입합니다.
* **[!UICONTROL 적절한 항목에 대한 서식 지정 함수]**: 는 **[!UICONTROL toSmartCase]** 각 단어의 첫 번째 문자를 대문자로 변경하는 Javascript 함수입니다.
* **[!UICONTROL 인사말]**: 받는 사람의 전체 이름과 쉼표를 삽입합니다. 예: &quot;안녕하세요, 존 도.&quot;
* **[!UICONTROL 로고 삽입]**: 인스턴스 설정에 정의된 로고를 삽입합니다.
* **[!UICONTROL 미러 페이지에 대한 링크]**: 에 링크를 삽입합니다. [미러 페이지](../content/mirror-page.md). 기본 형식은 다음과 같습니다. &quot;이 메시지를 올바르게 볼 수 없는 경우 여기를 클릭하십시오.&quot;
* **[!UICONTROL 미러 페이지 URL]**: 는 미러 페이지 URL을 삽입하여 게재 디자이너가 링크를 확인할 수 있도록 합니다.
* **[!UICONTROL 단일 모드의 오퍼 수락 URL]**: 오퍼를 설정할 수 있는 URL을 삽입합니다. **[!UICONTROL 수락됨]**. (상호 작용 모듈이 활성화된 경우 이 블록을 사용할 수 있습니다.)
* **[!UICONTROL 등록 확인]**: 구독을 확인하는 링크를 삽입합니다.
* **[!UICONTROL 등록 링크]**: 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다. 기본 콘텐츠는 다음과 같습니다. &quot;등록하려면 여기를 클릭하십시오.&quot;
* **[!UICONTROL 등록 링크(레퍼러 포함)]**: 방문자 및 게재를 식별할 수 있도록 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다.
* **[!UICONTROL 등록 페이지 URL]**: 구독 URL을 삽입합니다.
* **[!UICONTROL 콘텐츠 이메일 스타일]** 및 **[!UICONTROL 알림 스타일]**: 사전 정의된 HTML 스타일로 전자 메일의 형식을 지정하는 코드를 생성합니다.
* **[!UICONTROL 구독 취소 링크]**: 모든 게재에서 구독을 취소할 수 있는 링크를 차단 목록 삽입합니다. 연결된 기본 컨텐츠는 다음과 같습니다. &quot;이 메시지를 받는 이유는 ***조직 이름*** 또는 제휴 더 이상 메시지를 받지 않으려면 ***조직 이름*** 여기를 클릭하세요.&quot;



## 이메일에서 링크 개인화 {#personalize-links}

개인화하려면 **링크**:

1. 텍스트 블록 또는 이미지를 선택합니다.
1. 상황별 도구 모음에서 를 선택합니다 **링크 삽입**.

   ![](assets/perso-link.png)

1. 링크 레이블을 입력하고 **링크 삽입** 링크를 개인화하는 단추입니다.

   ![](assets/perso-link-insert-icon.png)

1. 개인화 편집기를 사용하여 링크를 정의 및 개인화하고 확인합니다.

   ![](assets/perso-link-edit.png)


## 오퍼 개인화 {#personalize-offers}

오퍼 표현에 텍스트 유형 컨텐츠를 추가할 때 개인화 편집기에 액세스할 수도 있습니다. 추가 정보 [이 섹션](../content/offers.md).
