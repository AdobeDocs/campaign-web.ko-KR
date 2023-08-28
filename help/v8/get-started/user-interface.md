---
audience: end-user
title: 인터페이스 살펴보기
description: Campaign v8 Web 사용자 인터페이스
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha"
source-git-commit: bbe4ed0ce05048cf22a18a36967b9a4c0422d93f
workflow-type: tm+mt
source-wordcount: '2567'
ht-degree: 99%

---

# 인터페이스 살펴보기 {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="인터페이스 살펴보기"
>abstract="새로운 Campaign v8 Web 인터페이스는 통합되고 직관적이며, 일관된 사용자 경험을 제공합니다."

새로운 Campaign v8 Web 인터페이스는 현대적이고 직관적인 사용자 경험을 제공하여 마케팅 캠페인 디자인 및 게재를 간소화합니다. 이 새로운 인터페이스는 Adobe Experience Platform과 통합됩니다.


>[!NOTE]
>
>이 설명서는 제품 사용자 인터페이스의 최신 변경 내용을 반영하여 자주 업데이트됩니다. 단, 실제 사용자 인터페이스와 약간 다른 스크린샷도 있습니다.


## 왼쪽 탐색 메뉴 {#user-interface-left-nav}

왼쪽에 있는 링크를 찾아 Campaign v8 Web 기능에 액세스합니다. 여러 링크에 정렬 및 필터링할 수 있는 오브젝트 목록이 표시됩니다. 필요한 모든 정보를 표시하도록 열을 구성할 수도 있습니다. 이 [섹션](#list-screens)을 참조하십시오. 이메일 게재 목록을 제외한 모든 목록 화면은 읽기 전용입니다. Alpha에서는 편집/보기를 위해 목록 항목을 클릭할 수 없습니다. 향후 버전에서는 모든 목록을 편집할 수 있습니다. 왼쪽 탐색 메뉴에 표시되는 항목은 사용자 권한에 따라 다릅니다.

![](assets/home.png)

### 홈 {#user-interface-home}

이 화면에는 주요 Campaign v8 Web 기능에 빠르게 액세스할 수 있는 주요 링크와 리소스가 포함되어 있습니다.

**최근 항목** 목록은 최근 생성 및 수정된 게재에 대한 단축키를 제공합니다. 이 목록에는 채널, 상태, 소유자, 생성 및 수정일이 표시됩니다.

**주요 성과 지표**&#x200B;를 사용하면 공통 KPI를 통해 플랫폼 효율성을 확인할 수 있습니다.

홈 페이지 **학습** 섹션의 Campaign v8 Web 주요 도움말 페이지에 액세스합니다.


### 주요 성과 지표 {#user-interface-key-indicators}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="스팸"
>abstract="스팸 KPI"

플랫폼의 주요 성과 지표를 확인하려면 홈 페이지로 이동합니다. 이러한 지표에는 게재, 열람, 클릭, 구독 취소된 메시지의 수 및 비율과 오류율이 표시됩니다.

지표는 기본적으로 지난 7일 동안 전송된 게재에 대해 계산됩니다. 카드 오른쪽 상단에 있는 드롭다운 목록에서 기간을 변경할 수 있습니다. 테스트 프로필로 전송된 메시지는 제외됩니다.

표시할 채널을 선택할 수 있습니다. 기본적으로 이러한 표시기는 이메일 채널에 대한 지표를 반영합니다.

![](assets/kpi.png)

#### 게재된 메시지 {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="게재됨"
>abstract="이 지표에는 선택된 채널에 대해 성공적으로 처리된 모든 메시지 수의 합계와, 전송된 총 메시지 수에 대한 성공적으로 게재된 메시지 수의 비율이 표시됩니다."

게재된 메시지 수는 전달성 비율을 반영합니다. 이 비율은 일부 주소나 전화번호가 잘못되었거나, 이메일 제공업체의 스팸 차단기가 메시지를 거부하거나, 전달성 문제가 발생하는 등의 이유로 100%는 될 수 없습니다.

**게재됨** 표시기에는 각 채널에 대해 다음 KPI가 표시됩니다.

* 전송된 총 메시지 수에 대한 성공적으로 게재된 메시지 수의 비율

* 성공적으로 처리된 모든 메시지 수의 합계

Adobe Campaign에서 메시지를 “전달됨”으로 표시하는 규칙은 다음과 같습니다.

“시드 주소” 필드가 “아니요”이고 상태가 “서비스 공급자에 의해 고려됨”(SMS의 경우), “전송됨”(이메일의 경우) 또는 “모바일에서 수신됨”(푸시 알림의 경우)인 메시지 수


#### 총 열람 수 {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="열람 수"
>abstract="이 지표에는 선택된 채널에 대해 열람된 모든 메시지 수의 합계와, 성공적으로 게재된 총 메시지 수에 대한 열람된 메시지 수의 비율이 표시됩니다."

총 열람 수는 해당 열람을 생성한 개별 수신자 수에 관계없이 메시지가 열린 총 횟수를 추적하여 계산됩니다. 이 표시기는 이메일에만 사용할 수 있습니다.

**열람 수** 표시기에는 각 채널에 대해 다음 KPI가 표시됩니다.

* 성공적으로 게재된 총 메시지 수에 대한 열람된 메시지 수의 비율

* 채널당 열람된 모든 메시지 수의 합계

Adobe Campaign은 수신자가 이메일의 이미지를 다운로드할 때 메시지 열람을 감지합니다. HTML 및 다중 파트/대체 이메일에는 열람된 메시지를 감지할 수 있는 0픽셀 이미지가 포함되어 있습니다. 텍스트 포맷의 메시지에는 이미지가 포함되어 있지 않으므로 열람되었는지 여부를 감지할 수 없습니다. 메시지 열람 수를 기준으로 계산된 값은 이미지 표시와 관련된 오차 범위로 인해 언제까지나 추정치에 불과합니다.



#### 클릭스루 비율 {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="클릭 수"
>abstract="이 지표에는 선택된 채널에 대해 메시지에서 클릭된 모든 URL의 합계와, 성공적으로 게재된 총 메시지 수에 대한 클릭 수의 비율이 표시됩니다."

메시지 내용에 URL을 추가하면 수신자를 특정 페이지로 리디렉션할 수 있습니다. 클릭스루 비율은 메시지의 링크를 클릭한 수신자의 수와 비율을 측정합니다.

**클릭 수** 표시기에는 각 채널에 대해 다음 KPI가 표시됩니다.

* 성공적으로 게재된 총 메시지 수에 대한 클릭 수의 비율

* 게재 시 한 번 이상 클릭한 고유 사용자 수 (구독 취소 링크 및 이메일 미러 페이지 링크 제외)

이 지표는 통합 추적 테이블(`nms:trackingStats`)을 기반으로 합니다. 이 집계 테이블은 보고서를 표시할 때 수신자 추적 로그 테이블(`nms:trackingLogRcp`) 대신 성능상의 목적으로 사용되며 실시간으로 계산되지 않습니다. 추적 로그가 검색되고 몇 분 후에 테이블이 생성됩니다.


#### 구독 취소 비율 {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="구독 취소 건수"
>abstract="이 지표에는 선택한 채널에 대해 서비스의 모든 구독 취소 건수의 합계와, 성공적으로 게재된 총 메시지 수에 대한 구독 취소 수의 비율이 표시됩니다."

수신자는 이메일 콘텐츠의 전용 구독 취소 링크를 통해 또는 SMS에 STOP이라고 답장하여 이메일 및 SMS를 옵트아웃할 수 있어야 합니다.

**구독 취소 건수** 표시기에는 각 채널에 대해 다음 KPI가 표시됩니다.

* 성공적으로 게재된 총 메시지 수에 대한 구독 취소 건수의 비율

* 구독 취소 링크(“옵트아웃”과 같은 URL 범주)의 모든 클릭 수 합계


#### 오류율 {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="오류 수"
>abstract="게재 및 자동 바운스 처리 중 누적된 총 오류 수입니다. 결합된 비율은 게재될 메시지 수에 대한 비율입니다."

Adobe Campaign 플랫폼에서 전송한 일부 메시지는 대상에 도달하지 못할 수 있습니다. 이는 사용자 주소나 전화번호에 오타가 있거나, 수신자가 이메일 주소를 변경했거나, 수신자의 사서함이 가득 찬 경우에 발생할 수 있습니다. 메시지를 프로필로 보낼 수 없는 경우 원격 서버는 자동으로 Adobe Campaign에 오류 메시지를 보냅니다. 이 오류는 이메일 주소, 전화번호 또는 디바이스를 격리해야 하는지 여부를 결정하는 데 적합합니다.

따라서 항상 데이터베이스를 확인하고 업데이트해야 하며 모든 프로필이 활성 상태이고 실제인지 확인해야 합니다. 게재 오류는 메시지가 게재되지 않은 이유에 따라 일시적이거나 영구적일 수 있습니다(소프트 바운스이거나 하드 바운스일 수 있습니다).

**오류 수** 표시기에는 각 채널에 대해 다음 KPI가 표시됩니다.

* 게재될 총 메시지 수에 대한 오류 수의 비율

* 게재 및 자동 리바운드 처리 중 누적된 총 오류 수


### 탐색기 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="탐색기"
>abstract="**탐색기** 메뉴에는 클라이언트 콘솔의 폴더 계층과 동일한 폴더 계층과 함께 모든 Campaign 구성 요소 및 오브젝트가 표시됩니다. 모든 Campaign v8 구성 요소, 폴더 및 스키마를 찾아보고 게재, 워크플로 및 캠페인을 만듭니다. 다른 모든 목록은 읽기 전용입니다."

**탐색기** 메뉴에는 클라이언트 콘솔의 폴더 계층과 동일한 폴더 계층과 함께 모든 Campaign 리소스 및 오브젝트가 표시됩니다. 모든 Campaign v8 구성 요소, 폴더 및 스키마를 찾아보고 게재, 워크플로 및 캠페인을 만듭니다. 다른 모든 목록은 읽기 전용입니다.

탐색기에 표시되는 항목은 사용자 권한에 따라 다릅니다.

모든 목록 화면과 마찬가지로 디스플레이를 개인화하고 필요한 모든 정보를 표시하도록 열을 구성할 수 있습니다. 이 [섹션](#list-screens)을 참조하십시오.

Campaign 탐색기, 폴더 계층 및 리소스에 대한 자세한 내용은 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}를 참조하십시오.

### 캠페인 관리 {#user-interface-campaign-management}

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="캠페인"
>abstract="다음은 캠페인 목록입니다. 시작/종료/마지막 수정 일자 및 상태와 같은 유용한 정보를 볼 수 있습니다. 상태 또는 시작/종료 일자별로 목록을 필터링할 수 있습니다. “캠페인 만들기” 버튼을 클릭하여 새 캠페인을 추가합니다. 콘텐츠, 게재 및 세부 정보를 보려면 캠페인을 선택합니다. 템플릿을 보고 만들려면 “템플릿” 탭으로 이동합니다."



캠페인 관리 섹션에서 마케팅 캠페인, 게재 및 워크플로에 액세스할 수 있습니다.

* **캠페인** - 다음은 캠페인 목록 및 캠페인 템플릿입니다. 기본적으로 각 캠페인의 경우 시작/종료/생성/마지막 수정 일자, 현재 상태와 캠페인을 만든 캠페인 운영자 이름을 볼 수 있습니다. 상태, 시작/종료 일자, 폴더별로 목록을 필터링하거나, 고급 필터를 만들어 자신만의 필터링 기준을 정의할 수 있습니다. [이 섹션에서](../campaigns/gs-campaigns.md) 캠페인에 대해 자세히 알아보십시오.

* **게재** - 게재 목록을 탐색합니다. 기본적으로 상태, 마지막 수정 일자 및 주요 KPI를 볼 수 있습니다. 상태, 연락일 또는 채널별로 목록을 필터링할 수 있습니다. 이메일 게재를 클릭하여 대시보드를 열고 게재 세부 정보의 개요를 확인합니다. 다른 채널의 게재는 읽기 전용입니다. [이 섹션에서](../msg/gs-messages.md) 게재에 대해 자세히 알아보십시오.

  **추가 작업**&#x200B;을 사용하여 게재를 삭제하거나 복제할 수 있습니다.

  ![](assets/more-actions.png){width="70%" align="left"}

* **워크플로** - 이 화면에서 워크플로 전체 목록 및 워크플로 템플릿에 액세스할 수 있습니다. 상태, 마지막/다음 실행 일자를 확인하고 새 워크플로 또는 새 워크플로 템플릿을 만들 수 있습니다. 다른 오브젝트와 동일한 기준으로 목록을 필터링할 수 있습니다. 또한 캠페인에 속한 워크플로 또는 속하지 않은 워크플로를 필터링할 수 있습니다. [이 섹션에서](../workflows/gs-workflows.md) 워크플로에 대해 자세히 알아보십시오.


### 고객 관리 {#user-interface-customer-management}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="수신자"
>abstract="수신자 데이터베이스에 액세스합니다. 이메일 주소, 이름, 성과 같은 유용한 정보를 볼 수 있습니다. 이 목록은 읽기 전용입니다."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="대상자"
>abstract="다음은 대상자 목록입니다. 유형, 원본, 생성/마지막 수정 일자 및 레이블을 볼 수 있습니다. 원본을 기준으로 목록을 필터링할 수 있습니다. 이 목록은 읽기 전용입니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="구독 목록"
>abstract="구독 목록을 탐색합니다. 유형, 모드 및 레이블을 볼 수 있습니다. 이 목록은 읽기 전용입니다."


고객 관리 섹션에서 수신자, 대상자 및 구독을 볼 수 있습니다. 이 목록은 읽기 전용입니다.

* **수신자** - 수신자 데이터베이스에 액세스합니다. 기본적으로 이메일 주소, 이름 및 성을 볼 수 있습니다. [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/gs-audiences.html){target="_blank"}에서 수신자에 대해 자세히 알아보십시오.
* **대상자** - 대상자 목록입니다. 기본적으로 유형, 원본, 생성/마지막 수정 일자 및 레이블을 볼 수 있습니다. 원본을 기준으로 목록을 필터링할 수 있습니다. [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}에서 대상자에 대해 자세히 알아보십시오.
* **구독** - 구독 목록을 탐색합니다. 기본적으로 해당 유형, 모드 및 레이블을 볼 수 있습니다. [Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}에서 구독 및 구독 취소를 관리하는 방법에 대해 알아봅니다.

### 의사 결정 관리

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="오퍼"
>abstract="상호 작용 오퍼 목록을 찾아보십시오. 기본적으로 상태, 시작/종료 일자 및 환경을 볼 수 있습니다. 상태 및 시작/종료 날짜별로 목록을 필터링할 수 있습니다. 오퍼 템플릿도 사용할 수 있습니다. 이 목록은 읽기 전용입니다."

* **오퍼** - 상호 작용 오퍼 목록을 탐색합니다. 기본적으로 상태, 시작/종료 일자 및 환경을 볼 수 있습니다. 상태 및 시작/종료 날짜별로 목록을 필터링할 수 있습니다. 오퍼 템플릿도 사용할 수 있습니다. 이 목록은 읽기 전용입니다.

[Adobe Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}에서 오퍼를 만들고 관리하는 방법에 대해 알아봅니다.

## 상단 막대

인터페이스의 상단 막대를 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* Alpha 테스터로서 피드백 공유
* 조직과 인스턴스 간 전환
* Adobe Experience Cloud 애플리케이션 간 전환
* 도움말 페이지 액세스, 지원 팀에 문의 및 피드백 공유 검색 필드에서 도움말 문서와 비디오를 검색할 수 있습니다.

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 상황별 도움말 {#contextual-help}

인터페이스에서 상황별 도움말을 사용할 수 있습니다. 사용 가능한 경우 `?` 아이콘을 클릭하면 도움말 정보 및 관련 설명서 링크가 표시됩니다.

![](assets/context-help.png){width="40%" align="left"}

<!--An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}-->

## 지원되는 브라우저 {#browsers}

Campaign v8 Web은 최신 버전의 Google Chrome, Safari 및 Microsoft Edge에서 최적으로 작동하도록 디자인되었습니다. 이전 버전이나 다른 브라우저에서 특정 기능 사용 시 문제가 발생할 수 있습니다.

## 언어 환경 설정 {#language-pref}

Campaign v8 Web은 현재 다음 언어로 제공됩니다.

<table>
<tr>
<td>
<p>영어(미국) - EN-US</p>
<p>프랑스어 - FR</p>
<p>독일어 - DE</p>
<p>이탈리아어 - IT</p>
</td>
<td>
<p>스페인어 - ES</p>
<p>포르투갈어(브라질) - PTBR</p>
<p>일본어 - JP</p>
</td>
<td>
<p>한국어 - KR</p>
<p>중국어 간체 - CHS</p>
<p>중국어 번체 - CHT</p>
</td>
</tr>
</table>

기본 인터페이스 언어는 사용자 프로필에 지정된 기본 언어에 따라 결정됩니다.

언어를 변경하려면 다음 작업을 수행하십시오.

1. 오른쪽 상단의 프로필 아이콘을 클릭한 다음 **환경 설정**&#x200B;을 선택합니다.
1. 그런 다음 이메일 주소 아래에 표시되는 언어 링크를 클릭합니다.
1. 원하는 언어를 선택하고 **저장**&#x200B;을 클릭합니다. 사용 중인 구성 요소가 첫 번째 언어로 현지화되어 있지 않은 경우 두 번째 언어를 선택할 수 있습니다.


## 자세히 알아보기 {#learn-more}

[이 페이지](list-filters.md)에서 Campaign 환경에서 사용 가능한 목록을 탐색, 검색 및 필터링하는 방법에 대해 알아보십시오.


<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="보강 데이터"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="보고 전송"
>abstract="캠페인 보고에 전송 표시기를 참조하십시오."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="보고 추적"
>abstract="캠페인 보고에 추적 표시기를 참조하십시오."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="보고 개요"
>abstract="게재에 대한 주요 지표."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="대상 통계 보고"
>abstract="이 섹션에는 대상자에 따라 특정 지표가 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="집계된 게재 보고"
>abstract="집계된 데이터 보고서를 표시하려면 두 개 이상의 게재를 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="중복 제거 필드"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="중복 제거 설정"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="중복 제거 보조 항목"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="차원 보조 항목"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="권한 필요"
>abstract="세그먼트를 만들려면 먼저 관리자가 권한을 부여해야 합니다."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="권한 필요"
>abstract="세그먼트를 만들려면 먼저 관리자가 권한을 부여해야 합니다."


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="이 캠페인은 읽기 전용입니다."
>abstract="이 캠페인을 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="이 게재는 읽기 전용입니다."
>abstract="이 게재를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="이 서비스는 읽기 전용입니다."
>abstract="이 서비스를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

<!-- Workflows-->

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="워크플로 목록"
>abstract="캠페인에 사용할 수 있는 워크플로 목록. “워크플로 만들기” 버튼을 사용하여 캠페인에서 워크플로를 추가합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="대상자 저장을 위한 아웃바운드 전환"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="대상자 저장"
>abstract="이 활동을 사용하여 워크플로 대상자를 저장합니다."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="이 워크플로는 읽기 전용입니다."
>abstract="이 워크플로를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="이 워크플로는 읽기 전용입니다."
>abstract="지원되지 않거나 호환되지 않는 캔버스로 인해 이 워크플로를 편집할 수 없습니다."

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="유효 기간"
>abstract="이 옵션은 추적이 URL에서 활성화되는 기간을 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="게재 기간"
>abstract="게재 기간 필드를 통해 글로벌 게재 재시도에 대한 제한 값을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 전송하고 나서 메시지가 오류만 반환하는 경우 유효성 검사 제한에 도달할 때까지 구성 가능한 일반 재시도를 수행합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="리소스 유효성 검사 제한"
>abstract="유효성 검사 제한 필드는 미러 페이지나 이미지와 같이 업로드된 리소스에 사용됩니다. 이러한 리소스는 제한된 시간 동안만 유효합니다. 한도에 도달하면 리소스를 더 이상 사용할 수 없습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="승인 모드"
>abstract="각 게재 단계는 승인을 받아 다양한 프로세스를 전체 모니터링하고 제어할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="최대 재시도 수"
>abstract="일시적인 오류로 인해 메시지 전송이 실패하면 게재 기간이 종료될 때까지 재시도를 수행합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="수신자 중요도"
>abstract="수신자 중요도는 용량 유형화 규칙 초과 시 유지되는 수신자를 결정하는 데 사용되는 공식입니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="게재 가중치"
>abstract="게재 가중치를 통해 압력 관리 프레임워크 내에서 최우선 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선 순위가 높습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="유형화"
>abstract="유형화로 게재 전송을 제어, 필터링 및 모니터링할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_reporting_email_exportation"
>title="내보내기"
>abstract="선택한 페이지만 내보낼 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="캠페인의 게재 목록"
>abstract="캠페인의 게재 목록"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="캠페인의 워크플로 목록"
>abstract="캠페인의 워크플로 목록"

<!-- delivery settings-->

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="게재 설정 대상"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="게재 설정 승인"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="게재 설정 테스트 설정"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="게재 설정 웹 분석"
>abstract="TBC"
