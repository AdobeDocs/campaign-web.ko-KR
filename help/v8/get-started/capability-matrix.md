---
audience: end-user
title: Campaign Web 사용자 인터페이스/클라이언트 콘솔 기능 매트릭스
description: Campaign Web 사용자 인터페이스에서 지원되는 기능 목록
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '2134'
ht-degree: 100%

---

# Campaign Web 및 Campaign 클라이언트 콘솔 {#capabilities-matrix}

Campaign Web 사용자 인터페이스에서 주요 캠페인 기능을 사용할 수 있습니다. 이 인터페이스는 주로 마케팅 담당자가 마케팅 캠페인을 계획, 실행 및 측정할 수 있도록 설계되었습니다. 모든 기능은 [이 페이지](../rn/whats-new.md)에 나열되어 있습니다.

비즈니스 및 데이터 요구 사항에 따른 Campaign 플랫폼 사용자 정의 및 다른 시스템에 대한 연결은 Campaign 클라이언트 콘솔에서 관리됩니다. 결과적으로 일부 설정 및 기능은 Campaign 클라이언트 콘솔에서만 액세스하거나 만들거나 관리할 수 있습니다. 일부 기능은 Campaign Web 사용자 인터페이스의 향후 업데이트에서 사용할 수 있습니다.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 캠페인 관리 {#campaign-mgt-capabilities}

Campaign Web 사용자 인터페이스를 통해 [이 섹션](../campaigns/gs-campaigns.md)에서 자세히 설명하는 바와 같이 크로스 채널 캠페인을 만들 수 있습니다. 다음 기능은 Campaign 클라이언트 콘솔에서만 사용할 수 있습니다. Campaign Web 사용자 인터페이스에서는 액세스할 수 없지만 일부는 [탐색기 메뉴](user-interface.md#user-interface-explorer)에 보일 수도 있습니다.

Campaign v8(클라이언트 콘솔) 설명서를 찾아보고 이 기능을 사용하는 방법을 알아보려면 제공된 링크를 사용하십시오.

* **마케팅 캘린더**. 캠페인 캘린더에는 모든 프로그램, 기획, 캠페인, 게재가 통합 타임라인으로 표시됩니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=ko#campaign-calendar){target="_blank"}
* **프로그램 및 기획**. 각 캠페인은 프로그램에 속하며, 프로그램은 기획에 속합니다. Campaign Web 사용자 인터페이스에서 모든 캠페인은 기본 제공되는 플랜 및 프로그램과 연결되어 있습니다. 클라이언트 콘솔에서만 기획과 프로그램을 만들고 관리할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=ko#work-with-plan-and-program){target="_blank"}
* **공급자, 예산, 비용 관리**. 캠페인 내에서 수행하는 작업에 참여하는 서비스 공급자를 구성(비용 구조 포함)하고 각 프로그램 및 캠페인 내에서 예산을 관리할 수 있습니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=ko){target="_blank"}
* **분산 마케팅**(중앙/로컬 마케팅). Adobe Campaign에서는 중앙 엔티티(본사, 마케팅 부서 등)와 로컬 엔티티(매장, 지역 대리점 등) 간 협력 캠페인을 구현하는 데 사용할 수 있는 분산 마케팅 앱을 제공합니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=ko){target="_blank"}
* **마케팅 리소스 관리**(MRM), 목표, 시뮬레이션, 원가 관리. Adobe Campaign은 관련 작업, 예산, 마케팅 리소스에 대한 완전한 관리 및 실시간 추적으로 공동 작업 모드에서 마케팅 액션을 제어할 수 있는 마케팅 리소스 관리(MRM) 앱을 제공합니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=ko){target="_blank"}
* **작업 관리**. MRM 앱의 일부로 Campaign 작업을 캠페인 대시보드에서 만들고 할당, 추적, 모니터링할 수 있습니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=ko){target="_blank"}

## 커뮤니케이션 채널 {#channels-capabilities}

