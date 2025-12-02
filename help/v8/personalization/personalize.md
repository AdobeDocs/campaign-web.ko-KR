---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign 웹에서 콘텐츠를 개인화하는 방법을 알아봅니다
feature: Personalization
topic: Personalization
old-role: Data Engineer
role: Developer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 4%

---

# 콘텐츠 개인화 {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="현재 날짜 추가"
>abstract="이 메뉴는 콘텐츠를 개인화하는 데 활용할 수 있는 날짜 형식 지정과 관련된 기능을 제공합니다."

게재 콘텐츠 Personalization은 메시지를 개별 수신자에게 맞춤화할 수 있는 주요 기능으로, 커뮤니케이션의 관련성을 높이고 참여를 유도합니다.

Adobe Campaign에서는 프로필의 이름, 위치 또는 과거 상호 작용과 같은 [프로필 데이터](#data-personalization) 및 게재의 특정 [변수](#variables-personalization)를 사용하여 커뮤니케이션에서 텍스트, 이미지 및 오퍼와 같은 요소를 동적으로 사용자 지정합니다.

게재 개인화는 사용자 경험을 개선하고 참여율을 향상시켜 전환율과 고객 만족도를 향상시킵니다.

## 개인화에 프로필 데이터 사용 {#data-personalization}

제목란, 전자 메일 링크 및 텍스트/단추 콘텐츠 구성 요소와 같은 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘이 있는 필드에서 액세스할 수 있는 표현식 편집기를 사용하여 프로필 데이터를 통해 게재를 개인화합니다. [식 편집기에 액세스하는 방법을 알아봅니다](gs-personalization.md#access).

### Personalization 구문 {#syntax}

Personalization 태그는 특정 구문 `<%= table.field %>`을(를) 따릅니다. 예를들어 받는 사람 테이블에서 받는 사람의 성을 삽입하려면 `<%= recipient.lastName %>` 구문을 사용합니다.

게재 준비 프로세스 중에 Adobe Campaign은 이러한 태그를 해석하여 각 수신자에 대한 해당 필드 값으로 대체합니다. 콘텐츠를 시뮬레이션하여 실제 교체를 확인합니다.

독립 실행형 이메일 전달을 위해 외부 파일에서 연락처를 업로드할 때 입력 파일의 모든 필드를 개인화할 수 있습니다. 구문은 다음과 같습니다. `<%= dataSource.field %>`

### 개인화 태그 추가 {#add}

게재에 개인화 태그를 추가하려면 다음 단계를 수행합니다.

1. 제목란이나 SMS 본문 같은 텍스트 유형 편집 필드에서 액세스할 수 있는 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘을 사용하여 식 편집기를 엽니다. [식 편집기에 액세스하는 방법을 알아봅니다](gs-personalization.md#access).

   ![개인화 대화 상자에 액세스하는 방법을 보여 주는 스크린샷](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. 표현식 편집기가 열립니다. Adobe Campaign 데이터베이스에서 사용할 수 있는 개인화 필드는 화면 왼쪽에 있는 여러 메뉴로 구성됩니다.

   ![개인화 필드 메뉴를 보여 주는 스크린샷](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | 메뉴 | 설명 |
   |------|-------------|
   | ![구독자 응용 프로그램 메뉴 아이콘](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | **[!UICONTROL 구독자 응용 프로그램]** 메뉴에는 사용된 터미널 또는 운영 체제와 같은 응용 프로그램의 구독자와 관련된 필드가 나열됩니다. *이 메뉴는 푸시 알림에만 사용할 수 있습니다.* |
   | ![받는 사람 메뉴 아이콘](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | **[!UICONTROL 받는 사람]** 메뉴에는 받는 사람의 이름, 나이 또는 주소와 같이 받는 사람 테이블에 정의된 필드가 나열됩니다. 독립 실행형 전자 메일 게재를 위해 [외부 파일에서 연락처를 업로드](../audience/file-audience.md)할 때 이 메뉴에는 입력 파일에서 사용할 수 있는 모든 필드가 나열됩니다. |
   | ![메시지 메뉴 아이콘](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | **[!UICONTROL 메시지]** 메뉴에는 지정된 수신자가 있는 마지막 이벤트의 날짜와 같이 모든 채널에서 받는 사람 또는 장치로 보낸 모든 메시지를 포함하여 게재 로그와 관련된 필드가 나열됩니다. |
   | ![배달 메뉴 아이콘](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | **[!UICONTROL 게재]** 메뉴에는 게재 채널 또는 레이블과 같이 게재 수행에 필요한 매개 변수와 관련된 필드가 나열됩니다. |

   >[!NOTE]
   >
   >기본적으로 각 메뉴에는 선택한 테이블(수신자, 메시지/게재) 내의 모든 필드가 나열됩니다. 선택한 테이블에 연결된 테이블의 필드를 포함하려면 목록 아래에 있는 **[!UICONTROL 고급 특성 표시]** 옵션을 사용하도록 설정하십시오.

1. 개인화 필드를 추가하려면 컨텐츠 내에서 원하는 위치에 커서를 놓고 `+` 단추를 클릭하여 삽입합니다.

1. 콘텐츠가 준비되면 저장하고 콘텐츠를 시뮬레이션하여 개인화 렌더링을 테스트합니다. 아래 예는 수신자의 이름을 사용하는 SMS 메시지의 개인화를 보여 줍니다.

   ![수신자의 이름으로 SMS 개인화 미리 보기를 표시하는 스크린샷](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![수신자의 이름으로 SMS 개인화 미리 보기를 표시하는 스크린샷](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## 개인화에 변수 사용 {#variables-personalization}

변수를 사용하여 게재를 개인화할 수도 있습니다. [게재에 변수 추가](../advanced-settings/delivery-settings.md#variables-delivery)에 대해 자세히 알아보세요.

예를 들어 `deliveryType` 변수는 아래와 같이 정의됩니다.

![deliveryType 변수의 정의를 보여 주는 스크린샷](assets/variables-deliveryType.png){zoomable="yes"}

이 변수는 **[!UICONTROL Personalization 추가]** 아이콘과 이 예제의 표현식 `<%= variables.deliveryType %>`을(를) 사용하여 게재 콘텐츠에 사용됩니다.

![개인화에서 deliveryType 변수의 사용을 보여 주는 스크린샷](assets/variables-perso.png){zoomable="yes"}

**[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 사용하여 변수 사용을 확인하십시오.

![deliveryType 변수가 있는 콘텐츠 시뮬레이션을 보여 주는 스크린샷](assets/variables-simulate.png){zoomable="yes"}