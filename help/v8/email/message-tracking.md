---
audience: end-user
title: 메시지 추적
description: 링크를 추가하고 전송된 메시지를 추적하는 방법 알아보기
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: 53f3cc27ed6d768d134902a9196f0b221fedcde0
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 21%

---

# 링크 추가 및 메시지 추적 {#tracking}

이메일 Designer을 사용하여 콘텐츠에 링크를 추가하고 전송된 메시지를 추적하여 수신자의 동작을 모니터링할 수 있습니다.

## 링크 삽입 {#insert-links}

메시지를 디자인할 때 콘텐츠에 링크를 추가할 수 있습니다.

>[!NOTE]
>
>추적이 활성화되면 메시지 콘텐츠에 포함된 모든 링크가 추적됩니다.

이메일 콘텐츠에 링크를 삽입하려면 다음 단계를 따르십시오.

1. 요소를 선택하고 상황별 도구 모음에서 **[!UICONTROL 링크 삽입]**&#x200B;을 클릭합니다.

1. 만들려는 링크의 유형을 선택합니다.

   ![메시지 추적 도구에 링크를 삽입하는 인터페이스를 보여 주는 스크린샷](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL 외부 링크]**: 외부 URL에 링크를 삽입합니다.

   * **[!UICONTROL 랜딩 페이지]**: 랜딩 페이지에 링크를 삽입합니다. 동적 랜딩 페이지(**[!UICONTROL URL의 서비스]** 옵션이 선택된 상태)를 선택하면 목록에서 서비스를 선택할 수 있습니다. [자세히 알아보기](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![이메일 디자이너의 랜딩 페이지에 연결하는 인터페이스를 보여 주는 스크린샷](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL 구독 링크]**: 구독 서비스에 대한 링크를 삽입합니다. 사용자가 링크를 클릭하면 선택한 서비스에서 참조한 구독 랜딩 페이지로 이동됩니다. [자세히 알아보기](../audience/manage-services.md#create-service)

     ![서비스 도구에서 기본 구독 링크를 만드는 인터페이스를 보여주는 스크린샷](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL 구독 취소 링크]**: 구독 취소 서비스에 대한 링크를 삽입합니다. 구독자가 링크를 클릭하면 선택한 서비스에서 참조되는 구독 취소 랜딩 페이지로 이동됩니다. [자세히 알아보기](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. 해당 필드에 원하는 URL을 입력하거나 랜딩 페이지 또는 서비스를 선택하고 링크 설정 및 스타일을 정의합니다.

1. **[!UICONTROL 레이블]**&#x200B;과 **[!UICONTROL 링크]**&#x200B;를 추가합니다.

1. 변경 내용을 저장합니다.

1. 링크를 만든 후 필요한 경우 **[!UICONTROL 설정]** 탭에서 수정합니다.

   * 링크를 편집하고 **[!UICONTROL Target]**&#x200B;을(를) 변경합니다.
   * 해당 옵션을 선택하여 링크에 밑줄을 긋을지 여부를 선택합니다.

   ![메시지 추적 도구에서 링크 속성을 수정하기 위한 설정 인터페이스를 표시하는 스크린샷](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>마케팅 유형 이메일 메시지에는 트랜잭션 메시지에 필요하지 않은 옵트아웃 링크를 포함해야 합니다. 메시지 범주(**[!UICONTROL 마케팅]** 또는 **[!UICONTROL 트랜잭션]**)는 채널 표면 수준에서 메시지를 만들 때 정의됩니다.

모든 이메일 메시지에 미러 페이지에 대한 특정 링크를 포함합니다. [이 섹션](mirror-page.md)에서 미러 페이지에 대해 자세히 알아보십시오.

## 추적 관리 {#manage-tracking}

[전자 메일 Designer](create-email-content.md)을(를) 사용하면 각 링크에 대한 추적 유형을 편집하는 등 추적된 URL을 관리할 수 있습니다.

1. 추적할 콘텐츠의 모든 URL 목록을 표시하려면 왼쪽 창에서 **[!UICONTROL 링크]** 아이콘을 클릭합니다.

   이 목록은 중앙 집중식 보기를 제공하며 이메일 콘텐츠에서 각 URL을 찾는 데 도움이 됩니다.

1. 링크를 편집하려면 해당 연필 아이콘을 클릭합니다.

   ![메시지 추적 도구에서 링크를 편집하기 위한 인터페이스를 보여주는 스크린샷](assets/message-tracking-edit-links.png){zoomable="yes"}

1. 필요한 경우 **[!UICONTROL 추적 형식]**&#x200B;을(를) 수정합니다.

   ![메시지 추적 도구에서 추적 형식을 편집하기 위한 인터페이스를 보여주는 스크린샷](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   추적된 각 URL에 대해 추적 모드를 다음 값 중 하나로 설정합니다.

   * **[!UICONTROL 추적됨]**: 이 URL에 대한 추적을 활성화합니다.
   * **[!UICONTROL 옵트아웃]**: 이 URL을 옵트아웃 또는 구독 취소 URL로 표시합니다.
   * **[!UICONTROL 미러 페이지]**: 이 URL을 미러 페이지 URL로 표시합니다.
   * **[!UICONTROL Never]**: 이 URL을 추적할 수 없습니다. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 추적된 링크를 그룹화할 수 있는 링크에 **[!UICONTROL Category]**&#x200B;를 추가하고 **[!UICONTROL 저장]**&#x200B;을 클릭하세요.

   ![메시지 추적 도구에서 추적된 링크에 범주를 추가하는 인터페이스를 보여주는 스크린샷](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. 게재를 전송한 후 게재 보고서에 액세스합니다. **[!UICONTROL 추적]** 메뉴의 **[!UICONTROL URL 및 클릭스트림]** 보고서에는 게재에서 가장 많이 방문한 URL이 표시됩니다. [자세히 알아보기](../reporting/gs-reports.md)