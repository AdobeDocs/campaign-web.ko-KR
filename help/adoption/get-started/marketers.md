---
title: 마케터를 위한 Adobe Campaign v8 시작
description: Campaign v8의 주요 기능을 살펴보십시오. Campaign Standard에서 Campaign v8로 마이그레이션하는 마케터를 위한 것입니다.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 18%

---

# 마케터를 위한 시작 튜토리얼 {#acs-gs-marketers}

이 안내서에서는 Campaign Standard에서 Campaign v8로 전환하는 마케터를 위해 Campaign v8의 주요 기능에 대한 개요를 제공합니다.

클라이언트 콘솔 또는 웹 사용자 인터페이스를 통해 Adobe Campaign v8에 액세스할 수 있습니다. 웹 인터페이스를 사용하면 주요 마케팅 작업을 생성, 관리 및 실행할 수 있습니다. 새로운 Adobe Campaign Web 인터페이스는 현대적이고 직관적인 사용자 경험을 제공하여 마케팅 캠페인 디자인 및 게재를 간소화합니다. [자세히 알아보기](../../v8/get-started/user-interface.md).

마이그레이션을 통해 Campaign Standard의 모든 데이터를 Campaign v8로 가져와 진행 중인 작업에 대한 중단을 최소화하면서 원활하게 전환할 수 있습니다.

기존 자격 증명을 계속 사용하여 로그인하고 새 Adobe Campaign v8 인스턴스에 연결할 수 있습니다. 로그인하고 나면 마이그레이션 중인 모든 프로필 및 워크플로를 찾을 수 있으므로 캠페인을 계속 진행할 수 있습니다.

가장 큰 차이점은 사용자 인터페이스입니다. 아래에서는 두 인터페이스의 동일한 워크플로우를 비교합니다.

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign 웹 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 제공 모델에서 작동합니다. [릴리스 정보](../../v8/rn/release-notes.md)에서 최신 업데이트를 정기적으로 확인하십시오.

## Campaign 웹 사용자 인터페이스 살펴보기 {#acs-gs-marketers-ui}

아래 비디오에서 Campaign 웹 사용자 인터페이스에 액세스하고 탐색하는 방법과 인벤토리 목록을 사용자 지정하는 방법을 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3453429?quality=12&learn=on&captions=kor){transcript=true}

자세한 내용은 아래 설명서를 참조하십시오.

1. [Campaign 웹 사용자 인터페이스 살펴보기](../../v8/get-started/user-interface.md)

1. [목록 찾아보기 및 필터링](../../v8/get-started/list-filters.md)


## 프로필 및 대상자 만들기 및 관리 {#acs-gs-marketers-profiles-and-audiences}

Campaign v8에서 프로필 및 대상을 만들고 관리하기 위한 일반적인 개념은 Adobe Campaign Standard과 동일합니다. [이 섹션](../../v8/audience/gs-audiences-recipients.md)에서 프로필 및 대상자로 시작하는 방법을 알아봅니다.

시작할 수 있는 몇 가지 유용한 링크를 아래에서 확인할 수 있습니다.

### 프로필 관리 {#acs-gs-marketers-profiles}

Adobe Campaign에서 프로필은 데이터베이스에 저장된 레코드이며, 게재 대상을 만들고 콘텐츠에 개인화 데이터를 추가하는 주요 구성 요소 역할을 합니다.

1. 이 비디오에서는 Campaign 웹 사용자 인터페이스를 사용하여 프로필에 액세스, 관리 및 탐색하는 방법을 알아봅니다.

   >[!VIDEO](https://video.tv.adobe.com/v/3448371?quality=12&learn=on&captions=kor){transcript=true}

   [프로필 시작](../../v8/audience/about-recipients.md) 설명서에서 자세히 알아보세요.

1. Campaign v8에서 [테스트 프로필을 만들고 관리](../../v8/audience/test-profiles.md)하는 방법을 알아봅니다.

### 대상자 관리 {#acs-gs-marketers-audiences}

대상자는 유사한 행동 및/또는 특성을 공유하는 프로필 세트입니다. 이러한 사용자 컬렉션은 생성하거나 선택하거나 로드할 수 있습니다.  대상자를 생성한 후에는 게재의 대상 집단으로 활용할 수 있습니다.

이 비디오에서는 대상을 빌드 및 관리하고, 게재할 대상을 선택하고, 컨트롤 그룹을 정의하는 방법에 대해 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3453209?quality=12&learn=on&captions=kor){transcript=true}

