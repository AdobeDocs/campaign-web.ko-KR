---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign Web UI에서 콘텐츠를 개인화하는 방법 알아보기
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# 콘텐츠 개인화{#add-personalization}

표현식 편집기를 사용하여 모든 게재에 개인화를 추가할 수 있습니다.

개인화 태그는 항상 다음 구문을 사용합니다. `<%=table.field%>`예를 들어 수신자 테이블에 저장된 수신자 이름을 삽입하려면 개인화 태그에 &lt;%= recipient.lastName %> 구문이 사용됩니다.

게재가 준비되면 이러한 태그는 Adobe Campaign에 의해 자동으로 해석되고 지정된 수신자에 대한 필드 값으로 대체됩니다. 그런 다음 콘텐츠를 시뮬레이션할 때 실제 교체 내용을 볼 수 있습니다.

게재에 개인화 태그를 추가하려면 제목 줄이나 SMS 본문과 같은 텍스트 유형 편집 필드에서 액세스할 수 있는 개인화 대화 상자 열기 아이콘을 클릭합니다.

![](assets/perso-access.png)

표현식 편집기가 표시됩니다. 개인화 필드는 화면 왼쪽에 있는 세 개의 메뉴로 구성됩니다. 이러한 메뉴를 통해 Adobe Campaign 데이터베이스에서 사용할 수 있는 모든 필드에 액세스할 수 있습니다.

| 메뉴 | 설명 |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | 다음 **[!UICONTROL 수신자]** 메뉴에는 수신자의 이름, 나이 또는 주소와 같이 수신자 표에 정의된 모든 필드가 나열됩니다. |
| ![](assets/do-not-localize/perso-message-menu.png) | 다음 **[!UICONTROL 메시지]** 메뉴에는 게재 로그와 관련된 모든 필드(예: 지정된 수신자가 있는 마지막 이벤트의 날짜 등 모든 채널에서 수신자 또는 장치로 전송된 모든 메시지)가 나열됩니다 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 다음 **[!UICONTROL 게재]** 메뉴에는 게재 채널, 레이블 등 게재 수행에 필요한 매개 변수와 관련된 모든 필드가 나열됩니다. |

>[!NOTE]
>
>기본적으로 이 목록에는 선택한 테이블(수신자, 메시지/게재) 내의 모든 필드가 표시됩니다. 선택한 테이블에 연결된 테이블의 필드를 포함하려면 **[!UICONTROL 고급 속성 표시]** 옵션은 목록 아래에 있습니다.

개인화 필드를 추가하려면 컨텐츠 내에서 원하는 위치에 커서를 놓고 + 단추를 클릭하여 삽입합니다.

![](assets/perso-insert-field.png)

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

1. 콘텐츠 블록을 삽입하면 이메일 콘텐츠에 추가됩니다. 게재 준비 단계에서 개인화가 생성되면 수신자 프로필에 자동으로 적용됩니다.

   ![](assets/perso-content-block-in-email.png)


## 오퍼 개인화 {#personalize-offers}

오퍼 표시에 텍스트 유형의 콘텐츠를 추가할 때도 개인화 편집기에 액세스할 수 있습니다. [이 섹션](../content/offers.md)에서 자세히 알아보십시오.

