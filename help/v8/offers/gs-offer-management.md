---
audience: end-user
title: 오퍼 관리 시작
description: Adobe Campaign 웹에서 오퍼를 관리하는 방법 알아보기
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 763
ht-degree: 3%

---

# 오퍼 관리 시작 {#gs-offer-management}

이 기능을 사용하면 게재에 개인화된 오퍼를 추가하고 주어진 컨텍스트에서 각 프로필에 대해 가장 관련성이 높은 오퍼를 제공할 수 있습니다. 오퍼는 간단한 커뮤니케이션 메시지이거나 하나 또는 여러 제품에 대한 프로모션일 수 있습니다. 자격 규칙 및 우선 순위 가중치에 따라 오퍼 엔진은 제시할 최상의 제안을 선택합니다.

Campaign 웹 사용자 인터페이스를 사용하여 오퍼를 엔드투엔드 관리할 수 있습니다. 오퍼 환경을 만들고, 구성하고, 오퍼 공간을 디자인하고, 오퍼 카탈로그를 만들고, 자격 규칙을 설정하고, 오퍼 콘텐츠를 편집하고, 오퍼를 게시할 수 있습니다.

그런 다음 오퍼가 **자격 규칙** 및 **우선 순위 가중치**&#x200B;를 기반으로 하는 게재를 통해 수신자에게 제공되므로 주어진 컨텍스트에서 각 프로필에 대해 최상의 오퍼가 선택됩니다.

>[!NOTE]
>
>Campaign 웹 사용자 인터페이스는 가장 일반적인 오퍼 관리 사용에 중점을 둡니다. 고급 구성은 Campaign 클라이언트 콘솔에서 계속 사용할 수 있습니다. [Campaign v8 설명서를 참조하세요](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=ko){target="_blank"}

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## 주요 개념 {#concepts}

오퍼 작업을 시작하기 전에 관련된 주요 오브젝트에 익숙해지십시오.

* **오퍼 환경** — 오퍼 카탈로그 및 관련 오퍼 공간을 포함하는 컨테이너입니다. 오퍼를 만들고 구성하는 **디자인** 환경과 배달에 사용할 수 있는 승인되고 배포된 개체가 포함된 읽기 전용 **[!UICONTROL Live]** 환경의 두 가지 유형이 있습니다. [자세히 알아보기](offer-environment.md)

* **오퍼 공간** — 오퍼가 노출되는 위치와 방법(전자 메일, DM, SMS, 인바운드 웹 등)을 정의합니다. 스페이스에는 오퍼에서 사용할 수 있는 컨텐츠 필드, 오퍼 표시를 작성하는 렌더링 함수 및 제안 상태를 유도하는 저장소 설정이 나열됩니다. [자세히 알아보기](offer-space.md)

* **오퍼 카탈로그 및 범주** — 오퍼는 **범주** 및 하위 범주의 계층 구조 카탈로그로 구성됩니다. 각 범주는 자격 규칙, 유효 날짜 및 **응용 프로그램 테마**&#x200B;를 공유할 수 있습니다. 모든 오퍼를 수신하기 위해 디자인 환경에 기본 카테고리가 제공됩니다.

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **오퍼** — 자체 자격 기간, 대상 필터, 가중치 및 콘텐츠가 있는 개별 오퍼입니다. 오퍼를 승인하고 배포한 후에 수신자에게 제공할 수 있습니다. [자세히 알아보기](create-offer.md)

* **오퍼 제안** — 지정된 스페이스(웹 사이트의 배너, 이메일, SMS 등)에서 담당자에게 오퍼를 제공한 결과. 게재당 제안 수는 [게재에서 오퍼를 설정](../msg/offers.md)할 때 구성됩니다.

* **중재** - 제공할 오퍼를 선택하기 위해 오퍼 엔진에서 우선 순위별로 적격 오퍼에 순위를 매기는 원칙입니다. 차익거래는 카테고리, 오퍼 및 컨텍스트 오퍼에 정의된 기준을 사용합니다.

## 오퍼 관리 플로우 {#workflow}

Campaign 웹 UI의 일반적인 전체 흐름은 다음과 같습니다.

1. **오퍼 환경 설정 검토** - 디자인/라이브 매핑, 자격 조건 및 가중치 관리 설정을 확인하십시오. [자세히 알아보기](offer-environment.md)

1. **오퍼 공간 만들기** — 채널과 일치하는 콘텐츠 필드, 렌더링 함수 및 고급 매개 변수를 정의합니다. [자세히 알아보기](offer-space.md)

1. **카탈로그에 오퍼 만들기** - 각 오퍼의 자격 기간, 대상 필터, 가중치 및 콘텐츠를 설정합니다. [자세히 알아보기](create-offer.md)

1. **승인 및 배포** — 승인을 위해 오퍼를 제출하고 해당 콘텐츠 및 자격을 승인한 다음 배포 프로세스에서 이를 라이브 환경에 게시하도록 합니다. [자세히 알아보기](create-offer.md#approve-deploy)

1. **게재에 오퍼 추가** — 이메일, SMS, 푸시 또는 DM 게재에서 오퍼 공간 및 제안을 참조합니다. [자세히 알아보기](../msg/offers.md)

## 웹 UI에서 오퍼에 액세스 {#access}

오퍼는 **[!UICONTROL 오퍼]** 왼쪽 메뉴에서 사용할 수 있습니다. 거기에서 카탈로그를 검색하고, 에디션에 대한 오퍼를 열고, 승인 및 배포 상태를 모니터링할 수 있습니다.

![오퍼 메뉴를 보여 주는 스크린샷](assets/offers-gs.png){zoomable="yes"}

오퍼 환경 및 오퍼 공간은 해당 폴더로 이동하여 **[!UICONTROL 탐색기]**&#x200B;를 통해 액세스합니다.


## 콘솔 전용 보완 {#console-complements}

일부 오퍼 기능은 아직 웹 사용자 인터페이스에 노출되지 않았으며 클라이언트 콘솔에서 구성해야 합니다.

* **오퍼 시뮬레이션** — 보내기 전에 오퍼 배포를 테스트할 수 있는 **시뮬레이션** 모듈입니다. [오퍼 시뮬레이션](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=ko#offer-simulation){target="_blank"}을 참조하세요.

* **사전 정의된 필터** 관리 — 오퍼에서 참조할 수 있는 재사용 가능한 필터 규칙입니다. [미리 정의된 필터 관리](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}를 참조하세요.

* **오퍼 추적** — 제안 내역을 제공할 오퍼 제안에 대한 추적을 구성하는 중입니다. [오퍼 제안 추적](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=ko){target="_blank"}을 참조하세요.

* **운영자 역할** — 오퍼 관리자/게재 관리자 권한을 할당합니다. [상호 작용 모듈의 연산자](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}를 참조하십시오.

* **상호 작용 모범 사례 및 중재 규칙**. [캠페인 상호 작용 모범 사례](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=ko){target="_blank"}를 참조하세요.

* **보고** — 전용 오퍼 및 제안 보고서는 아직 웹 사용자 인터페이스에서 사용할 수 없습니다.