Campaign Web 사용자 인터페이스를 통해 [이 섹션](../msg/gs-messages.md)에서 자세히 설명하는 바와 같이 **이메일**, **SMS**, **푸시 알림**, **다이렉트 메일**&#x200B;을 만들고 디자인하고 보내며 그 효과를 다양한 전용 보고서로 측정할 수 있습니다. 다만, 현재 인앱, LINE, 콜센터/사용자 정의 채널, X(Twitter)를 통한 소셜 마케팅 채널은 사용이 **불가능**&#x200B;합니다.

Campaign v8(클라이언트 콘솔) 설명서를 찾아보고 이 채널에 대해 자세히 알아보려면 제공된 링크를 사용하십시오.

* **LINE 메시지**. LINE은 모든 모바일 디바이스와 PC에서 사용할 수 있는 무료 인스턴트 메시지, 음성 및 영상 통화용 애플리케이션입니다. Adobe Campaign의 경우 클라이언트 콘솔에서만 LINE 메시지를 보낼 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=ko){target="_blank"}
* **콜센터 및 사용자 정의 채널**. Campaign 환경에 콜센터 및 기타 사용자 정의 채널을 구현할 수 있습니다. 이 채널은 클라이언트 콘솔에서만 사용할 수 있습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=ko#other-channels){target="_blank"}
* X(Twitter) **소셜 마케팅**. X(Twitter)를 통해 메시지를 게시하고 DM을 보내 고객과 소통합니다. 소셜 마케팅 추가 기능과 함께 제공되는 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=ko){target="_blank"}

## 랜딩 페이지 및 웹 애플리케이션 {#Webapps-capabilities}

Adobe Campaign을 사용하면 랜딩 페이지를 만들고, 디자인하고, 공유할 수 있습니다. 새로운 인터페이스에서는 랜딩 페이지 경험이 완전히 새로워졌습니다. [이 섹션](../landing-pages/get-started-lp.md)에서 Campaign Web 사용자 인터페이스의 랜딩 페이지를 생성, 디자인 및 게시하는 방법을 알아보십시오.

결과적으로 Campaign 클라이언트 콘솔에서는 웹 인터페이스에서 생성된 랜딩 페이지를 편집, 업데이트 또는 수정할 수 없으며 그 반대의 경우도 마찬가지입니다. 다음 유형의 웹 애플리케이션은 Campaign Web 사용자 인터페이스에서 사용할 수 없습니다. 단, 랜딩 페이지 목록에는 표시됩니다. 제공된 링크를 사용하여 Campaign Classic v7 설명서를 찾아보고 다음 웹 앱에 대해 자세히 알아보십시오.

* **웹 애플리케이션**. Adobe Campaign을 사용하면 데이터베이스에서 미리 로드된 데이터와 연결된 사용자의 권한에 맞게 조정된 콘텐츠를 사용하여 동적 및 대화형 웹 애플리케이션을 만들고 게시할 수 있습니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=ko){target="_blank"}
* **웹 폼**. 클라이언트 콘솔에서 디자인된 웹 및 랜딩 페이지는 Campaign Web 사용자 인터페이스에 표시되지만 편집하거나 수정할 수는 없습니다. 클라이언트 콘솔 웹 페이지 디자이너와 Campaign Web 사용자 인터페이스와 함께 제공되는 랜딩 페이지 디자이너 간에 일부 옵션이 다를 수 있습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=ko){target="_blank"}
* **온라인 설문 조사**. 온라인 설문 조사를 만들고 클라이언트 콘솔에서만 답변을 수집할 수 있습니다. Campaign Web 사용자 인터페이스에서는 이 기능을 사용할 수 없습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=ko){target="_blank"}

## 프로필, 테스트 프로필 및 대상자 {#profiles-audiences-capabilities}

Campaign 클라이언트 콘솔과 Campaign Web 사용자 인터페이스 모두에서 프로필과 테스트 프로필을 생성, 관리 및 업데이트할 수 있습니다. 한 인터페이스에서 수행된 모든 변경 사항은 다른 인터페이스에서 볼 수 있습니다. 단, 일부 특정 수신자 설정 및 고급 매개변수는 새 Campaign Web 사용자 인터페이스에서 누락될 수 있습니다.

