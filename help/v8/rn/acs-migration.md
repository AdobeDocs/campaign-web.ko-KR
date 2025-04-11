---
audience: end-user
title: Campaign Standard에서 Adobe Campaign Web으로의 전환
description: Campaign Web 사용자 인터페이스 살펴보기
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Campaign Standard에서 Campaign v8로의 전환 {#acs-to-ac}

Adobe Campaign Standard 사용자는 이제 Adobe Campaign Managed Cloud Services v8로 전환할 수 있습니다. 이러한 전환은 다음과 같은 몇 가지 이점을 제공합니다.

* **강력한 IT 인프라**: Managed Cloud Services v8은 보다 강력한 IT 인프라를 제공하여 캠페인에 대한 향상된 성능, 안정성 및 확장성을 보장합니다.
* **향상된 지원**: Managed Cloud Services 팀은 원활한 전환과 지속적인 플랫폼 모니터링을 위해 최고의 지원을 제공합니다. 지원에는 문제 해결 및 사전 예방 유지 관리가 포함됩니다.
* **Adobe Experience Platform과 통합**: Managed Cloud Services v8은 Adobe Experience Platform과 원활하게 연결되어 사용자가 데이터를 완전히 활용하고 채널 간에 개인화되고 영향력 있는 캠페인을 제공할 수 있습니다.
* **일관된 사용자 인터페이스 및 경험**: Managed Cloud Services v8로 전환해도 워크플로가 중단되지 않습니다. 사용자는 익숙한 인터페이스와 경험을 계속 즐기면서 팀의 학습 곡선을 최소화합니다.

**Campaign v8로 전환하는 Campaign Standard 사용자라면 [이 문서에서](../../adoption/home.md) 시작하는 방법을 알아보십시오.**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 주요 기능 {#key-features}

Campaign v8 사용자는 새로운 Campaign 웹 인터페이스와 v8 콘솔 모두에 액세스할 수 있습니다. 데이터와 설정은 환경 간에 동기화됩니다. 클라이언트 콘솔에서 사용할 수 있는 모든 데이터와 설정은 Explorer 왼쪽 탐색에서 액세스할 수 있는 Campaign 웹 사용자 인터페이스에 표시됩니다. [자세히 알아보기](../get-started/user-interface.md#user-interface-explorer)

Campaign 웹 사용자 인터페이스는 마케터가 캠페인을 쉽게 빌드하고 오케스트레이션할 수 있도록 설계되었습니다. Campaign v8 웹 사용자 인터페이스의 주요 기능은 다음과 같습니다.

* **현대적이고 친숙한 통합 경험**. [자세히 알아보기](../get-started/connect-to-campaign.md).
* **강력한 새로운 기능 및 원활한 프로세스**. [자세히 알아보기](../get-started/user-interface.md).
* **단순하고 직관적인 쿼리 모델러**. [자세히 알아보기](../query/query-modeler-overview.md).
* **기본 제공 크로스 채널 캠페인 관리 기능**. [자세히 알아보기](../msg/gs-messages.md).
* **캠페인 워크플로우 활동을 다시 디자인했습니다**. [자세히 알아보기](../workflows/gs-workflows.md).
* **간단한 프로필 만들기 및 관리**. [자세히 알아보기](../audience/about-recipients.md).
* **미리 정의된 필터**. [자세히 알아보기](../get-started/predefined-filters.md).
* 전자 메일 디자인을 위한 **HTML 변환기**. [자세히 알아보기](../email/existing-content.md).
* **오퍼가 있는 SMS**. [자세히 알아보기](../msg/offers.md).

Campaign 클라이언트 콘솔은 관리자와 개발자가 환경을 구성하고 사용자 정의할 수 있도록 설계되었습니다. Campaign 클라이언트 콘솔에서 사용할 수 있는 주요 기능은 [이 설명서](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/new/whats-new){target="_blank"}에 자세히 설명되어 있습니다.

>[!NOTE]
>
>이 페이지](../get-started/capability-matrix.md)에서 Campaign 웹 사용자 인터페이스와 Campaign 클라이언트 콘솔 간의 상호 운용성과 지원되는 기능 및 지원되지 않는 기능에 대해 자세히 알아보십시오.[

## 용어 {#terminology}

대부분의 개념은 Campaign v8과 Campaign Standard 간에 유사합니다. 그러나 몇 가지 용어 차이가 있습니다. 예를 들면 다음과 같습니다.

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## 특정 기능 {#new-features}

Campaign v8로 원활하게 전환할 수 있도록 주요 Campaign Standard 기능이 Campaign v8에 추가되었습니다. 이러한 기능은 [이 설명서](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank}에 자세히 설명되어 있으며 Campaign Standard에서 전환하는 사용자만 사용할 수 있습니다.

* **동적 보고**: 동적 보고에서는 마케팅 활동의 영향을 측정할 수 있는 사용자 지정 가능한 실시간 보고서를 제공합니다. 여기에는 열람 및 클릭과 같은 실용적인 이메일 캠페인 데이터와 함께 성별, 도시, 연령 등의 차원별 인구 통계 분석을 위한 프로필 데이터에 대한 액세스가 포함됩니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}

* **중앙 브랜딩**: Adobe Campaign을 통해 회사는 브랜드 시각적 및 기술적 지침을 정의할 수 있습니다. 사용자는 로고부터 이메일 발신자, URL 또는 도메인과 같은 기술적 측면까지 일관된 브랜드를 고객에게 제시할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html).

* **REST API**: Campaign Standard 마이그레이션된 사용자는 REST API를 사용하여 Adobe Campaign에 대한 통합을 만들고 Adobe Campaign과 다른 기술을 연결하여 에코시스템을 구축할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}

* **랜딩 페이지**: Campaign v8 랜딩 페이지에는 Campaign Standard과의 기능 패리티를 보장하기 위한 개선 사항이 포함되어 있습니다. [릴리스 정보](../rn/release-notes.md#new-24-4) 및 랜딩 페이지 [설명서](../landing-pages/get-started-lp.md)에서 자세한 내용을 살펴보십시오.

* **시각적 조각**: 시각적 조각은 하나 이상의 이메일 게재 또는 콘텐츠 템플릿에서 참조되는 재사용 가능한 시각적 구성 요소입니다. 조각을 수정하면 해당 조각을 사용하는 모든 콘텐츠가 업데이트됩니다. 이 기능을 사용하면 마케팅 사용자가 개선된 디자인 프로세스에서 빠른 메시지 어셈블리를 위해 여러 사용자 지정 콘텐츠 블록을 미리 빌드할 수 있습니다. [자세히 알아보기](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->