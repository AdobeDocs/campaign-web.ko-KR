---
audience: end-user
title: 오퍼 만들기 및 게시
description: Campaign 웹에서 오퍼를 만들고, 구성하고, 승인하고, 배포하는 방법을 알아봅니다
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 1%

---

# 오퍼 만들기 및 게시 {#create-offer}

**오퍼**&#x200B;는 자체 자격 기간, 대상 필터, 가중치 및 콘텐츠를 가진 개별 제안입니다. 오퍼는 **카테고리**&#x200B;를 통해 오퍼 카탈로그에 구성되어 있으며 **오퍼 공간**&#x200B;을 통해 수신자에게 제공됩니다.

오퍼를 만들기 전에 오퍼 환경이 구성되어 있고 오퍼 공간이 하나 이상 게시되어 있는지 확인하십시오. [오퍼 환경 구성](offer-environment.md) 및 [오퍼 공간 만들기 및 관리](offer-space.md)에서 자세히 알아보세요.

## 오퍼 카탈로그 액세스 {#access}

오퍼를 탐색하고 만들려면 왼쪽 탐색 레일에서 **[!UICONTROL 오퍼]**&#x200B;를 선택하십시오. 목록에는 기존 오퍼가 표시됩니다. 검색 필드, 폴더 선택기 또는 [쿼리 모델러](../query/query-modeler-overview.md)를 사용하여 목록을 필터링합니다.

![오퍼 카탈로그를 표시하는 스크린샷입니다.](assets/offers-offer.png){zoomable="yes"}

편집할 오퍼 이름을 클릭하거나 옆에 있는 세 점을 사용하여 **[!UICONTROL 복제]** 또는 **[!UICONTROL 삭제]**&#x200B;하세요.

## 오퍼 만들기 {#create}

새 오퍼를 만들려면 다음 작업을 수행하십시오.

1. 오퍼 목록에서 **[!UICONTROL 오퍼 만들기]**&#x200B;를 클릭합니다.

1. 오퍼를 만들 **[!UICONTROL 템플릿]**&#x200B;을(를) 선택하십시오(예: 빈 오퍼 또는 익명 오퍼 템플릿).

   ![오퍼 만들기를 보여 주는 스크린샷입니다.](assets/offers-offer-1.png){zoomable="yes"}

1. **[!UICONTROL 레이블]**&#x200B;을(를) 입력하고, 선택적으로 **[!UICONTROL 할당 대상]**&#x200B;을(를) 사용하여 운영자에게 오퍼를 할당하거나 **[!UICONTROL 오퍼 코드]**&#x200B;를 입력하십시오.

1. **[!UICONTROL 추가 옵션]**&#x200B;을 확장하여 자동 생성된 **[!UICONTROL 내부 이름]**&#x200B;을 편집하고, 오퍼가 저장된 **[!UICONTROL 범주]**&#x200B;를 선택하거나 설명을 추가하십시오. 조건을 추가합니다.

1. **[!UICONTROL 승인]**&#x200B;을 확장하여 **[!UICONTROL 자격 승인]** 및 **[!UICONTROL 콘텐츠 승인]** 그룹에 승인자를 할당합니다. 조건을 추가합니다.

1. **[!UICONTROL 사용자 지정 옵션]**&#x200B;을 확장하여 조직에서 오퍼 스키마에 추가한 추가 필드를 채웁니다. 이 섹션에 표시되는 필드는 Campaign 인스턴스마다 다릅니다. 조건을 추가합니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. 전체 설정 화면이 표시됩니다.

   ![오퍼 설정 화면을 보여주는 스크린샷](assets/offers-offer-2.png){zoomable="yes"}

### 자격 요건 정의 {#eligibility}

이 섹션에서는 오퍼를 표시할 시기와 대상을 제어할 수 있습니다. 다음 옵션을 사용할 수 있습니다.

* **[!UICONTROL 일정]** — 오퍼를 표시할 시작 날짜와 종료 날짜를 설정합니다.

  >[!NOTE]
  >
  >상위 범주와 자격 기간 교차가 고려됩니다. 오퍼의 자체 일정이 더 넓은 경우에도 오퍼는 표시되는 반면 상위 범주는 자격을 갖습니다.

* **[!UICONTROL 대상에 대한 필터]** — **[!UICONTROL 필터 만들기]**&#x200B;를 클릭하여 규칙 빌더를 열고 오퍼를 특정 대상으로 제한합니다. 전체 환경 대상에 오퍼를 사용할 수 있도록 하려면 필터를 비워 둡니다. 플랫폼 수준에서 선언된 **미리 정의된 필터**&#x200B;를 다시 사용하려면 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}를 참조하세요. 사전 정의된 필터는 클라이언트 콘솔에서 만들어집니다.

* **[!UICONTROL 오퍼 가중치 관리]** — **[!UICONTROL 오퍼 가중치 표시]**&#x200B;를 클릭한 다음 **[!UICONTROL 가중치 추가]**&#x200B;를 클릭하여 여러 오퍼를 동시에 사용할 수 있는 경우 오퍼의 우선 순위에 영향을 줍니다. 각 가중치에는 시작 날짜, 종료 날짜 및 선택적 필터가 있습니다.

>[!NOTE]
>
>오퍼 엔진은 가중치를 낮추어 적격 오퍼를 정렬하고 가장 높은 가중치 제안을 먼저 반환합니다. 선택 논리(**중재**)는 상위 범주 및 환경에 구성된 자격 규칙 및 가중치도 고려합니다. [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=ko){target="_blank"}에서 중재 원칙에 대해 자세히 알아보세요.