새 웹 사용자 인터페이스에서는 “수신자”라는 용어가 “프로필”로 변경되었으며 “시드 주소”는 이제 “테스트 프로필”입니다.

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Campaign 클라이언트 콘솔 또는 Adobe Experience Platform에서 만든 모든 대상자는 Campaign Web 사용자 인터페이스에서 사용할 수 있습니다.

[Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=ko#import-jobs){target="_blank"}에 나온 것과 같은 일회성 가져오기/내보내기 작업은 Campaign Web 사용자 인터페이스에서 사용할 수 없습니다. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## 콘텐츠 디자인 {#content-capabilities}

Adobe Campaign Web 사용자 인터페이스와 함께 제공되는 새로운 [이메일 디자이너]를 사용하면 직관적인 드래그 앤 드롭 인터페이스를 통해 시선을 사로잡는 개인 맞춤형 이메일을 쉽게 만들 수 있습니다. 처음부터 빈 화면으로 시작하고 기존 콘텐츠를 가져오거나 기존 템플릿을 활용하는 경우 모든 이메일 콘텐츠를 디자인하고 세부적으로 조정할 수 있습니다. [자세히 알아보기](../email/edit-content.md)

이 새로운 사용자 인터페이스를 사용하면 Adobe Experience Manager에서 이메일 템플릿 동기화를 관리하고 Adobe Experience Manager as a Cloud Service와 통합할 수 있습니다.

현재 Campaign Web 사용자 인터페이스에서는 다음 기능을 사용할 수 없다는 점에 유의하십시오. Campaign v8(클라이언트 콘솔) 설명서를 찾아보고 이 기능에 대해 자세히 알아보려면 제공된 링크를 사용하십시오.

* **사용자 정의 개인화 블록 만들기**. 기본 개인화 블록 외에도 클라이언트 콘솔에서 사용자 정의 블록을 만들 수 있습니다. Campaign Web 사용자 인터페이스에서는 이 기능을 사용할 수 없습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=ko#create-custom-personalization-blocks){target="_blank"}
* **사용자 정의 양식의 콘텐츠**. [콘텐츠 관리] 모듈을 사용하면 사용자가 Campaign에서 콘텐츠를 만들 때 도움이 되는 양식을 만들고 관리할 수 있습니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=ko){target="_blank"}
* **이메일용 AMP**. 이메일용 AMP 포맷을 사용하면 메시지에 AMP 구성 요소를 포함하여 풍부하고 실행 가능한 콘텐츠로 이메일 경험을 개선할 수 있습니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [Campaign Classic v7 설명서에서 자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=ko){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 유형화 및 유형화 규칙 {#rules-capabilities}

유형화는 특정 게재에 여러 필터링 규칙을 한 번에 쉽게 적용하기 위해 준비 단계에서 실행되는 유형화 규칙 세트입니다. 이 기능으로 마케터가 게재 발송을 제어, 필터링하고 우선 순위를 지정하여 모든 게재에 걸쳐 비즈니스 관행을 표준화할 수 있습니다.

유형화 규칙은 [이 섹션](../advanced-settings/delivery-settings.md#typology)에서 자세히 설명하는 바와 같이 Campaign Web 사용자 인터페이스에서 게재 또는 게재 템플릿에 대해 선택할 수 있습니다. 단, 규칙 및 유형 규칙 만들기, 관리, 사용자 정의는 Campaign 클라이언트 콘솔에서만 가능합니다.

Campaign v8(클라이언트 콘솔) 설명서를 찾아보고 유형 규칙에 대해 자세히 알아보려면 제공된 링크를 사용하십시오.

<!--
* Control rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
-->
* 피로도/압력 규칙 만들기. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}
<!--
* Filtering rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Typology rules management. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
-->
* 캠페인 시뮬레이션. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
<!--
* JavaScript coding for typology rules authoring. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}
-->

## 워크플로 {#wf-capabilities}

새로운 Campaign Web 사용자 인터페이스는 프로세스를 디자인하고 관리할 수 있도록 재구성된 워크플로 캔버스 인터페이스를 제공합니다. 주요 워크플로 활동은 이미 새로운 디자인으로 사용할 수 있으며 일부는 향후 업데이트에서 제공될 예정입니다. 가드레일 및 제한 사항 등 워크플로 기능에 대한 자세한 정보는 [이 섹션](../get-started/guardrails.md)을 참조하십시오.

다음 기능은 Campaign 클라이언트 콘솔에서만 사용할 수 있다는 점에 유의하십시오.

<!--
* Scripting in workflows
-->

* ETL 활동: 내보내기, 스키마 편집, 데이터 로드, 데이터 추출, SQL 코드

사용 가능한 워크플로 활동에 대한 자세한 내용은 [여기](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=ko){target="_blank"}에 있는 Adobe Campaign v8(콘솔) 워크플로 설명서를 참조하십시오.

## 오퍼 관리 {#offer-capabilities}

Adobe Campaign Web 사용자 인터페이스에서 만든 게재를 통해 오퍼를 보낼 수 있습니다. 이 오퍼는 클라이언트 콘솔에서 **[!UICONTROL 상호 작용]** 모듈을 사용하여 만들어야 합니다. 오퍼 디자인, 적격성 규칙, 오퍼 관리는 Campaign 클라이언트 콘솔에서만 할 수 있습니다. [자세히 알아보기](../msg/offers.md)

오퍼 카탈로그를 관리하는 방법은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=ko){target="_blank"}를 참조하십시오.

