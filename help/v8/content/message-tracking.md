---
audience: end-user
title: 메시지 추적
description: 링크를 추가하고 보낸 메시지를 추적하는 방법을 알아봅니다
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c1fc5bd98969ab43680daf613e4050f9cd2185bf
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# 링크 추가 및 메시지 추적 {#tracking}

>[!NOTE]
>
>이 설명서는 개발 중이며 자주 업데이트됩니다. 이 컨텐츠의 최종 버전은 2023년 1월에 준비될 예정입니다.

수신자의 동작을 모니터링하기 위해 이메일 디자이너를 사용하여 컨텐츠에 링크를 추가하고 메시지를 추적합니다.

## 링크 삽입 {#insert-links}

메시지를 디자인할 때 콘텐츠에 링크를 추가할 수 있습니다.

>[!NOTE]
>
>추적이 활성화되면 메시지 콘텐츠에 포함된 모든 링크가 추적됩니다.

이메일 콘텐츠에 링크를 삽입하려면 아래 단계를 수행하십시오.

1. 요소를 선택하고 를 클릭합니다 **[!UICONTROL 링크 삽입]** 상황별 도구 모음

   ![](assets/message-tracking-insert-link.png)

1. 추가 **[!UICONTROL 레이블]** 그리고 **[!UICONTROL 링크]**.

1. 변경 내용을 저장합니다.

1. 링크가 만들어지더라도 **[!UICONTROL 구성 요소 설정]** 오른쪽 창입니다.

   * 링크를 편집하고 링크를 변경할 수 있습니다 **[!UICONTROL Target]**.
   * 해당 옵션을 선택하여 링크에 밑줄을 긋도록 선택할 수 있습니다.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>마케팅 유형 이메일 메시지에는 옵트아웃 링크가 포함되어야 하며, 이것은 트랜잭션 메시지에 필요하지 않습니다. 메시지 카테고리(**[!UICONTROL 마케팅]** 또는 **[!UICONTROL 트랜잭션]**)은 채널 표면(즉, 메시지 사전 설정) 수준에서 정의되며 메시지를 만들 때 정의됩니다.

## 미러 페이지에 대한 링크 {#mirror-page}

미러 페이지는 웹 브라우저를 통해 온라인으로 액세스할 수 있는 HTML 페이지입니다. 콘텐츠는 전자 메일의 콘텐츠와 동일합니다.

이메일의 미러 페이지에 대한 링크를 추가하려면 다음을 수행합니다.

1. 요소를 선택하고 를 클릭합니다 **[!UICONTROL 링크 삽입]** 상황별 도구 모음

   ![](assets/message-tracking-mirror-page.png)

1. 을(를) 선택합니다 **[!UICONTROL 링크 삽입]** 아이콘을 클릭하여 개인화 메뉴에 액세스합니다.

   ![](assets/message-tracking-mirror-page_2.png)

1. 에서 **[!UICONTROL 콘텐츠 블록]** 메뉴, 선택 **[!UICONTROL 미러 페이지 URL]** 을(를) 클릭합니다. **[!UICONTROL 추가]**.

   ![](assets/message-tracking-mirror-page_3.png)

미러 페이지가 자동으로 생성됩니다.

>[!IMPORTANT]
>
>미러 페이지 링크는 자동으로 생성되므로 편집할 수 없습니다. 여기에는 원본 이메일을 렌더링하는 데 필요한 암호화된 개인화된 데이터가 모두 포함됩니다. 따라서 값이 큰 개인화된 속성을 사용하면 긴 미러 페이지 URL이 생성되므로 링크가 최대 URL 길이를 갖는 웹 브라우저에서 작동하지 않을 수 있습니다.

전자 메일이 전송되면 수신자가 미러 페이지 링크를 클릭하면 전자 메일의 컨텐츠가 기본 웹 브라우저에 표시됩니다.

>[!NOTE]
>
>테스트 프로필로 전송된 증명의 경우 미러 페이지에 대한 링크가 활성화되지 않습니다. 최종 메시지에서만 활성화됩니다.

미러 페이지의 보존 기간은 60일입니다. 이후 미러 페이지는 더 이상 사용할 수 없습니다.

## 추적 관리 {#manage-tracking}

다음 [이메일 디자이너](create-email-content.md) 각 링크에 대한 추적 유형 편집과 같이 추적된 URL을 관리할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 링크]** 아이콘을 클릭하여 추적할 컨텐츠의 모든 URL 목록을 표시합니다.

   이 목록을 사용하면 중앙 집중식 보기를 사용하고 이메일 콘텐츠에서 각 URL을 찾을 수 있습니다.

1. 링크를 편집하려면 해당 연필 아이콘을 클릭합니다.

   ![](assets/message-tracking-edit-links.png)

1. 을 수정할 수 있습니다 **[!UICONTROL 추적 유형]** 필요한 경우:

   ![](assets/message-tracking-edit-a-link.png)

   추적된 각 URL에 대해 추적 모드를 다음 값 중 하나로 설정할 수 있습니다.

   * **[!UICONTROL 추적됨]**: 이 URL에서 추적을 활성화합니다.
   * **[!UICONTROL 옵트아웃]**: 이 URL을 옵트아웃 또는 구독 취소 URL로 간주합니다.
   * **[!UICONTROL 미러 페이지]**: 이 URL이 미러 페이지 URL인 것으로 간주합니다.
   * **[!UICONTROL 절대 안 함]**: 이 URL의 추적을 활성화하지 않습니다. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

