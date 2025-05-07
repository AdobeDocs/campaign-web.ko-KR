---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: ht
source-wordcount: '689'
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [2024](release-notes-24.md) 및 [2025](release-notes-25.md)에 나열되어 있습니다.

## 2025년 4월 릴리스 {#25-4-release}

**릴리스 일자**: 2025년 4월 29일


### 새로운 기능 {#25-4-features}

다음 기능은 4월 릴리스 이후 모든 사용자가 사용할 수 있습니다.

<table>
<thead>
<tr>
<th><strong>콜센터 채널</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign Web 사용자 인터페이스에서 콜센터 채널을 사용할 수 있습니다. 이 채널은 콜센터를 통해 처리되는 커뮤니케이션 또는 상호 작용을 관리하고 추적하는 데 사용되는 커뮤니케이션 방식을 의미합니다. 일반적으로 상담원이 고객이나 잠재 고객에게 전화를 거는 경우에 사용됩니다.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>자세한 내용은 <a href="../call-center/gs-call-center.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>새로운 규칙 빌더</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 개선된 사용자 인터페이스에서 복잡한 조건을 정의하는 데 도움이 되는 새로운 규칙 작성기를 사용할 수 있습니다. 필요에 따라 이전 규칙 빌더에서 새로운 규칙 빌더로 전환할 수 있습니다.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>자세한 내용은 <a href="../query/query-modeler-overview.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>외부 계정 작성</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>캠페인 관리자는 이제 Campaign Web 사용자 인터페이스에서 외부 시스템과의 새로운 연결을 설정할 수 있습니다.
기존 외부 계정을 보고, 업데이트하고, 관리할 수도 있습니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#25-4-improvements}

**일반 인터페이스 개선**

* 이제 사용자 인터페이스에서 스키마 속성에 대한 필드 설명, 즐겨찾기에 추가 및 값 분포 옵션을 더 쉽게 확인할 수 있습니다. 자세한 내용은 [세부 설명서](../get-started/attributes.md)를 참조하십시오.
* 이제 인터페이스에서 날짜와 시간이 Experience League 환경 설정에서 설정된 기본 언어에 따라 표시됩니다. 이 개선 사항은 몇몇 언어에만 적용됩니다. 지원되는 언어의 전체 목록을 보려면 [세부 설명서](https://experienceleague.adobe.com/ko/docs/core-services/interface/features/browser-language){target=_blank}를 참조하십시오.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**이메일 편집기**: 이제 Campaign Web UI의 접근성을 높이기 위해 이메일 디자이너에서 두 개의 새로운 필드를 사용할 수 있습니다. 이 필드는 이메일 콘텐츠의 `title` 요소와 `html` 요소의 언어 속성에 해당합니다. 이러한 설정은 이메일 본문 섹션에서 프리헤더 필드 외에도 정의할 수 있습니다. 자세한 내용은 [세부 설명서](../email/metadata.md)를 참조하십시오.

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**스키마**

* 이제 Campaign Web 사용자 인터페이스에서 목록의 임시 스키마를 편집할 수 있습니다. 자세한 내용은 [세부 설명서](../audience/manage-audience.md)를 참조하십시오.
* 이제 샘플 화면에서 스키마의 사용자 정의 필드를 미리 볼 수 있습니다. 자세한 내용은 [세부 설명서](../administration/custom-fields.md#add)를 참조하십시오.
* 이제 끌어다 놓기로 목록에서 사용자 정의 필드를 이동할 수 있습니다. 자세한 내용은 [세부 설명서](../administration/custom-fields.md#add)를 참조하십시오.


### 제한 공개된 새로운 기능 {#25-4-features-la}

>[!AVAILABILITY]
>
>다음 기능은 제한 공개(LA)로 제공됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8로** 마이그레이션하는 고객으로 제한되며 다른 환경에는 배포할 수 없습니다. 해당 고객은 Campaign 서버를 v8.7.4로 업그레이드해야 합니다.
>
>[Campaign Standard에서 Campaign v8로의 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) 설명서 페이지를 참조하십시오.

* **다국어 게재 생성** - 이제 Adobe Campaign Web 사용자 인터페이스에서 다양한 언어로 여러 이메일 게재를 전송할 수 있습니다. 다국어 게재 기능을 사용하면 게재의 기본 언어는 물론, 게재를 전송할 수 있는 다양한 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다. 자세한 내용은 [세부 설명서](../email/edit-content.md)를 참조하십시오.

* **다국어를 위한 동적 보고** - 이제 다국어 이메일 게재에 대해 동적 보고가 가능합니다. 자세한 내용은 [세부 설명서](../reporting/global-reports.md)를 참조하십시오.

* **SMS REST API 지원(LA)** - 이제 SMS 채널에서 트랜잭션 메시지 REST API를 사용할 수 있습니다. 페이로드에 이메일과 휴대폰이 모두 있는 경우 “wishedChannel” 필드를 사용하여 채널을 지정할 수 있습니다. 제공되지 않으면 wishedChannel에서 SMS를 명시적으로 요청하지 않는 한 기본적으로 이메일이 사용됩니다. 자세한 내용은 [세부 설명서](https://experienceleague.adobe.com/ko/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}를 참조하십시오.

