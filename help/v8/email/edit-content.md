---
audience: end-user
title: 이메일 콘텐츠 편집
description: Campaign 웹 사용자 인터페이스에서 이메일 콘텐츠를 편집하는 방법을 알아봅니다
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: d64e4c2833757239be181cbd333a9d2ce95aa35f
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 24%

---

# 이메일 콘텐츠 구성 {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="이메일 콘텐츠 정의"
>abstract="**콘텐츠 편집** 화면에서는 발신자 주소 및 제목 줄과 같은 메시지의 기본 요소를 정의하고, 첨부 파일이나 오퍼 추가와 같은 추가 작업을 수행하고, 이메일 디자이너에 액세스하여 메시지를 세련된 형태로 지정할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="이메일 속성 설정"
>abstract="**기본 세부 정보** 섹션에서는 발신자의 주소와 회신 주소를 업데이트하고 표현식 편집기를 사용하여 제목 줄을 정의할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="이메일에 파일 첨부"
>abstract="메시지에 삽입할 하나 이상의 파일을 선택합니다. 성능 문제를 방지하려면 이메일당 둘 이상의 첨부 파일을 포함하지 않는 것이 좋습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="추적 편집"
>abstract="기본적으로 게재에 대한 추적이 활성화됩니다. 즉, 메시지 콘텐츠에 포함된 모든 링크가 추적됩니다. 여기에서 이 옵션을 비활성화할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="링크 추가 및 메시지 추적"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="언어 추가"
>abstract="이 탭에서는 게재를 전송할 언어 목록을 찾을 수 있습니다. 언어 추가 버튼을 클릭하거나, 이 탭을 통해 다른 언어를 복제하여 더 많은 언어를 추가할 수 있습니다."

전자 메일 **[!UICONTROL 콘텐츠 편집]** 화면에서 다음을 수행할 수 있습니다.