자세한 내용은 [대상자 시작](../../v8/audience/manage-audience.md){target="_blank"}을 참조하세요.

Campaign Standard에서와 같이 게재에 컨트롤 그룹을 추가할 수 있습니다. 대상자의 일부에 메시지를 보내지 않도록 컨트롤 그룹을 정의하고 게재 후 동작을 기본 대상과 비교할 수 있습니다. 이 옵션은 캠페인의 영향을 측정하는 데 도움이 됩니다.
[컨트롤 그룹을 설정](../../v8/audience/control-group.md){target="_blank"}하는 방법을 알아보세요.

>[!AVAILABILITY]
>
>* Campaign Standard 쿼리 활동을 통해 만든 모든 대상자는 전환 중에 Campaign v8의 사전 정의된 필터로 변환됩니다. Campaign v8은 쿼리 활동도 지원합니다.
>
>* 읽기 대상은 [사전 정의된 필터](../../v8/query/build-query.md)를 사용하여 쿼리 활동으로 변환됩니다.
>
>* 사전 정의된 필터는 Campaign v8로 대상을 마이그레이션한 후에만 최신 값을 사용합니다.
>
>* Campaign Standard의 파일 유형 대상은 차원 없이 목록 유형으로 마이그레이션됩니다.

### 구독 관리 {#acs-gs-marketers-sub}

뉴스레터와 같은 서비스를 관리 및 생성하고, 이러한 서비스에 대한 구독 또는 구독 취소를 확인할 수 있습니다. 주요 단계는 Campaign Standard과 동일하게 전역적입니다. 자세한 내용은 아래 페이지를 참조하세요.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="저빈도" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>구독 서비스 만들기</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="저빈도" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>구독자 관리<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="유효성 검사" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/send-to-subscribers"><strong>서비스 구독자에게 메시지 보내기</strong></a>
</div>
<p>
</td>
</tr>
</table>

## 계획, 프로그램 및 캠페인 사용 {#acs-gs-marketers-plans}

Adobe Campaign v8을 사용하면 마케팅 계획 및 프로그램에 대한 폴더 계층 구조를 구성할 수 있습니다. 계획, 프로그램 및 캠페인 기능은 Campaign Standard 및 Campaign v8과 유사합니다.

자세한 내용은 [계획 및 프로그램 설명서](../../v8/administration/plans-programs.md)를 참조하세요.

시작하는 데 유용한 링크를 아래에서 찾을 수 있습니다. 사용자 경험에 영향을 줄 수 있는 변경 사항은 가용성 노트에서 강조 표시됩니다.


### 캠페인 만들기 {#acs-gs-marketers-campaign}

Adobe Campaign을 사용하면 내장된 캠페인 관리 기능을 사용하여 타깃팅된 마케팅 이니셔티브를 손쉽게 오케스트레이션할 수 있습니다. 예약을 정의하는 기능을 사용하여 전략적 목표에 맞게 캠페인 기간 및 시기를 계획하고 대상자 참여를 극대화할 수 있습니다.

![캠페인 흐름](assets/campaign-flow.png)

캠페인에 대한 자세한 내용은 아래 설명서를 참조하십시오.

1. [캠페인 시작하기](../../v8/campaigns/gs-campaigns.md)
1. [캠페인 액세스 및 관리](../../v8/campaigns/manage-campaigns.md)
1. [첫 캠페인 만들기](../../v8/campaigns/create-campaigns.md)


### 워크플로 만들기 {#acs-gs-marketers-wf}

워크플로우 사용자 인터페이스는 사용, 구성, 실행 및 문제 해결을 용이하게 하기 위해 Campaign 웹 사용자 인터페이스에서 완전히 다시 상상되었습니다. 워크플로우를 통해 Campaign Standard에서 이미 경험했듯이 전체 프로세스 및 작업을 오케스트레이션하고, 세그먼트 만들기, 메시지 준비에서 게재에 이르기까지 마케팅 캠페인의 모든 측면에 대한 속도와 규모를 개선할 수 있습니다. 또한 캠페인 오케스트레이션을 위해 사용하기 쉬운 단일 인터페이스로 채널을 동기화할 수 있습니다.

