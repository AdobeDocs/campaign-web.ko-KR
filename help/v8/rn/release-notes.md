---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 36d2b7a67ef087d628151199a223ceee54f84180
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 31%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [2024](release-notes-24.md) 및 [2025](release-notes-25.md) 페이지에 나열되어 있습니다.

## 2026년 1월 릴리스 {#26-1-release}

_2026년 1월 27일_

### 새로운 기능 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>GA(다국어 게재 기능)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 모든 고객(GA)이 다국어 게재 기능을 사용할 수 있습니다. 이 기능을 사용하면 Adobe Campaign 웹 사용자 인터페이스에서 여러 언어로 여러 메시지를 보낼 수 있습니다. 게재의 기본 언어와 게재를 보낼 수 있는 여러 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다. 
<p>자세한 내용은 <a href="../msg/multilingual.md">세부 설명서</a>를 참조하세요.</p>
<p>다국어 푸시 알림에 대해 다음과 같은 사항이 개선되었습니다.</p>
<ul>
<li>이제 다국어 콘텐츠가 포함된 CSV 파일을 업로드하여 모든 언어 변형을 빠르게 채울 수 있습니다. <a href="../msg/multilingual.md#csv-upload">자세히 보기</a>
</li>
<li>이제 리치 푸시 알림이 지원됩니다.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>트랜잭션 메시지(GA)의 프로필 보강</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 모든 고객(GA)이 트랜잭션 메시지의 프로필 강화 기능을 사용할 수 있습니다. 이제 이메일 외에도 SMS 및 푸시 알림도 지원됩니다. 이 기능을 사용하면 Adobe Campaign 데이터베이스 필드를 메시지 콘텐츠에 연결하여 트랜잭션 메시지를 개인화할 수 있습니다. 대상 매핑, 데이터 보강 열 및 조정 키를 선택하여 성능 임계값을 유지하면서 정확한 실시간 개인화를 보장할 수 있습니다.</p>
<p>자세한 내용은 <a href="../transactional-messaging/profile-enrichment.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager 라이브 및 언어 사본</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Manager 컨텐츠 통합을 사용하면 게재를 작성할 때 Adobe Experience Manager 내에서 직접 만든 모든 언어 및 라이브 카피에 액세스할 수 있습니다. 실시간으로 콘텐츠를 새로 고쳐 최신 Adobe Experience Manager 버전을 가져올 수 있습니다. 이 통합을 통해 Adobe Experience Manager과 Campaign 간의 수동 콘텐츠 동기화를 제거함으로써 다국어 캠페인 워크플로우를 간소화합니다.</p>
<p>자세한 내용은 <a href="../integrations/aem-multilingual.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>콘텐츠 실험 - A/B 테스트</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign 웹의 콘텐츠 실험을 사용하면 타겟 대상자에게 가장 적합한 성과를 측정하기 위해 여러 A/B 테스트 게재 변형을 정의할 수 있습니다. 게재 콘텐츠, 제목 또는 발신자를 다양하게 하여 다양한 버전을 테스트하고 가장 좋은 결과를 도출하는 변형을 결정할 수 있습니다. 제목란, 발신자 이름 및 이메일 본문 콘텐츠와 같은 다양한 이메일 요소에 대해 A/B 테스트를 수행할 수 있습니다.</p>
<p>자세한 내용은 <a href="../email/ab-testing.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>지속적인 게재 활동</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>연속 게재 활동을 사용하면 기존 게재에 새 수신자를 추가할 수 있습니다. 이 게재 유형은 매번 새 게재를 만들 필요가 없으므로 필요에 따라 전송되는 낮은 볼륨 경고 또는 알림에 대해 보다 효율적입니다. 연속 게재는 단일 게재 인스턴스를 만듭니다. 모든 게재 로그(broadLog) 및 추적 로그는 이 하나의 게재를 참조하므로 모니터링 및 보고를 단순화합니다.</p>
<p>자세한 내용은 <a href="../workflows/activities/continuous-delivery.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>캠페인 승인 관리</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>승인 프로세스를 통해 여러 관련자를 조정하고 게재를 보내기 전에 품질 관리를 할 수 있습니다. 조직에서 콘텐츠 검토 마케팅 관리자나 타겟 대상의 유효성을 검사하는 데이터 분석가와 같이 서로 다른 팀의 유효성 검사가 필요한 경우 승인을 사용하십시오.</p>
<p>자세한 내용은 <a href="../campaigns/campaign-approvals.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#26-1-improvements}

* 이제 동적 보고에서 푸시 알림 및 SMS를 지원합니다. [자세히 알아보기](../reporting/dynamic-reporting/get-started-reporting.md)
* 사전 정의된 필터 - 새로운 &quot;공유 필터&quot; 옵션을 사용하면 조직의 다른 사용자가 사전 정의된 필터를 사용할 수 있도록 할 수 있습니다. [자세히 알아보기](../get-started/predefined-filters.md#share-filter)
* 이름, 이메일, 날짜 및 주소와 같이 Adobe Experience Manager에서 생성된 개인화 필드는 이제 콘텐츠 템플릿을 사용할 때 포함되고 사용할 수 있습니다.
* 이제 콘텐츠 품질 평가는 브랜드 지침과 관계없이 명확성, 응집성 및 효율성 문제를 점검하여 명확하지 않은 메시지, 일관되지 않은 말투 또는 구조적 차이를 식별합니다. [자세히 알아보기](../content/brands-score.md)