## Adobe Experience Cloud 솔루션과 통합 {#exc-capabilities}

새로운 Campaign 최신 UI는 Adobe Experience Platform 및 Adobe Experience Manager를 비롯한 다른 Adobe 솔루션과 함께 마케팅 캠페인 디자인 및 게재를 간소화하고 일관성을 제공합니다.

다음 통합 기능은 Adobe Campaign 클라이언트 콘솔에서 사용할 수 있으며 Campaign Web 사용자 인터페이스에서는 아직 사용할 수 없습니다. Campaign v8(클라이언트 콘솔) 설명서를 찾아보고 이 통합에 대해 자세히 알아보려면 제공된 링크를 사용하십시오.

* Adobe Analytics 데이터 사용 및 KPI 공유. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=ko){target="_blank"}
* Adobe Experience Cloud(Adobe Audience Manager)를 통한 대상자 공유. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=ko){target="_blank"}
* Adobe Target과 통합. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=ko){target="_blank"}
* Adobe Experience Cloud 트리거와 통합. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=ko){target="_blank"}

## 보고 {#reporting-capabilities}

새로운 Campaign Web 사용자 인터페이스에는 게재 보고서, 캠페인 보고서, 글로벌 보고서 등 모든 채널에 대한 새로운 보고서 및 KPI 세트가 함께 제공됩니다. [이 섹션에서](../reporting/gs-reports.md) 자세히 알아보기

일부 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=ko){target="_blank"}를 찾아보고 자세히 알아보려면 제공된 링크를 탐색하십시오.

* 기본 제공 전달성 보고서 및 받은 편지함 렌더링. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=ko){target="_blank"}
* 보고 사용자 정의. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=ko){target="_blank"}
* 기술 분석. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=ko){target="_blank"}
* 캠페인 분석/큐브 보고서. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=ko){target="_blank"}
* PDF, CSV 또는 링크로 공유 예약 보고. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=ko){target="_blank"}

## 데이터 모델링 및 데이터 수집 {#data-capabilities}

Campaign Web 사용자 인터페이스에는 다음 기능이 표시되지 않습니다. 클라이언트 콘솔에서만 사용할 수 있습니다.

### 외부 계정 {#external}

Adobe Campaign에는 외부 시스템과 연결하기 위해 사전 정의된 외부 계정 세트가 함께 제공됩니다. Campaign 시스템 관리자는 외부 계정을 만들고 관리할 수 있습니다. [자세히 알아보기](../administration/external-account.md)

