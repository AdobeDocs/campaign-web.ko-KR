---
audience: end-user
title: 메시지 추적
description: 링크를 추가하고 보낸 메시지를 추적하는 방법을 알아봅니다
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Advertising"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# 링크 추가 및 메시지 추적 {#tracking}

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

모든 이메일 메시지에 미러 페이지에 대한 특정 링크를 추가해야 합니다. 의 미러 페이지에 대해 자세히 알아보기 [이 섹션](mirror-page.md).

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

1. 추가 **[!UICONTROL 카테고리]** 추적된 링크를 그룹화하기 위한 링크로 이동하여 **[!UICONTROL 저장]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. 게재를 보낸 후 게재 보고서에 액세스합니다. 아래에 **[!UICONTROL 추적]** 메뉴, **[!UICONTROL URL 및 클릭 스트림]** 보고서는 게재 중 가장 많이 방문한 URL을 표시합니다. [자세히 알아보기](../reporting/reports.md)
