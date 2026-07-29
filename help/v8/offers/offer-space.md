---
audience: end-user
title: 오퍼 공간 만들기 및 관리
description: Campaign 웹에서 오퍼 공간을 만들고, 구성하고, 배포하고, 미리 보는 방법에 대해 알아봅니다
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# 오퍼 공간 만들기 및 관리 {#offer-space}

**오퍼 공간**&#x200B;은(는) 오퍼가 연락처에 노출되는 위치와 방법, 오퍼가 사용하는 채널(이메일, DM, SMS, 인바운드 웹 등), 오퍼가 사용할 수 있는 콘텐츠 필드, 최종 표시 작성 방법을 정의합니다. 단일 환경에는 각 노출 포인트에 대해 하나씩 여러 개의 오퍼 공간이 포함될 수 있습니다.

오퍼 공간은 그 자체로 채널이 아닙니다. 오퍼가 채널에 표시되는 특정 위치를 나타냅니다. 동일한 웹 페이지에 있는 두 개의 배너는 일반적으로 두 개의 서로 다른 오퍼 공간에 해당합니다. 전체 개념 모델은 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}를 참조하세요.

## 오퍼 공간 만들기 또는 수정{#create-offer-space}

오퍼 공간은 오퍼 환경 폴더에 저장됩니다. 플랫폼에서 사용할 수 있는 오퍼 공간을 찾아보려면 **[!UICONTROL 탐색기]**&#x200B;를 열고 오퍼 환경으로 이동한 다음 해당 공간이 포함된 하위 폴더를 선택하십시오.

![오퍼 공간 목록을 표시하는 스크린샷입니다.](assets/offers-space.png){zoomable="yes"}

**[!UICONTROL 오퍼 공간 만들기]**&#x200B;를 클릭하여 기존 오퍼 공간을 열거나 새 오퍼 공간을 만들 수 있습니다.

![오퍼 스페이스 화면을 표시하는 스크린샷입니다.](assets/offers-space-1.png){zoomable="yes"}

### 속성 정의 {#properties}

이 섹션에서는 다음 작업을 수행할 수 있습니다.

* 오퍼 공간에 대한 **[!UICONTROL 레이블]**&#x200B;을(를) 입력하십시오.
* 노출 지점(전자 메일, DM, SMS, 웹 등)과 일치하는 **[!UICONTROL 채널]**&#x200B;을 선택하세요.
* 이 오퍼 공간이 대량 게재 호출 외에 오퍼 엔진에 대한 단일(실시간, 단일 오퍼) 호출도 지원해야 하는 경우 **[!UICONTROL 단일 모드 사용]**&#x200B;을 선택합니다.

### 콘텐츠 필드 정의 {#content-fields}

컨텐츠 필드에는 오퍼 수준에서 편집하고 렌더링 함수에서 재사용할 수 있는 특성이 나열됩니다. 오퍼 공간의 필드를 추가하는 순서는 오퍼 **[!UICONTROL 콘텐츠]** 섹션에서 노출되는 순서를 제어합니다.

기본적으로 모든 오퍼에는 다음과 같은 기본 제공 콘텐츠 필드가 포함되어 있습니다. **[!UICONTROL 제목]**, **[!UICONTROL 대상 URL]**, **[!UICONTROL 이미지 URL]**, **[!UICONTROL HTML 콘텐츠]** 및 **[!UICONTROL 텍스트 콘텐츠]**. 렌더링에 필요한 사용자 지정 필드(예: **짧은 콘텐츠**, **추적된 URL** 또는 스키마 확장을 통해 추가된 모든 특성)를 사용하여 이 목록을 확장할 수 있습니다.

**[!UICONTROL 콘텐츠 필드 추가]**&#x200B;를 클릭한 다음 오퍼 스키마에서 표시할 특성을 선택하거나 **[!UICONTROL 식 편집]**&#x200B;을 클릭하여 사용자 지정 식을 대신 정의합니다.

>[!IMPORTANT]
>
>오퍼 **[!UICONTROL 콘텐츠]** 섹션에서 사용자 지정 특성을 편집할 수 있게 하려면 [!DNL nms:offer] 스키마의 **[!UICONTROL 오퍼 콘텐츠]** 섹션에서도 특성을 선언해야 합니다. [스키마 작업](../administration/schemas.md)에서 자세히 알아보세요.

### 렌더링 기능 구성 {#rendering}