### 콘텐츠 정의 {#content}

오퍼에서 **[!UICONTROL 콘텐츠]** 탭을 선택합니다. 이 탭은 렌더링 함수에 의해 노출될 값을 정의합니다.

1. 기본 제공 특성 — **[!UICONTROL Title]**, **[!UICONTROL 대상 URL]**, **[!UICONTROL 이미지 URL]** 및 오퍼 스키마에서 선언된 사용자 지정 특성을 입력합니다.

1. [표현식 편집기](../query/expression-editor.md)를 사용하여 프로필 데이터, 오퍼 특성 또는 제안 필드를 통해 값을 개인화합니다.

1. HTML 및 텍스트 페이로드의 경우 **[!UICONTROL 콘텐츠 편집]**&#x200B;을 클릭하여 콘텐츠 편집기를 엽니다. 콘텐츠를 처음부터 디자인하거나, 자체 HTML을 코딩하거나, 원할 경우 샘플 템플릿에서 시작하여 기존 HTML을 가져올 수 있습니다.

>[!IMPORTANT]
>
>**[!UICONTROL 콘텐츠]** 섹션에서 사용할 수 있는 특성은 [!DNL nms:offer] 스키마에 따라 다릅니다. 사용자 지정 특성을 표시하려면 스키마를 확장하고 **[!UICONTROL 오퍼 콘텐츠]** 섹션에서 선택하세요. [스키마 작업](../administration/schemas.md)에서 자세히 알아보세요.

## 오퍼 미리 보기 {#preview}

오퍼를 제출하기 전에 미리 볼 수 있습니다.

1. 오퍼에서 **[!UICONTROL 개요]** 옆의 **[!UICONTROL 미리 보기]** 탭을 선택합니다.

   ![오퍼 미리 보기를 표시하는 스크린샷입니다.](assets/offers-offer-3.png){zoomable="yes"}

1. 대상 프로필을 선택하고, 해당되는 경우 미리 보기를 실행할 오퍼 공간을 선택합니다.

   오퍼 공간에 정의된 렌더링 함수가 오퍼 콘텐츠에 적용되고 결과 표현이 표시됩니다.

>[!NOTE]
>
>미리보기에서 오류가 반환되거나 컨텐츠가 없는 경우 오퍼 공간의 렌더링 기능, 오퍼의 자격 규칙 및 모든 필수 컨텐츠 필드가 채워졌는지 확인하십시오.

## 오퍼 승인 및 배포 {#approve-deploy}

오퍼는 승인 및 배포 주기를 거치므로 게재에서 즉시 사용할 수 없습니다.

1. 오퍼 개요에서 **[!UICONTROL 승인]**&#x200B;을 클릭합니다.

   ![오퍼 승인을 보여 주는 스크린샷](assets/offers-offer-4.png){zoomable="yes"}

1. **[!UICONTROL 자격]** 및 **[!UICONTROL 콘텐츠]**&#x200B;를 승인합니다. 콘텐츠는 오퍼 공간별로 승인될 수 있으므로 다른 콘텐츠는 보류 중인 상태로 두고 하나의 오퍼 공간에 대해 승인할 수 있습니다.

1. 두 승인이 모두 승인되면 **[!UICONTROL 배포]**&#x200B;를 클릭하여 오퍼를 라이브 환경에 게시합니다.

1. 오퍼 보기를 새로 고쳐 **[!UICONTROL Live]** 표시가 최신 상태인지 확인하세요.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>오퍼의 자격 및 콘텐츠를 승인하는 것은 두 가지 별개의 작업입니다. 오퍼는 부분적으로 승인될 수 있으며(예를 들어 콘텐츠만) 자격 승인이 이루어질 때까지 게재에 사용할 수 없습니다.

## 오퍼 대시보드 모니터링 {#dashboard}

오퍼 **[!UICONTROL 개요]** 탭에는 **[!UICONTROL 속성]**, **[!UICONTROL 콘텐츠]** 및 **[!UICONTROL 자격]** 카드의 오퍼 상태가 요약되어 있으며, 각 카드에는 연필 모양의 아이콘이 있어 다시 편집할 수 있습니다. **[!UICONTROL 표시]** 카드는 현재 디자인 상태와 함께 오퍼가 연결된 모든 오퍼 공간을 나열합니다.

![오퍼 대시보드를 표시하는 스크린샷입니다.](assets/offers-offer-5.png){zoomable="yes"}

**[!UICONTROL 로그]**&#x200B;를 클릭하여 배포 로그에 액세스하거나 **···**(**[!UICONTROL 자세히]**) 메뉴를 클릭하여 오퍼를 **[!UICONTROL 복제]** 또는 **[!UICONTROL 삭제]**&#x200B;합니다.

오퍼가 라이브로 전환되면 설정을 수정하면 디자인 오퍼가 다시 편집 가능한 상태로 전환됩니다. 라이브 표현은 다음 승인 및 배포 주기까지 그대로 유지됩니다.

## 게재에서 오퍼 사용 {#use-in-delivery}

오퍼가 라이브인 경우 일치하는 오퍼 공간을 타겟팅하는 모든 게재에서 오퍼를 선택할 수 있습니다. [메시지에 오퍼 추가](../msg/offers.md)에서 게재에서 오퍼를 설정하는 방법을 알아봅니다.

엔진 호출 빌드 방법, 오퍼 링크에 추적 기능을 적용하는 방법 등 전체 아웃바운드 게재 통합에 대해서는 [아웃바운드 게재의 Campaign v8 설명서 오퍼](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html?lang=ko){target="_blank"}를 참조하십시오.

