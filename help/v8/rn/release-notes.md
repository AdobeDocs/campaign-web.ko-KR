---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 10월 릴리스 {#24-10-release}

**릴리스 날짜**: 2024년 10월 29일

10월 릴리스부터 다음 기능 및 개선 사항을 사용할 수 있습니다.

### 기능

<table>
<thead>
<tr>
<th><strong>외부 계정</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign 웹 사용자 인터페이스를 통해 직접 외부 계정을 설정하고 관리할 수 있습니다. 이 새로운 기능을 사용하면 바운스 이메일(POP3) 또는 실행 인스턴스와 같은 다양한 유형의 외부 계정을 간단하게 구성할 수 있습니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>트랜잭션 메시지</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign 웹 사용자 인터페이스에서 트랜잭션 메시지를 만들고 모니터링할 수 있습니다. 트랜잭션 메시지는 트리거된 메시지를 처리하도록 설계된 Adobe Campaign의 특수 모듈입니다. 이러한 메시지는 정보 시스템에서 발생하는 이벤트에 대한 응답으로 자동으로 생성됩니다. 이러한 이벤트의 일반적인 예로는 버튼 또는 링크 클릭, 장바구니 포기, 제품 가용성 경고 요청, 계정 생성 또는 수정 등이 있습니다.</p>
<p>자세한 내용은 <a href="../transactional-messaging/transactional.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### 개선 사항

* **워크플로우 활동** - 이제 워크플로우 내에서 전환에서 다른 전환으로 활동 및 모든 하위 노드를 이동할 수 있습니다. 해당 작업의 속성 창에서 전용 **이동** 단추를 사용하여 이 작업을 수행할 수 있습니다. [자세히 알아보기](../workflows/orchestrate-activities.md#move)

* **워크플로우 보강 활동**

   * 이제 **데이터 보강** 활동에서 새 필드를 만들 때 별칭 및 레이블을 정의할 수 있습니다. [자세히 알아보기](../workflows/activities/enrichment.md#collection-settings)
   * 이제 **데이터 보강** 활동의 각 프로필에 대한 오퍼를 추가할 수 있습니다. [자세히 알아보기](../workflows/activities/enrichment.md##add-offers)

* **값 배포** - 개인화를 위해 필드 목록에 액세스할 때 이제 각 필드에 대한 값이 어떻게 배포되어 있는지 확인할 수 있습니다. 전용 팝업 창에 각 값에 대한 숫자와 백분율이 표시됩니다. [자세히 알아보기](../query/build-query.md#distribution-values-query)


## 9월 업데이트 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI 어시스턴트 콘텐츠 가속기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>메시지를 만들고 맞춤화하면 Adobe Campaign 웹의 AI Assistant Content Accelerator를 사용하여 한 차원 높은 수준으로 메시지를 만들 수 있습니다. 이 강력한 도구를 사용하면 다양한 매력적인 텍스트, 메인 제목 및 시각적으로 매력적인 이미지를 생성하여 콘텐츠의 영향을 최적화할 수 있습니다.</p>
<p><a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">실시간 기능 미리보기</a>를 통해 직접 기능을 살펴보고 성능을 완벽하게 이해해 보십시오</a>.</p>
<p>자세한 내용은 <a href="../email/generative-gs.md">세부 설명서</a>를 참조하십시오.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>가용 일자: 9월 12일</p>
</td>
</tr>
</tbody>
</table>

## 8월 릴리스 {#24-8-release}

**릴리스 일자**: 2024년 9월 3일

8월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

* **SMTP 매개변수** - 이제 SMTP 설정을 이메일 게재 설정에서 사용할 수 있습니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#smtp)

* **전역 변수** - 이제 전역 변수를 정의하여 게재에 대한 값을 정의할 수 있습니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#variables-delivery)

### 제한 공개된 새로운 기능 {#acs-24-8}

>[!AVAILABILITY]
>
>다음 기능은 제한 공개(LA)로 제공됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8로** 마이그레이션하는 고객으로 제한되며 다른 환경에는 배포할 수 없습니다.
>
>[Campaign Standard에서 Campaign v8로의 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ko){target="_blank"} 설명서 페이지를 참조하십시오.

* **다이렉트 메일에 대한 브랜딩** - 기술 관리자는 이제 브랜드의 정체성에 영향을 미치는 매개변수를 중앙 집중화하기 위해 하나 이상의 브랜드를 정의할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이제 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. [자세히 알아보기](https://experienceleague.adobe.com/ko/docs/experience-cloud/campaign/branding/branding-assign)

* **랜딩 페이지를 통한 구독** - 이제 랜딩 페이지를 서비스에 연결하고, 사용자가 이를 검증하면 확인 메시지를 보낼 수 있습니다. [자세히 알아보기](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **시각적 조각** - 이제 시각적 콘텐츠 조각을 보관할 수 있습니다. [자세히 알아보기](../content/create-fragment.md#archive)

* **랜딩 페이지의 Captcha** - 이제 Captcha를 추가하여 봇으로 인한 스팸과 남용으로부터 랜딩 페이지를 보호할 수 있습니다. 이는 고객과의 상호 작용이 필요하지 않고 사이트와의 상호 작용을 기반으로 하기 때문에 고객을 방해하지 않습니다. [자세히 알아보기](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
