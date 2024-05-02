---
audience: end-user
title: Campaign Standard에서 Adobe Campaign 웹으로 전환
description: Campaign 웹 사용자 인터페이스 살펴보기
source-git-commit: 2e5ddb7aca83a1a348ca50603d38a89c2762bb80
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 7%

---


# Campaign v8로 Campaign Standard 전환{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Adobe Campaign Managed Cloud Services v8에 오신 것을 환영합니다!

Adobe Campaign Standard 사용자가 이제 Adobe Campaign Managed Cloud Services v8로 전환할 수 있음을 발표하게 되어 기쁘게 생각합니다. 이러한 전환은 다음과 같은 많은 이점을 제공합니다.

* 강력한 IT 인프라: 관리 Cloud Service v8을 통해 고객은 보다 강력한 IT 인프라를 활용하여 캠페인에 대한 성능, 안정성 및 확장성을 향상시킬 수 있습니다.
* 향상된 지원: 당사의 관리 Cloud Service 팀은 귀하의 플랫폼을 원활하게 전환하고 지속적으로 모니터링할 수 있도록 최고 수준의 지원을 제공하기 위해 최선을 다하고 있습니다. 문제 해결에서 사전 유지 관리에 이르기까지 모든 문제를 해결해 드립니다.
* Adobe Experience Platform과 통합: 관리 Cloud Service v8은 Adobe Experience Platform과 원활하게 연결되어 고객이 데이터의 모든 잠재력을 활용하고 채널 전반에 개인화되고 영향력 있는 캠페인을 제공할 수 있습니다.
* 일관된 사용자 인터페이스 및 경험: 관리 Cloud Service v8로 전환해도 워크플로우가 중단되지 않으므로 안심할 수 있습니다. 친숙한 사용자 인터페이스와 사용자 경험을 계속 활용하여 팀에 대한 최소한의 학습 곡선을 보장할 수 있습니다.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 주요 기능 {#key-features}

Campaign v8이 제공하는 주요 기능에 대해 자세히 알아보겠습니다.

* 현대적이고 친근하며 통합된 경험. [자세히 알아보기](../get-started/connect-to-campaign.md)
* 새로운 강력한 기능과 원활한 프로세스 [자세히 알아보기](../get-started/user-interface.md)
* 단순하고 직관적인 새 쿼리 모델러입니다. [자세히 알아보기](../query/query-modeler-overview.md)
* 내장된 크로스 채널 캠페인 관리 기능. [자세히 알아보기](../msg/gs-messages.md)
* 새롭고 재설계된 캠페인 워크플로우 활동. [자세히 알아보기](../workflows/gs-workflows.md)
* 쿼리 모델러를 사용하여 대상자를 타깃팅합니다. [자세히 알아보기](../query/query-modeler-overview.md)
* 간편한 프로필 생성 및 관리 [자세히 알아보기](../audience/about-recipients.md)
* 사전 정의된 필터. [자세히 알아보기](../get-started/predefined-filters.md)
* 이메일 디자인용 HTML 변환기. [자세히 알아보기](../email/existing-content.md)
* 오퍼가 있는 SMS. [자세히 알아보기](../msg/offers.md)

## 콘솔 및 웹 인터페이스 {#console}

Campaign v8 사용자는 새로운 Campaign 웹 인터페이스와 v8 콘솔 모두에 액세스할 수 있습니다. 데이터와 설정은 한 환경에서 다른 환경으로 동기화됩니다. 클라이언트 콘솔에서 사용할 수 있는 모든 데이터와 설정은 Explorer 왼쪽 탐색에서 Campaign 웹 사용자 인터페이스에 표시됩니다. [자세히 알아보기](../get-started/user-interface.md#user-interface-explorer)

Campaign 웹 사용자 인터페이스와 Campaign 클라이언트 콘솔 간의 지원 및 지원되지 않는 기능 및 상호 운용성 [이 페이지에서](../get-started/capability-matrix.md)

## Terminology {#terminology}

대부분의 개념은 Campaign 웹 인터페이스와 Campaign Standard 간에 유사합니다. 그러나 몇 가지 차이점이 있습니다. 다음은 Campaign Standard과 Campaign 웹 인터페이스 간의 용어 차이점에 대한 몇 가지 예입니다.

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* 사용자 지정 리소스는 다음과 같습니다 **스키마** Campaign 웹 사용자 인터페이스에서 다음을 수행합니다.
* 마케팅 활동이 더 이상 존재하지 않습니다.
* 메시지: **게재**.
* 연산자는 **사용자**.
* 명명된 권한: **역할**.
* 연산자 그룹은 다음과 같습니다 **보안 그룹**.
* 폴더 권한은 **조직 단위**

## 새로운 기능 {#new-features}

전환할 수 있도록 다음을 추가했습니다. [주요 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) Campaign Standard에서 v8까지:

* **다이내믹 보고**: 동적 보고는 마케팅 활동의 영향을 측정하기 위한 사용자 지정 및 실시간 보고서를 제공합니다. 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 실용적인 이메일 캠페인 데이터 외에도 성별, 도시 및 연령 등의 프로필 차원별 인구 통계 분석을 활성화합니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **중앙 집중식 브랜딩**: 모든 회사에는 브랜드 시각적 및 기술적 지침이 있습니다. Adobe Campaign을 사용하면 로고부터 이메일 발신자, URL 또는 도메인과 같은 기술적 측면까지 일관된 브랜드를 고객에게 제시하기 위해 일련의 사양을 정의할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **나머지 API** - Campaign Stardard를 마이그레이션한 사용자는 Rest API를 사용하여 Adobe Campaign을 위한 통합을 만들고 사용 중인 기술 패널과 Adobe Campaign을 연결하여 고유한 에코시스템을 구축할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **랜딩 페이지** - Campaign v8에서는 기능을 잃지 않도록 많은 기능이 개선되었습니다. 다음에서 자세히 알아보기 [릴리스 정보](../rn/release-notes.md#new-24-4) 및 랜딩 페이지 [설명서](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->