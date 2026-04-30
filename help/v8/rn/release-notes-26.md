---
title: Campaign v8 Web 사용자 인터페이스 이전 릴리스 정보
description: 2026년 Campaign Web 사용자 인터페이스 릴리스
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: ht
source-wordcount: '753'
ht-degree: 100%

---

# 2026년 릴리스 정보 {#2026-release}

이 페이지에는 **2026년 릴리스**&#x200B;에서 제공되는 모든 변경 사항과 개선 사항이 나열되어 있습니다. 최신 릴리스 정보는 [이 페이지](release-notes.md)에서 확인할 수 있습니다.

## 2026년 2월 릴리스 {#26-2-release}

_2026년 2월 17일_

### 새로운 기능 {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>캠페인 인벤토리의 타임라인 보기</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 캠페인 인벤토리에 시간 경과에 따른 캠페인을 시각화하고 관리할 수 있는 타임라인 보기가 포함됩니다. 목록 및 타임라인 간을 전환하고 주, 월 또는 일별로 탐색하며, 오늘 버튼을 사용하여 현재 날짜로 이동하며, 목록 보기와 동일한 필터 및 검색을 사용하여 오른쪽 패널에서 캠페인 세부 사항(상태, 워크플로, 게재)을 열 수 있습니다.</p>
<p>자세한 내용은 <a href="../campaigns/manage-campaigns.md#timeline">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>스키마 작성(LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign Web 사용자 인터페이스에서 직접 스키마를 만들고 관리할 수 있습니다. 이 기능을 사용하면 새 테이블을 만들고, 기존 스키마를 확장하고, 사용자 정의 양식을 만들 수 있습니다. 클라이언트 콘솔에 액세스하지 않고도 특정 비즈니스 요구 사항을 지원하기 위해 사용자 정의 데이터 구조를 정의할 수 있습니다.</p>
<p>참고: 이 기능은 조직 집합에만 사용할 수 있으며(제한된 가용성), 향후 릴리스를 통해 전역적으로 출시될 예정입니다.</p>
<p>자세한 내용은 <a href="../administration/schemas.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## 2026년 1월 릴리스 {#26-1-release}

_2026년 1월 27일_

### 새로운 기능 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>다국어 게재 기능(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 모든 고객이 다국어 게재 기능을 사용할 수 있습니다(GA). 이 기능을 사용하면 Adobe Campaign Web 사용자 인터페이스에서 여러 언어로 여러 메시지를 보낼 수 있습니다. 게재의 기본 언어는 물론, 게재를 전송할 수 있는 다양한 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다. 
<p>자세한 내용은 <a href="../msg/multilingual.md">세부 설명서</a>를 참조하십시오.</p>
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
<th><strong>트랜잭션 메시지의 프로필 보강(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 모든 고객이 트랜잭션 메시지의 프로필 강화 기능을 사용할 수 있습니다(GA). 이제 이메일 외에도 SMS 및 푸시 알림도 지원됩니다. 이 기능을 사용하면 Adobe Campaign 데이터베이스 필드를 메시지 콘텐츠에 연결하여 트랜잭션 메시지를 개인화할 수 있습니다. 대상 매핑, 데이터 보강 열 및 조정 키를 선택하여 성능 임계값을 유지하면서 정확한 실시간 개인화를 보장할 수 있습니다.</p>
<p>자세한 내용은 <a href="../transactional-messaging/profile-enrichment.md">세부 설명서</a>를 참조하십시오.</p>
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
<p>Adobe Experience Manager 컨텐츠 통합을 사용하면 게재를 작성할 때 Adobe Experience Manager 내에서 직접 만든 모든 언어 및 Live Copy에 액세스할 수 있습니다. 실시간으로 콘텐츠를 새로 고쳐 최신 Adobe Experience Manager 버전을 가져올 수 있습니다. 이 통합을 통해 Adobe Experience Manager와 Campaign 간의 수동 콘텐츠 동기화를 제거하여 다국어 캠페인 워크플로를 간소화합니다.</p>
<p>자세한 내용은 <a href="../integrations/aem-multilingual.md">세부 설명서</a>를 참조하십시오.</p>
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
<p>Adobe Campaign Web의 콘텐츠 실험을 통해 타깃 대상자에게 가장 적합한 성과를 측정하기 위해 여러 A/B 테스트 게재 변형을 정의할 수 있습니다. 게재 콘텐츠, 제목 또는 발신자를 다양화하여 여러 가지 버전을 테스트하고 최선의 결과를 도출하는 변형을 결정할 수 있습니다. 제목란, 발신자 이름 및 이메일 본문 콘텐츠와 같은 다양한 이메일 요소에 대해 A/B 테스트를 수행할 수 있습니다.</p>
<p>자세한 내용은 <a href="../email/ab-testing.md">세부 설명서</a>를 참조하십시오.</p>
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
<p>연속 게재 활동을 사용하면 기존 게재에 새 수신자를 추가할 수 있습니다. 이 게재 유형은 매번 새로운 게재를 만들 필요가 없으므로 필요에 따라 낮은 볼륨의 경고나 알림에 대해 더 효율적입니다. 연속 게재는 단일 게재 인스턴스를 만듭니다. 모든 게재 로그(broadLog) 및 추적 로그는 하나의 게재를 참조하므로 모니터링 및 보고를 단순화합니다.</p>
<p>자세한 내용은 <a href="../workflows/activities/continuous-delivery.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Campaign 승인 관리</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>승인 프로세스를 통해 여러 이해 당사자를 조정하고 게재를 보내기 전에 품질 관리를 할 수 있습니다. 조직에서 마케팅 관리자가 콘텐츠를 검토하거나 데이터 분석가가 타깃 대상자를 검증하는 것과 같이 서로 다른 팀의 유효성 검사가 필요한 경우 승인을 사용하십시오.</p>
<p>자세한 내용은 <a href="../campaigns/campaign-approvals.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#26-1-improvements}

* 이제 동적 보고에서 푸시 알림 및 SMS를 지원합니다. [자세히 알아보기](../reporting/dynamic-reporting/get-started-reporting.md)
* 미리 정의된 필터 - 새로운 &quot;공유 필터&quot; 옵션을 사용하면 조직의 다른 사용자가 미리 정의된 필터를 사용할 수 있도록 할 수 있습니다. [자세히 알아보기](../get-started/predefined-filters.md#share-filter)
* 이름, 이메일, 날짜 및 주소와 같이 Adobe Experience Manager에서 생성된 개인화 필드는 이제 콘텐츠 템플릿을 사용할 때 포함되고 사용할 수 있습니다.
* 콘텐츠 품질 평가는 이제 브랜드 가이드라인과 관계없이 가독성, 일치도, 효과성 문제를 점검하여 불명확한 메시지, 일관되지 않은 톤 또는 구조적 차이를 식별합니다. [자세히 알아보기](../content/brands-score.md)