* 보낸 사람의 주소 및 제목란과 같은 메시지의 기본 요소를 정의합니다.
* 첨부 추가 또는 오퍼 설정과 같은 추가 작업 수행
* [Email Designer](get-started-email-designer.md#start-authoring)에 액세스하여 올바른 이메일 콘텐츠 작성을 시작합니다
* 게재에 언어 변형을 추가합니다.

>[!NOTE]
>
>개인화 필드를 사용하여 이 화면에서 편집 가능한 모든 텍스트 필드를 채울 수 있습니다. [콘텐츠 개인화 방법 알아보기](../personalization/personalize.md)

## 게재 구성

전자 메일의 콘텐츠를 구성하거나 편집하려면 아래 단계를 따르십시오.

1. **[!UICONTROL 전자 메일 게재 대시보드]** 화면에서 [콘텐츠 편집](../email/create-email.md) 단추를 클릭합니다.

   ![전자 메일 게재 대시보드의 콘텐츠 편집 단추를 표시하는 스크린샷입니다.](assets/email-edit-content-button.png){zoomable="yes"}

1. 이메일 콘텐츠 편집 화면이 열립니다.

   ![전자 메일 콘텐츠 편집 대시보드를 표시하는 스크린샷입니다.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >새 전자 메일을 구성하는 경우 **[!UICONTROL 보낸 사람 이름]** 및 **[!UICONTROL 보낸 사람 전자 메일]** 필드가 이미 채워져 있습니다.

1. **[!UICONTROL 보낸 사람 이름]** 필드가 전자 메일 템플릿에 정의되어 있습니다. 이를 수정하려면 브랜드 이름과 같이 수신자가 쉽게 식별할 수 있는 이름을 사용하여 게재의 열람률을 높입니다.

   >[!NOTE]
   >
   >수신자의 경험을 더 개선하기 위해, 예를 들어 &quot;Luma에서 온 이브&quot;와 같은 사람의 이름을 추가할 수 있습니다.

1. **[!UICONTROL 보낸 사람 전자 메일]** 주소 필드도 전자 메일 템플릿에 정의되어 있습니다. 주소 도메인이 Adobe에게 위임한 하위 도메인과 일치하는지 확인합니다.

   >[!NOTE]
   >
   >&#39;@&#39; 앞 부분은 변경할 수 있지만 도메인 주소는 변경할 수 없습니다.

1. **[!UICONTROL 회신 필드]** 섹션을 확장합니다. 보낸 사람의 이름과 주소는 기본적으로 회신에 사용됩니다. 그러나 Adobe에서는 브랜드의 고객 지원 센터와 같은 기존 실제 주소를 사용하는 것이 좋습니다. 이 경우 수신자가 회신을 보내면 고객 지원팀에서 처리할 수 있습니다.

   ![전자 메일 콘텐츠 편집기의 회신 필드 섹션을 보여 주는 스크린샷입니다.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. 이메일 **[!UICONTROL 제목 줄]**&#x200B;을 정의합니다. 제목을 전용 필드에 직접 입력하거나 표현식 편집기를 열어 다양한 특성, 표현식 조각 또는 오퍼를 사용하여 [개인화](../personalization/personalize.md)를 추가하십시오.

1. 전자 메일에 파일을 첨부하려면 **[!UICONTROL 첨부 파일 추가]** 단추를 클릭한 다음 하나 이상의 파일을 선택하십시오.

   >[!NOTE]
   >
   >성능 문제를 방지하려면 이메일당 둘 이상의 첨부 파일을 포함하지 않는 것이 좋습니다.

   <!--limitation on size + number of files?-->

1. 전자 메일로 오퍼를 보내려면 **[!UICONTROL 오퍼 설정]** 단추를 사용하여 오퍼를 선택하십시오.

   그런 다음 개인화 필드를 사용하여 전자 메일에 삽입할 수 있습니다. [오퍼 전송 방법 알아보기](../msg/offers.md)

## 이메일 본문 편집

1. **[!UICONTROL 전자 메일 Designer]**&#x200B;을(를) 사용하여 전자 메일 콘텐츠를 구성하고 디자인하려면 [전자 메일 본문 편집](get-started-email-designer.md#start-authoring) 단추를 클릭하십시오.

   >[!NOTE]
   >
   >전자 메일 미리 보기 위에 마우스를 올려 놓고 **[!UICONTROL 전자 메일 디자이너 열기]**&#x200B;를 선택할 수도 있습니다.


   이메일 콘텐츠를 디자인하는 방법에 대한 추가 정보는 다음 섹션에서 확인할 수 있습니다.

   * [처음부터 이메일 작성](create-email-content.md)
   * [콘텐츠 스타일 지정](get-started-email-style.md)

1. 기본적으로 게재에 대해 추적 기능이 활성화되어 있습니다. **[!UICONTROL 선택 기능]** 섹션에서 이 옵션을 비활성화할 수 있습니다. [링크 추가 및 추적 관리 방법 알아보기](message-tracking.md)

1. 이메일 콘텐츠를 정의한 다음에는 **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 사용하여 이메일을 전송하기 전에 어떻게 표시되는지 확인합니다. [전자 메일을 미리 보고 테스트하는 방법을 알아보세요](../preview-test/preview-test.md).

## 다국어 게재 구성 {#multilingual-delivery}

Campaign 웹 사용자 인터페이스에서 전자 메일 게재를 다국어로 설정하여 프로필의 기본 언어를 기반으로 메시지를 보낼 수 있습니다. 기본 설정이 정의되지 않으면 메시지가 기본 언어로 전송됩니다.

다국어 게재에서 언어 관리는 변형을 기반으로 합니다. 각 변형은 하나의 언어를 나타냅니다.

게재를 만드는 동안 메시지에 필요한 언어 수에 해당하는 변형 수를 추가할 수 있습니다. 새 언어를 추가할 때 기본 언어를 정의할 수도 있습니다.

### 언어 변형 추가

언어 변형을 만들려면 다음 단계를 수행합니다.

1. 전자 메일 구성 화면의 상단에서 **[!UICONTROL 언어 추가]** 단추를 클릭합니다.

   >[!IMPORTANT]
   >
   >**[!UICONTROL 언어 추가]** 단추는 대상 차원에 언어 스키마가 포함된 경우에만 사용할 수 있습니다. 스키마 및 대상 차원에 대한 자세한 내용은 [자세한 설명서](https://experienceleague.adobe.com/ko/docs/campaign-web/v8/audiences/targeting-dimensions){target=_blank}를 참조하세요.

   ![](assets/edit-content_2.png){zoomable="yes"}


1. **[!UICONTROL 언어]** 드롭다운 목록에서 추가할 언어를 선택하십시오. 첫 번째 언어를 추가할 때 이 언어는 기본값으로 설정되고, 현재 콘텐츠는 기본 콘텐츠입니다. 새 언어를 추가할 때 콘텐츠는 기본 콘텐츠를 기반으로 합니다.

   >[!NOTE]
   >
   >이 목록을 통해 사용할 수 있는 언어는 언어 속성으로 정의된 값(예: 시스템, 사용자, dbenum 등)에 따라 다릅니다. 이 [섹션](https://experienceleague.adobe.com/ko/docs/campaign-web/v8/conf/enumerations){target=_blank}에서 열거형 관리에 대해 자세히 알아보세요.


   ![](assets/edit-content_3.png){zoomable="yes"}

   예를 들어, 영어(미국)의 경우:

   ![](assets/edit-content_8.png){zoomable="yes"}


1. 다른 언어를 추가하려면 이 프로세스를 반복합니다. **[!UICONTROL 언어]** 패널에 선택한 언어 목록, 다른 언어 수 및 기본 언어가 표시됩니다.

   예를 들어 영어, 프랑스어 및 스웨덴어를 선택한 경우 다음과 같이 이 3개의 언어를 볼 수 있습니다.

   ![](assets/edit-content_9.png){zoomable="yes"}

   오른쪽 상단 모서리에 있는 확장 버튼을 클릭하여 모든 언어를 삭제할 수 있습니다.

### 각 변형에 대한 이메일 콘텐츠 정의

언어가 설정되면 프로필로 보낼 전자 메일의 해당 기본 언어 콘텐츠를 정의합니다.

이메일 콘텐츠를 정의하려면 다음 단계를 수행합니다.

1. [전자 메일 본문 편집](get-started-email-designer.md#start-authoring) 단추를 클릭하여 **[!UICONTROL 전자 메일 Designer]**&#x200B;을(를) 엽니다.

   >[!NOTE]
   >
   >전자 메일 미리 보기 위에 마우스를 올려 놓고 **[!UICONTROL 전자 메일 디자이너 열기]**&#x200B;를 선택할 수도 있습니다.

   ![](assets/edit-content_11.png){zoomable="yes"}


1. **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 클릭하고 전자 메일이 표시되는 프로필 및 언어를 선택하여 게재를 미리 볼 수 있습니다.

1. 콘텐츠 시뮬레이트 창에서 프로필을 전환하여 해당 프로필에 대해 설정된 언어에 해당하는 이메일 콘텐츠를 미리 볼 수 있습니다.

   ![](assets/edit-content_5.png){zoomable="yes"}

### 언어 변형 복제 또는 제거

오른쪽 상단의 확장 단추를 클릭하고 **[!UICONTROL 모든 변형 삭제]** 단추를 클릭하여 모든 언어를 삭제할 수 있습니다.

![](assets/edit-content_13.png){zoomable="yes"}

언어 변형을 제거하려면 탭의 오른쪽에 있는 세 점을 클릭하고 제거를 선택합니다.

언어 변형을 복제하려면 탭의 오른쪽에 있는 세 점을 클릭하고 복제를 선택합니다. 기본 언어가 아닌 다른 언어를 복제하도록 선택하면 복제된 콘텐츠는 복제하도록 선택한 언어를 기반으로 합니다.


1. 이메일 콘텐츠를 정의한 다음에는 **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 사용하여 이메일을 전송하기 전에 어떻게 표시되는지 확인합니다. [전자 메일을 미리 보고 테스트하는 방법을 알아보세요](../preview-test/preview-test.md).