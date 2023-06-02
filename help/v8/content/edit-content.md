---
audience: end-user
title: 이메일 콘텐츠 편집
description: Campaign Web UI에서 이메일 콘텐츠를 편집하는 방법 알아보기
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: f04e8aa5ecb12fca02da640b0037441d4cd7d4d3
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 69%

---

# 이메일 콘텐츠 편집 {#configure-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="이메일 콘텐츠 만들기"
>abstract="이 섹션에서는 이메일 콘텐츠를 만들고 이메일 디자이너를 통해 세련된 형태를 지정할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="이메일 매개변수"
>abstract="“발신자” 및 “발신 이메일” 값은 이메일 템플릿에서 정의됩니다. 제목 줄은 표현식 편집기를 사용하여 개인화할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="이메일 첨부 파일"
>abstract="메시지에 삽입할 하나 이상의 파일을 선택하십시오."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="추적 옵션"
>abstract="기본적으로 게재에 대해 추적 기능이 활성화되어 있습니다. 여기에서 이 옵션을 비활성화할 수 있습니다."

이메일 콘텐츠를 작성하려면 이메일 생성 화면에서 **[!UICONTROL 콘텐츠 수정]** 버튼을 클릭합니다.[](../email/create-email.md)

![](assets/email-edit-content.png)

화면에 기본 세부 정보를 정의하고, 첨부 파일 추가 또는 오퍼 설정과 같은 추가 작업을 수행하고, 이메일 디자이너에 액세스하여 콘텐츠를 작성할 수 있습니다.

![](assets/email-edit-content-dashboard.png)

전자 메일 콘텐츠를 편집하는 단계는 다음과 같습니다.

1. 다음에서 **[!UICONTROL 보낸 사람 이름]** 필드에서는 브랜드 이름과 같이 수신자가 쉽게 식별할 수 있는 이름을 사용하여 게재의 열람률을 높입니다.

1. 이메일 **[!UICONTROL 제목 줄]**&#x200B;을 정의합니다. 이렇게 하려면 제목을 전용 필드에 직접 입력하거나 표현식 편집기를 열어 다양한 속성 및 콘텐츠 블록 또는 오퍼를 사용하여 개인화를 추가하도록 정의합니다. [콘텐츠 개인화 방법 알아보기](../personalization/personalize.md)
수신자의 경험을 더 개선하기 위해 개인 이름을 추가할 수 있습니다(예: &quot;Megastore의 Emma&quot;).

1. 다음에서 **[!UICONTROL 보낸 사람 이메일]** 주소 필드에서 주소 도메인이 Adobe에게 위임한 하위 도메인과 동일한지 확인합니다.

   &#39;@&#39; 앞 부분은 변경할 수 있지만 도메인 주소는 변경할 수 없습니다.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. 이메일 **[!UICONTROL 제목 줄]**&#x200B;을 정의합니다. 전용 필드에 제목을 직접 입력하거나 표현식 편집기를 열어 다양한 속성 및 콘텐츠 블록 또는 오퍼를 사용하여 개인화를 추가합니다. [콘텐츠 개인화 방법 알아보기](../personalization/personalize.md)

1. 이메일에 파일을 첨부하려면 **[!UICONTROL 첨부 파일 추가]** 버튼을 클릭한 다음 하나 이상의 파일을 선택합니다.

   >[!NOTE]
   >
   >    성능 문제를 방지하려면 이메일당 둘 이상의 첨부 파일을 포함하지 않는 것이 좋습니다.

   <!--limitation on size + number of files?-->

1. **[!UICONTROL 오퍼 설정]** 버튼으로 오퍼를 선택하여 이메일로 오퍼를 전송합니다.

   그런 다음 개인화 필드를 사용하여 선택한 오퍼를 이메일에 삽입할 수 있습니다. [오퍼 전송 방법 알아보기](offers.md)

1. **[!UICONTROL 이메일 본문 편집]** 버튼을 클릭하여 이메일 콘텐츠를 구조화하고 디자인합니다. 이메일 콘텐츠를 디자인하는 방법에 대한 추가 정보는 다음 섹션에서 확인할 수 있습니다.

   * [이메일 디자인 방법 알아보기](create-email-content.md)
   * [콘텐츠 스타일 지정](get-started-email-style.md)

1. 기본적으로 게재에 대해 추적 기능이 활성화되어 있습니다. **[!UICONTROL 선택 기능]** 섹션에서 이 옵션을 비활성화할 수 있습니다. [링크 추가 및 추적 관리 방법 알아보기](message-tracking.md)

1. 이메일 콘텐츠를 정의한 다음에는 **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 사용하여 이메일을 전송하기 전에 어떻게 표시되는지 확인합니다. [이메일 미리보기 및 테스트 방법 알아보기](../preview-test/preview-test.md)