렌더링 함수는 콘텐츠 필드에서 최종 오퍼 표현을 빌드합니다. 콘텐츠를 있는 그대로 출력하는 기본 렌더링 또는 필드를 HTML, XML 또는 텍스트와 결합하는 사용자 지정 함수 중에서 선택할 수 있습니다.

**[!UICONTROL HTML 렌더링]**, **[!UICONTROL XML 렌더링]** 또는 **[!UICONTROL 텍스트 렌더링]** 탭을 선택하고 **[!UICONTROL 렌더링 기능 오버로드]**&#x200B;를 활성화하십시오.

표현식 편집기를 사용하여 렌더링 함수를 작성합니다. [표현식 편집기](../query/expression-editor.md)에서 스페이스, 오퍼 특성 및 함수에 정의된 콘텐츠 필드를 참조할 수 있습니다.

>[!NOTE]
>
>렌더링 함수가 정의되지 않은 경우 오퍼 콘텐츠는 기본 특성을 사용하여 있는 그대로 반환됩니다. 오퍼 공간에서 **[!UICONTROL 단일 모드 사용]**&#x200B;을(를) 선택한 경우에만 XML 렌더링 함수를 사용할 수 있습니다.

### 스토리지 및 제안 상태 구성 {#storage}

이 섹션에서는 이 공간을 통해 생성된 제안이 지속되는 방식과 해당 상태가 라이프사이클 동안 어떻게 진화하는지를 제어할 수 있습니다.

* **[!UICONTROL 제안 삽입 비활성화]** — 이 오퍼 공간을 통해 생성된 제안이 제안 저장 테이블에 삽입되지 않도록 합니다.

* 제안 시 **[!UICONTROL 상태]** - 오퍼 엔진이 제안을 반환하는 즉시 제안에 적용된 상태(일반적으로 아웃바운드 게재에 대해 **[!UICONTROL 표시됨]**).

* 수락 시 **[!UICONTROL 상태]** — 받는 사람이 오퍼와 상호 작용할 때 적용되는 상태입니다(일반적으로 **[!UICONTROL 수락됨]**).

사용 가능한 상태 값은 클라이언트 콘솔에서 사용하는 목록과 일치합니다. 자세한 내용은 콘솔 설명서에서 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"}를 참조하세요.

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### 고급 설정 구성 {#advanced}

이 섹션에서 **[!UICONTROL 대상 식별]**&#x200B;을(를) 정의할 수 있습니다. **[!UICONTROL 추가]**&#x200B;를 클릭하고 **[!UICONTROL 받는 사람]** 특성을 하나 또는 여러 개 선택하거나 **[!UICONTROL 식 편집]**&#x200B;을 클릭하여 사용자 지정 식을 대신 정의합니다. 이 설정은 기본 오퍼 공간에 선택 사항입니다. 전체 참조 및 동작을 보려면 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}를 참조하세요.

**인바운드 웹 채널**&#x200B;에서 만든 오퍼 공간도 오퍼를 표시하고 오퍼 엔진을 호출하도록 웹 사이트를 구성해야 합니다. 이 통합은 클라이언트 콘솔에서 수행됩니다. Campaign v8 설명서에서 [실시간으로 오퍼 제공](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"} 및 [오퍼 엔진 통합 구성](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"}을 참조하십시오.

## 오퍼 공간 배포 {#deploy}

오퍼 공간을 게재에서 사용하려면 먼저 배포해야 합니다. 오퍼 공간을 저장한 다음 **배포**&#x200B;를 클릭합니다. 배포 상태가 오퍼 공간에 반영됩니다.

![오퍼 배포를 보여 주는 스크린샷입니다.](assets/offers-space-2.png){zoomable="yes"}

## 오퍼 공간 미리 보기 {#preview}

미리보기를 통해 특정 대상에 대해 오퍼를 선택하고 렌더링하는 방법을 시뮬레이션할 수 있습니다.

1. 오퍼 공간에서 **[!UICONTROL 개요]** 옆에 있는 **[!UICONTROL 미리 보기]** 탭을 선택합니다.

   ![오퍼 미리 보기를 표시하는 스크린샷입니다.](assets/offers-space-3.png){zoomable="yes"}

1. 대상 프로필을 선택하고 미리보기를 실행합니다. 일치하는 오퍼는 렌더링 함수에 의해 생성된 표현과 함께 반환됩니다.

>[!NOTE]
>
>제안이 반환되지 않으면 오퍼의 자격 규칙 및 스페이스의 구성을 확인하십시오.

그런 다음 카탈로그에서 [오퍼를 만들고](create-offer.md)을(를) 이 스페이스에 할당합니다.
