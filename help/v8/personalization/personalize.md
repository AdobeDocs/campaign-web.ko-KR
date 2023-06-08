---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign Web UI에서 콘텐츠를 개인화하는 방법 알아보기
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: fc9f6ffd8b242f608e05e51dee8299035518c533
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 5%

---


# 콘텐츠 개인화 {#add-personalization}

개인화는 를 사용하는 모든 필드에서 액세스할 수 있는 표현식 편집기를 사용하여 모든 게재에 추가할 수 있습니다. **[!UICONTROL 개인화 대화 상자 열기]** 제목 줄 필드 또는 이메일 링크 및 텍스트/버튼 콘텐츠 구성 요소와 같은 아이콘 [다이내믹 콘텐츠를 추가하는 위치 알아보기](gs-personalization.md/#access)

## 개인화 구문 {#syntax}

개인화 태그는 항상 다음 구문을 사용합니다. `<%=table.field%>`. 예를 들어 수신자 테이블에 저장된 수신자 이름을 삽입하려면 개인화 태그에 &lt;%= recipient.lastName %> 구문이 사용됩니다.

게재가 준비되면 이러한 태그는 Adobe Campaign에 의해 자동으로 해석되고 지정된 수신자에 대한 필드 값으로 대체됩니다. 그런 다음 콘텐츠를 시뮬레이션할 때 실제 교체 내용을 볼 수 있습니다.

## 개인화 태그 추가 {#add}

게재에 개인화 태그를 추가하려면 를 사용하여 표현식 편집기를 엽니다. **[!UICONTROL 개인화 대화 상자 열기]** 제목 줄이나 SMS 본문과 같은 텍스트 유형 편집 필드에서 액세스할 수 있는 아이콘 [다이내믹 콘텐츠를 추가하는 위치 알아보기](gs-personalization.md/#access)

![](assets/perso-access.png)

표현식 편집기가 표시됩니다. 개인화 필드는 화면 왼쪽에 있는 세 개의 메뉴로 구성됩니다. 이러한 메뉴를 통해 Adobe Campaign 데이터베이스에서 사용할 수 있는 모든 필드에 액세스할 수 있습니다.

![](assets/perso-insert-field.png)

| 메뉴 | 설명 |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | 다음 **[!UICONTROL 구독자 애플리케이션]** 메뉴에는 터미널 또는 운영 체제 사용 id와 같이 응용 프로그램의 구독자와 관련된 모든 필드가 나열됩니다. *이 메뉴는 푸시 알림에만 사용할 수 있습니다.* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | 다음 **[!UICONTROL 수신자]** 메뉴에는 수신자의 이름, 나이 또는 주소와 같이 수신자 표에 정의된 모든 필드가 나열됩니다. |
| ![](assets/do-not-localize/perso-message-menu.png) | 다음 **[!UICONTROL 메시지]** 메뉴에는 게재 로그와 관련된 모든 필드(예: 지정된 수신자가 있는 마지막 이벤트의 날짜 등 모든 채널에서 수신자 또는 장치로 전송된 모든 메시지)가 나열됩니다 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 다음 **[!UICONTROL 게재]** 메뉴에는 게재 채널, 레이블 등 게재 수행에 필요한 매개 변수와 관련된 모든 필드가 나열됩니다. |

>[!NOTE]
>
>기본적으로 각 메뉴에는 선택한 테이블(수신자, 메시지/게재) 내의 모든 필드가 표시됩니다. 선택한 테이블에 연결된 테이블의 필드를 포함하려면 **[!UICONTROL 고급 속성 표시]** 옵션은 목록 아래에 있습니다.

개인화 필드를 추가하려면 컨텐츠 내에서 원하는 위치에 커서를 놓고 + 단추를 클릭하여 삽입합니다.

콘텐츠가 준비되면 콘텐츠를 시뮬레이트하여 저장하고 개인화 렌더링을 테스트할 수 있습니다. 아래 예에서는 타겟팅된 프로필의 이름을 사용하는 SMS 메시지를 개인화하고 있습니다.

*메시지 콘텐츠에 개인화 태그 추가*

![](assets/perso-preview1.png)

*주어진 테스트 프로필에 대한 개인화 렌더링 시뮬레이션*

![](assets/perso-preview2.png)
