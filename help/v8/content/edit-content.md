---
audience: end-user
title: 이메일 콘텐츠 편집
description: Campaign Web UI에서 이메일 콘텐츠를 편집하는 방법 알아보기
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 100%

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

이메일 콘텐츠를 작성하려면 이메일 생성 화면에서 **[!UICONTROL 콘텐츠 수정]** 버튼을 클릭합니다.

![](assets/edit-content.png)

이 화면에서는 이메일 콘텐츠를 정의하고 이메일 디자이너에 액세스하여 이메일 콘텐츠를 디자인할 수 있습니다.

![](assets/content-dashboard.png)

이메일 콘텐츠를 정의하는 단계는 다음과 같습니다.

1. **[!UICONTROL 발신자]** 및 **[!UICONTROL 발신 이메일]** 정보를 확인합니다. 이 필드는 읽기 전용이며 이메일을 작성할 때 선택한 이메일 템플릿에서 구성됩니다.

1. 이메일 **[!UICONTROL 제목 줄]**&#x200B;을 정의합니다. 이렇게 하려면 제목을 전용 필드에 직접 입력하거나 표현식 편집기를 열어 다양한 속성 및 콘텐츠 블록 또는 오퍼를 사용하여 개인화를 추가하도록 정의합니다. [콘텐츠 개인화 방법 알아보기](../personalization/personalize.md)

1. **[!UICONTROL 오퍼 설정]** 버튼으로 오퍼를 선택하여 이메일로 오퍼를 전송합니다. 그런 다음 개인화 필드를 사용하여 선택한 오퍼를 이메일에 삽입할 수 있습니다. [오퍼 전송 방법 알아보기](offers.md)

1. **[!UICONTROL 이메일 본문 편집]** 버튼을 클릭하여 이메일 콘텐츠를 구조화하고 디자인합니다. 이메일 콘텐츠를 디자인하는 방법에 대한 추가 정보는 다음 섹션에서 확인할 수 있습니다.

   * [이메일 디자인 방법 알아보기](create-email-content.md)
   * [콘텐츠 스타일 지정](get-started-email-style.md)

1. 이메일에 파일을 첨부하려면 **[!UICONTROL 첨부 파일 추가]** 버튼을 클릭한 다음 하나 이상의 파일을 선택합니다.

   성능 문제를 방지하려면 이메일당 둘 이상의 첨부 파일을 포함하지 않는 것이 좋습니다.

   <!--limitation on size + number of files?-->

1. 기본적으로 게재에 대해 추적 기능이 활성화되어 있습니다. **[!UICONTROL 선택 기능]** 섹션에서 이 옵션을 비활성화할 수 있습니다. [링크 추가 및 추적 관리 방법 알아보기](message-tracking.md)

이메일 콘텐츠를 정의한 다음에는 **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 사용하여 이메일을 전송하기 전에 어떻게 표시되는지 확인합니다. [이메일 미리보기 및 테스트 방법 알아보기](../preview-test/preview-test.md)
