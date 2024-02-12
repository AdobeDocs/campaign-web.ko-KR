---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign 웹에서 콘텐츠를 개인화하는 방법을 알아봅니다
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 2%

---


# 콘텐츠 개인화 {#add-personalization}

를 사용하여 필드에서 액세스할 수 있는 표현식 편집기를 사용하여 모든 게재를 개인화할 수 있습니다 **[!UICONTROL 개인화 대화 상자 열기]** 제목 줄, 이메일 링크 및 텍스트/버튼 콘텐츠 구성 요소와 같은 아이콘 [표현식 편집기에 액세스하는 방법 알아보기](gs-personalization.md/#access)

## 개인화 구문 {#syntax}

개인화 태그는 특정 구문을 따릅니다. `<%= table.field %>`. 예를 들어 수신자 테이블에서 수신자의 성을 삽입하려면 `<%= recipient.lastName %>` 구문.

게재 준비 프로세스 중에 Adobe Campaign은 이러한 태그를 자동으로 해석하고 각 수신자에 대한 해당 필드 값으로 대체합니다. 콘텐츠를 시뮬레이션하여 실제 교체를 볼 수 있습니다.

독립 실행형 이메일 전달을 위해 외부 파일에서 연락처를 업로드할 때 입력 파일의 모든 필드를 개인화할 수 있습니다. 구문은 다음과 같습니다. `<%= dataSource.field %>`.

## 개인화 태그 추가 {#add}

게재에 개인화 태그를 추가하려면 다음 단계를 수행합니다.

1. 를 사용하여 표현식 편집기를 엽니다. **[!UICONTROL 개인화 대화 상자 열기]** 제목 줄이나 SMS 본문과 같은 텍스트 유형 편집 필드에서 액세스할 수 있는 아이콘 [표현식 편집기에 액세스하는 방법 알아보기](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 표현식 편집기가 열립니다. Adobe Campaign 데이터베이스에서 사용할 수 있는 개인화 필드는 화면 왼쪽에 있는 여러 메뉴로 구성됩니다.

   ![](assets/perso-insert-field.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   | 메뉴 | 설명 |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable=&quot;yes&quot;} | 다음 **[!UICONTROL 구독자 애플리케이션]** 메뉴에는 사용 단말 또는 운영 체제와 같은 애플리케이션의 가입자와 관련된 필드가 나열됩니다. *이 메뉴는 푸시 알림에만 사용할 수 있습니다.* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable=&quot;yes&quot;} | 다음 **[!UICONTROL 수신자]** 메뉴에는 수신자의 이름, 나이 또는 주소와 같이 수신자 표에 정의된 필드가 나열됩니다. 날짜 [외부 파일에서 연락처 업로드](../audience/file-audience.md) 독립 실행형 이메일 게재의 경우 이 메뉴에는 입력 파일에서 사용할 수 있는 모든 필드가 나열됩니다. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable=&quot;yes&quot;} | 다음 **[!UICONTROL 메시지]** 메뉴에는 지정된 수신자가 있는 마지막 이벤트의 날짜 등 모든 채널에서 수신자 또는 장치에 전송된 모든 메시지를 포함하여 게재 로그와 관련된 필드가 나열됩니다 |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable=&quot;yes&quot;} | 다음 **[!UICONTROL 게재]** 메뉴에는 게재 채널 또는 레이블과 같은 게재 수행에 필요한 매개 변수와 관련된 필드가 나열됩니다. |

   >[!NOTE]
   >
   >기본적으로 각 메뉴에는 선택한 테이블(수신자, 메시지/게재) 내의 모든 필드가 나열됩니다. 선택한 테이블에 연결된 테이블의 필드를 포함하려면 **[!UICONTROL 고급 속성 표시]** 옵션은 목록 아래에 있습니다.

1. 개인화 필드를 추가하려면 컨텐츠 내에서 원하는 위치에 커서를 놓고 `+` 단추를 클릭하여 삽입합니다.

1. 콘텐츠가 준비되면 콘텐츠를 시뮬레이트하여 저장하고 개인화 렌더링을 테스트할 수 있습니다. 아래 예는 수신자의 이름을 사용하는 SMS 메시지의 개인화를 보여 줍니다.

   ![](assets/perso-preview1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable=&quot;yes&quot;}{width="800" align="center"}