### 스키마 만들기 및 확장 {#schema}

스키마를 만들고 수정 및 확장하는 작업은 고급 사용자만 가능합니다. 이 기능은 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=ko){target="_blank"}

### 워크플로 데이터 관리 기능 {#data}

데이터 관리는 데이터 로드, 추출(파일), 데이터 업데이트, 스키마 편집 또는 가져오기/내보내기 기술 워크플로와 같은 보다 효율적이고 유연한 도구를 제공하여 복잡한 타기팅 문제를 해결하기 위한 일련의 활동을 결합합니다. [클라이언트 콘솔에서 워크플로 데이터 관리 기능 살펴보기](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=ko#data-management){target="_blank"}

>[!NOTE]
>
>이들 활동 중 일부는 클라이언트 콘솔에서만 사용할 수 있지만 **데이터 보강**, **파일 로드**, **데이터 소스 변경** 또는 **차원 변경** 활동 등 일부는 Campaign Web 사용자 인터페이스에서 사용할 수 있습니다. [Campaign Web 사용자 인터페이스의 타기팅 및 데이터 관리 활동에 대해 자세히 알아보기](../workflows/activities/about-activities.md#targeting)

### 페더레이션 데이터 액세스(FDA) 구성 {#fda}

Campaign 구성 및 외부 시스템에 대한 연결은 고급 사용자로 제한되며 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=ko){target="_blank"}

## 승인 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="승인 관리"
>abstract="승인 관리는 클라이언트 콘솔에서만 사용할 수 있습니다. "

Campaign Web 사용자 인터페이스에는 콘텐츠, 게재, 워크플로, 캠페인, 대상에 대한 승인 관리가 표시되지 않습니다. 클라이언트 콘솔에서만 사용할 수 있습니다.

워크플로의 승인을 관리하는 방법은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=ko){target="_blank"}를 참조하십시오.

캠페인의 게재, 콘텐츠, 대상 승인을 관리하는 방법은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=ko){target="_blank"}를 참조하십시오.

## 권한 {#permissions-capabilities}

Campaign 사용자는 Adobe ID를 사용해서만 Campaign Web 사용자 인터페이스에 Adobe Identity Management System(IMS)를 통해 액세스할 수 있습니다. 사용자에게 부여된 권한은 Campaign Web 사용자 인터페이스에도 적용됩니다.

권한은 [이 섹션에서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=ko) 자세히 설명하는 바와 같이 Adobe Admin Console 및 Adobe Campaign 클라이언트 콘솔에서 정의합니다. Adobe Campaign Web 사용자 인터페이스에서는 권한에 대한 작업이 불가능합니다.

## 모니터링 {#monitoring-capabilities}

Campaign 플랫폼 모니터링 기능은 클라이언트 콘솔과 Campaign [컨트롤 패널]에서만 사용할 수 있습니다. Campaign Web 사용자 인터페이스에는 표시되지 않습니다.

자세히 알아보려면 제공된 Campaign v8(클라이언트 콘솔) 설명서 및 [컨트롤 패널] 설명서 링크를 찾아보십시오.

* [워크플로 모니터링](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=ko){target="_blank"}
* [워크플로 히트맵](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=ko){target="_blank"}
* [성능 모니터링](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=ko){target="_blank"}
* [전달성 모니터링](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=ko){target="_blank"}

## 시간대 관리 {#timezone-management}

Adobe Campaign Web UI는 **사용자 웹 브라우저의 현지 시간대**&#x200B;를 바탕으로 모든 날짜와 시간 값을 표시합니다. 이로 인해 웹 UI 및 클라이언트 콘솔 간 타임스탬프 비교 시에 차이가 발생할 수 있습니다.

이 [페이지](../administration/timezone-management.md)를 참조하여 **웹 UI**, **클라이언트 콘솔** 및 **워크플로 실행** 시간대 간 차이점에 대해 자세히 알아보십시오.