이 비디오에서는 워크플로우의 작동 방식과 타겟팅 워크플로우를 만드는 방법을 이해합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3453979?quality=12&learn=on&captions=kor){transcript=true}

자세한 내용은 [워크플로 설명서](../../v8/workflows/gs-workflows.md)를 참조하세요.

Adobe Campaign 웹 사용자 인터페이스에서는 다양한 기준을 기반으로 데이터베이스를 필터링하는 프로세스를 간소화하는 워크플로우의 쿼리 모델러를 제공합니다. [쿼리 모델러에 대해 자세히 알아보기](../../v8/query/query-modeler-overview.md)

워크플로우 내의 각 활동의 목적과 기능을 이해하려면 [워크플로우 활동](../../v8/workflows/activities/about-activities.md)에서 사용할 수 있는 자세한 정보를 살펴보십시오

[워크플로에 대한 보호 기능 및 제한 사항](../../v8/get-started/guardrails.md)을 검토하여 워크플로의 효율성을 극대화하십시오.

>[!AVAILABILITY]
>
>* 워크플로우 실행 [기록 및 로그](../../v8/workflows/start-monitor-workflows.md#logs-tasks)는 Adobe Campaign v8에서 사용할 수 있습니다.
>
>* Campaign Standard 인스턴스에서 실행된 워크플로의 기록 로그는 Campaign v8로 마이그레이션되지 않습니다.
>
>* 조직 단위는 매핑하고 유사한 액세스 제어를 보장하기 위해 폴더 개념에 매핑됩니다.
>

## 게재 만들기 및 관리 {#acs-gs-marketers-deliveries}

마케터는 Campaign 웹 사용자 인터페이스를 사용하여 **게재** 왼쪽 메뉴에서 독립 실행형 게재를 만들거나 워크플로우의 컨텍스트에서 게재를 만들 수 있습니다(캠페인에 포함되거나 포함되지 않음). 주요 단계는 Campaign Standard의 이전 경험과 일치합니다. [게재 만들기 및 관리 설명서](../../v8/msg/gs-deliveries.md) 섹션에서 게재를 만드는 방법을 알아보세요.

유용한 링크:

* **게재 템플릿** - 디자인 프로세스를 가속화하고 개선하기 위해 게재 템플릿을 만들어 캠페인 전반에서 사용자 지정 콘텐츠 및 설정을 쉽게 재사용할 수 있습니다. 이 기능을 사용하면 크리에이티브 룩과 느낌을 표준화하여 캠페인 실행 및 실행을 보다 신속하게 수행할 수 있습니다./[게재 템플릿](../../v8/msg/delivery-template.md) 페이지에서 자세히 알아보세요.

* **게재 설정** - 게재 설정은 게재 템플릿에 정의된 기술 게재 매개 변수입니다. 각 게재에 대해 오버로드될 수 있습니다. 이러한 설정은 게재 또는 게재 템플릿을 편집할 때 사용할 수 있는 설정 버튼에서 사용할 수 있습니다. 자세한 내용은 [게재 설정](../../v8/advanced-settings/delivery-settings.md) 섹션을 참조하세요.

* **다이내믹 콘텐츠** - Adobe Campaign Web 다이내믹 콘텐츠 기능을 사용하면 수신자에 대해 수집한 정보를 기반으로 콘텐츠를 사용자 지정할 수 있습니다. 다이내믹 콘텐츠를 활용하여 원치 않거나 불필요한 제품 또는 서비스 마케팅을 방지하면서 마케팅 활동의 관련성을 높일 수 있습니다. [다이내믹 콘텐츠](../../v8/personalization/gs-personalization.md) 섹션에서 자세히 알아보세요.

* **테스트 및 증명** - 게재 콘텐츠가 정의되면 프로필 및 테스트 프로필을 사용하여 메시지를 보내기 전에 미리 보고 테스트할 수 있습니다. 이 단계는 정확하지만 컨텐츠 및 개인화 설정 모두에서 오류가 없는지 확인하는 데 중요합니다. [미리 보기 및 테스트](../../v8/preview-test/preview-test.md)를 참조하세요.

* **예약** - 메시지를 보낼 날짜와 정확한 시간을 설정할 수 있습니다. 마케팅 메시지에 가장 적합한 시간을 선택하면 열람율을 극대화할 수 있습니다.

   * [독립 실행형 게재를 예약하는 방법](../../v8/msg/gs-deliveries.md#gs-schedule) 알아보기
   * 워크플로우에서 [게재를 예약하는 방법](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow) 알아보기

* **오퍼 추가** - Adobe Campaign 웹 사용자 인터페이스에서 게재에 오퍼를 추가할 수 있습니다. 이러한 오퍼는 오퍼 목록에 액세스할 수 있는 오퍼 왼쪽 메뉴에서 사용할 수 있습니다.  [메시지에 오퍼 추가](../../v8/msg/offers.md)하는 방법을 알아보세요.

>[!AVAILABILITY]
>
>* 초안 상태 또는 완료됨 상태의 게재가 마이그레이션되었습니다.
>
>* 다음 상태 중 하나에 있는 게재가 Adobe Campaign v8로 마이그레이션되었지만 다시 준비해야 합니다. 전송 중 / 진행 중 / 취소됨 / 재시도 진행 중 / 준비 오류.
>
>* 다음 상태 중 하나의 게재가 취소된 게재로 마이그레이션되었습니다. (취소됨/다시 시도 진행 중).
>
>* 추적 링크, 미러 페이지 URL 링크, 구독/구독 취소 링크는 Campaign Standard에서와 같이 작동합니다.
>
>Adobe Campaign의 [추적 및 모니터링](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [브랜딩](https://experienceleague.adobe.com/ko/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} 섹션도 참조하세요.

### 이메일 게재 {#acs-gs-marketers-email}

이 비디오에서 이메일 게재를 처음부터 새로 만들고, 대상자를 정의하고, 콘텐츠를 디자인하고, 미리 보기를 시뮬레이트하고, 증명을 보내는 방법을 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3454012?quality=12&learn=on&captions=kor){transcript=true}

[첫 번째 전자 메일 문서 만들기](../../v8/email/create-email.md)에서 첫 번째 대상 전자 메일을 만드는 방법을 알아봅니다

Campaign v8에서 이메일 게재를 만들고, 테스트하고, 전송하는 자세한 단계는 Campaign Standard과 유사합니다.

1. **콘텐츠 디자인 및 정의**

   Campaign v8 이메일 디자이너는 Campaign Standard에서 사용할 수 있는 디자이너와 유사합니다. 몇 년 전 Campaign Standard[기존 전자 메일 편집기는 더 이상 사용되지 않습니다](https://experienceleague.adobe.com/ko/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}. 이메일 콘텐츠를 만들고 개인화하려면 이미 Campaign 이메일 Designer으로 전환했어야 합니다.

   이메일 디자이너를 탐색하는 방법을 이해합니다. 다음 비디오에서는 이메일을 처음부터 구조화하고 디자인하는 방법, 이메일을 개인화하고 테스트하는 방법에 대해 알아봅니다.

   >[!VIDEO](https://video.tv.adobe.com/v/3453572?quality=12&learn=on&captions=kor){transcript=true}

   이메일 디자이너를 사용하여 직관적인 끌어다 놓기 인터페이스를 통해 매력적인 개별 맞춤형 이메일을 만들 수 있습니다. 자세한 내용은 [전자 메일 Designer 설명서](../../v8/email/get-started-email-designer.md)를 참조하세요

   이 비디오에서는 HTML을 업로드하여 이메일을 만드는 방법, 이메일 Designer과 호환되도록 하는 방법 및 템플릿으로 변환하는 방법을 알아봅니다.

   >[!VIDEO](https://video.tv.adobe.com/v/3447039?quality=12&learn=on&captions=kor){transcript=true}

   콘텐츠 조각은 하나 이상의 메시지에서 참조할 수 있는 재사용 가능한 구성 요소입니다. 전자 메일 게재 만들기를 단순화하기 위해 [콘텐츠 조각](../../v8/content/fragments.md)에 대해 자세히 알아보세요.

   디자인 프로세스를 가속화하고 개선하기 위해 독립형 템플릿을 만들어 Adobe Campaign 전체에서 사용자 정의 콘텐츠를 쉽게 재사용할 수 있습니다. [전자 메일 템플릿 만들기](../../v8/content/create-email-templates.md)를 참조하세요.

1. **미리 보기 및 테스트**

   이 비디오에서는 인기 있는 데스크톱, 모바일 및 웹 기반 클라이언트에서 이메일 메시지 콘텐츠 및 개인화를 미리 보고, 테스트 게재(증명)를 보내고, 이메일 렌더링을 확인하는 방법을 알아봅니다.

   >[!VIDEO](https://video.tv.adobe.com/v/3450344?quality=12&learn=on&captions=kor){transcript=true}

1. **전자 메일 및 확인 로그 보내기**

   콘텐츠, 대상자 및 일정을 정의했으면 이메일 게재를 준비할 준비가 되었습니다. 다음 섹션에서 자세히 알아보세요.

   * [이메일 준비 및 전송](../../v8/monitor/prepare-send.md)
   * [게재 로그 모니터링](../../v8/monitor/delivery-logs.md)


### SMS 게재 {#acs-gs-marketers-sms}

SMS 게재를 사용하여 실용적이고 효율적으로 문자 메시지를 고객의 모바일 디바이스로 전송할 수 있습니다. 이 기능을 통해 메시지를 효과적으로 전달하기 위해 텍스트 기반 메시지를 생성하고, 개인화하고, 미리 볼 수 있습니다.

Campaign v8에서 SMS 게재를 만들고, 테스트하고, 전송하는 자세한 단계는 Campaign Standard과 유사합니다.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="리드" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/create-sms"><strong>SMS 게재 만들기</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="저빈도" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/content-sms"><strong>SMS 게재 디자인<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="유효성 검사" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/sms/send-sms"><strong>SMS 게재 미리 보기 및 보내기</strong></a>
</div>
<p>
</td>
</tr></table>

### 푸시 알림 {#acs-gs-marketers-push}

푸시 알림은 앱을 사용하지 않는 경우에도 모바일 앱 사용자에게 연락할 수 있는 필수적 기능입니다. 업데이트 제공, 특정 작업 추진 및 거래에 대한 알림과 같은 다양한 목적을 제공합니다.

Campaign v8에서 푸시 알림 게재를 만들고, 테스트하고, 전송하는 자세한 단계는 Campaign Standard과 유사합니다.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/create-push">
<img alt="리드" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/create-push"><strong>푸시 게재 만들기</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/content-push">
<img alt="저빈도" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/content-push"><strong>푸시 게재 디자인<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/send-push">
<img alt="유효성 검사" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/msg/push/send-push"><strong>푸시 게재 미리 보기 및 보내기</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8은 Android 및 iOS 푸시 채널을 모두 지원합니다. 푸시 채널을 사용하여 기존 워크플로우 및 게재를 전환하려면 Adobe Campaign 전환 관리자에게 문의하십시오. [채널 설정](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}에 대해 자세히 알아보세요.
>
>* 모바일 애플리케이션용 SDK V4는 몇 년 전에 Campaign Standard에서 [더 이상 사용되지 않습니다](https://experienceleague.adobe.com/ko/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}. 이미 Campaign v8에서 사용되는 것과 동일한 Adobe Experience Platform SDK으로 전환했어야 합니다.
> 

### DM {#acs-gs-marketers-direct-mail}

DM(다이렉트 메일)은 엽서, 전단지, 카탈로그와 같은 개인 맞춤화된 레터를 대량으로 고객에게 게재하기 위한 파일을 제작할 수 있는 오프라인 채널입니다. DM 게재를 만들 때 Adobe Campaign은 모든 대상 프로필과 선택한 데이터(우편 주소 및 프로필 속성 등)를 포함하는 추출 파일을 자동으로 생성합니다.

Campaign v8에서 DM 게재를 만들고, 테스트하고, 보내는 자세한 단계는 Campaign Standard과 유사합니다.


1. [DM 게재 만들기](../../v8/direct-mail/create-direct-mail.md)
1. [추출 파일 정의](../../v8/direct-mail/content-direct-mail.md)
1. [미리 보기 및 보내기](../../v8/direct-mail/send-direct-mail.md)

### 인앱 채널 {#acs-gs-marketers-in-app}

Campaign v8에서는 인앱 채널을 사용할 수 없습니다. 인앱 알림을 보내야 하는 경우 Adobe 담당자에게 문의하십시오.

## 랜딩 페이지 만들기 및 관리 {#acs-gs-marketers-lp}

Adobe Campaign v8 웹 사용자 인터페이스에는 랜딩 페이지를 위한 이미지 재작성 사용자 환경이 제공됩니다. Campaign에서는 랜딩 페이지를 만들고, 디자인하고, 공유할 수 있습니다. 랜딩 페이지를 통해 사용자가 자신의 데이터를 업데이트하거나 커뮤니케이션 수신에 옵트인/옵트아웃하거나 뉴스레터와 같은 특정 서비스에 가입할 수 있는 온라인 양식으로 사용자를 보낼 수 있습니다.

Campaign v8로 전환하는 Campaign Standard 사용자는 기존 랜딩 페이지를 Campaign 웹 사용자 인터페이스로 마이그레이션했습니다. 동일한 기능 범위에 액세스할 수 있습니다.

다음 섹션에서 랜딩 페이지에 대해 자세히 알아보세요.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="리드" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/create-lp"><strong>랜딩 페이지 만들기</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="유효성 검사" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/lp-content"><strong>랜딩 페이지 디자인</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="유효성 검사" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/landing-pages/lp-templates"><strong>랜딩 페이지 템플릿 작업</strong></a>
</div>
<p>
</td>
</tr></table>


## 보고 {#acs-gs-marketers-reporting}

Adobe Campaign은 [보고 도구](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"} 집합을 제공합니다. 관리자는 다른 Campaign 사용자와 공유할 보고서를 만들고 구성할 수 있습니다.

Adobe Campaign 보고 도구 세트는 마케팅 노력의 효과에 대한 중요한 통찰력을 제공하여 캠페인이 최대의 효과를 발휘하도록 최적화할 수 있습니다. 자세한 내용은 [보고 설명서](../../v8/reporting/gs-reports.md)를 참조하세요.

또한 Adobe Campaign Standard 경험에 따라 이메일 게재에 대해 Campaign v8에서 동적 보고를 사용할 수 있습니다. 마케팅 활동의 영향을 측정하기 위해 완전히 맞춤화가 가능한 실시간 보고서를 제공합니다. 이 기능은 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 기능적 이메일 캠페인 데이터 외에도 성별, 도시, 연령과 같은 프로필 차원별로 인구통계 분석을 지원합니다. 자세한 내용은 [동적 보고 설명서](https://experienceleague.adobe.com/ko/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}를 참조하세요.

>[!AVAILABILITY]
>
>* [동적 보고](https://experienceleague.adobe.com/ko/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}는 전자 메일 게재, 전자 메일 게재 및 트랜잭션 메시지를 포함하는 캠페인의 보고에 사용할 수 있습니다. 프로필 차원별 인구 통계 분석도 사용할 수 있습니다.
>
> * [Adobe Campaign 웹 사용자 인터페이스 보고](../../v8/reporting/campaign-reports.md)는 모든 사용자가 Adobe Campaign Standard에서 Adobe Campaign v8로 전환하는 경우에도 사용할 수 있습니다.

Adobe Campaign은 세 가지 보고서를 제공합니다.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="유효성 검사" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>캠페인 보고서</strong></a>
</div>
<p>
<div>
<p>개별 게재의 성능, 효율성 및 결과에 대한 자세한 정보를 제공하여 포괄적인 개요를 제공합니다.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="리드" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>게재 보고서</strong>
</div>
<p>
<div>
<p>채널당 각 게재의 성능에 대한 성공률, 대상자 참여 및 기타 필수 지표를 철저히 분석합니다. 이를 통해 캠페인에 미치는 전반적인 효과와 영향을 평가할 수 있습니다.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="전반적 보고서" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong>글로벌 보고서</strong></a>
</div>
<p>
<div>
<p>Campaign 인스턴스 내의 각 채널에 대한 트래픽 및 참여 지표에 대한 통합된 전체 요약을 제공합니다. 이러한 보고서는 다양한 위젯으로 구성되어 있으며, 각 위젯은 캠페인 또는 게재 성과에 대한 고유한 관점을 제공합니다.</p>
</div>
<p>
</td>
</tr>
</table>
