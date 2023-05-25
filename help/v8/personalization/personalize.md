---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign Web UI에서 콘텐츠를 개인화하는 방법 알아보기
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 048f754005744bcab5b64f265e9e9cdf9776dca8
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 90%

---


# 콘텐츠 개인화{#add-personalization}

다음과 같은 작업을 수행하여 메시지 콘텐츠를 개인화할 수 있습니다.

* 동적 **개인화 필드** 삽입

   개인화 필드는 메시지의 첫 번째 수준 개인화에 사용됩니다. 개인화 편집기에서 데이터베이스에서 사용 가능한 모든 필드를 선택할 수 있습니다. 게재의 경우 수신자, 메시지 또는 게재와 관련된 모든 필드를 선택할 수 있습니다. 이러한 개인화 속성은 메시지의 제목 줄이나 본문에 삽입할 수 있습니다.

   ![](assets/perso-subject-line.png)

   다음 구문은 콘텐츠에 수신자의 도시를 삽입합니다. &lt;%= recipient.location.city %>

* 미리 정의된 **콘텐츠 블록** 삽입

   Campaign에는 게재에 삽입할 수 있는 특정 렌더링이 포함된 개인화 블록 세트가 제공됩니다. 예를 들어 로고, 인사말 메시지 또는 메시지 미러 페이지에 대한 링크를 추가할 수 있습니다. 콘텐츠 블록은 개인화 편집기의 전용 항목에서 사용할 수 있습니다.

   ![](assets/perso-content-blocks.png)

* 만들기 **조건부 콘텐츠**

   예를 들어 수신자의 프로필을 기반으로 동적 개인화를 추가하도록 조건부 콘텐츠를 구성합니다. 특정 조건이 참일 때 텍스트 블록 및/또는 이미지가 삽입됩니다.


## 이메일 제목 줄 개인화 {#personalize-subject-line}

메시지의 **[!UICONTROL 제목 줄]** 필드에 개인화를 추가하려면 아래 단계를 따르십시오.

1. **[!UICONTROL 제목 줄]** 필드 오른쪽에 있는 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘을 클릭합니다.

   ![](assets/perso-subject.png){width="600"}

1. 제목 줄 콘텐츠를 입력하고 추가할 개인화 속성을 선택합니다.

1. 클릭 **[!UICONTROL 확인]****을 확인할 수 없습니다. 개인화 속성이 제목 줄에 추가됩니다.

## 이메일 콘텐츠 개인화 {#personalize-emails}

이메일 콘텐츠를 개인화하려면 이메일 디자이너에서 메시지를 열고 다음 작업을 수행하십시오.

1. 텍스트 블록 내부를 클릭합니다.
1. 상황별 도구 모음에서 **[!UICONTROL 개인화 추가]**&#x200B;를 선택합니다.

   ![](assets/perso-add-to-content.png)

1. 개인화 편집기에 수신자의 이름을 삽입하고 확인합니다.

   ![](assets/perso-add-name.png)

   개인화 속성이 이메일 콘텐츠에 추가됩니다.

   콘텐츠를 시뮬레이트하여 렌더링을 확인할 수 있습니다. [자세히 알아보기](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. 이메일에 콘텐츠 블록을 추가하려면 동일한 단계를 적용하고 마지막 아이콘에서 콘텐츠 블록을 선택합니다.

   ![](assets/perso-insert-block.png)

1. 삽입되면 콘텐츠 블록이 이메일 콘텐츠에 추가됩니다. 게재 준비 단계에서 개인화가 생성되면 수신자 프로필에 자동으로 조정됩니다.

   ![](assets/perso-content-block-in-email.png)

## 이메일 링크 개인화 {#personalize-links}

**링크**&#x200B;를 개인화하려면 다음 작업을 수행하십시오.

1. 텍스트 블록 또는 이미지를 선택합니다.
1. 상황별 도구 모음에서 **링크 삽입**&#x200B;을 선택합니다.

   ![](assets/perso-link.png)

1. 링크 레이블을 입력하고 **링크 삽입** 버튼을 사용하여 링크를 개인화합니다.

   ![](assets/perso-link-insert-icon.png)

1. 개인화 편집기를 사용하여 링크를 정의하고 개인화한 다음 확인합니다.

   ![](assets/perso-link-edit.png)


## 오퍼 개인화 {#personalize-offers}

오퍼 표시에 텍스트 유형의 콘텐츠를 추가할 때도 개인화 편집기에 액세스할 수 있습니다. [이 섹션](../content/offers.md)에서 자세히 알아보십시오.

## 기본 제공 콘텐츠 블록 {#ootb-content-blocks}

내장된 콘텐츠 블록은 다음과 같습니다.

* **[!UICONTROL Adobe Campaign에 의해 활성화됨]**: “Adobe Campaign에서 활성화됨” 로고를 삽입합니다.
* **[!UICONTROL 고유 명사 서식 지정 기능]**: **[!UICONTROL toSmartCase]** 자바스크립트 기능을 생성합니다. 이 기능은 각 단어의 첫 글자를 대문자로 바꿉니다.
* **[!UICONTROL 인사말]**: 수신자의 전체 이름과 함께 쉼표가 뒤따르는 인사말을 삽입합니다. 예: “안녕하세요 John Doe 님,”
* **[!UICONTROL 로고 삽입]**: 인스턴스 설정에서 정의한 로고를 삽입합니다.
* **[!UICONTROL 미러 페이지 링크]**: [미러 페이지](../content/mirror-page.md)에 대한 링크를 삽입합니다. 기본 형식은 “이 메시지가 제대로 표시되지 않는 경우 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 미러 페이지 URL]**: 미러 페이지 URL을 삽입하여 게재 디자이너가 링크를 확인할 수 있도록 합니다.
* **[!UICONTROL 단일 모드의 오퍼 수락 URL]**: 오퍼를 **[!UICONTROL 수락됨]**&#x200B;으로 설정할 수 있는 URL을 삽입합니다. 상호 작용 모듈이 활성화된 경우 이 블록을 사용할 수 있습니다.
* **[!UICONTROL 등록 확인]**: 구독을 확인할 수 있는 링크를 삽입합니다.
* **[!UICONTROL 등록 링크]**: 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다. 기본 콘텐츠는 “등록하려면 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 등록 링크(레퍼러 포함)]**: 방문자 및 게재를 식별할 수 있는 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다.
* **[!UICONTROL 등록 페이지 URL]**: 구독 URL을 삽입합니다.
* **[!UICONTROL 콘텐츠 이메일 스타일]** 및 **[!UICONTROL 알림 스타일]**: 미리 정의된 HTML 스타일로 이메일 형식을 지정하는 코드를 생성합니다.
* **[!UICONTROL 구독 취소 링크]**: 모든 게재에서 구독을 취소(차단 목록에 추가)할 수 있는 링크를 삽입합니다. 기본 관련 콘텐츠는 다음과 같습니다. “귀하가 ***조직 이름***&#x200B;의 소식을 받고 있거나 제휴를 맺고 있기 때문에 이 메시지가 전송되었습니다. 더 이상 ***조직 이름***&#x200B;에서 메시지를 받지 않으려면 여기를 클릭하십시오.”
