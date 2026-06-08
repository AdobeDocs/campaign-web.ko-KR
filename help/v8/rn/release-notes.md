---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 777611699d3d4189cdd7d0d7ded66a9b08cf26cd
workflow-type: ht
source-wordcount: 610
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 2026년 4월 릴리스 {#26-4-release}

_2026년 4월 29일_

### 개선 사항 {#26-4-improvement}

이제 **보강 데이터** 섹션을 **대상자 빌드** 워크플로 활동(쿼리 유형)에서 사용할 수 있습니다. Campaign Web 사용자 인터페이스에서 직접 **추가 데이터**&#x200B;를 조회하고, 추가하고, 편집하고, 제거할 수 있습니다. **보강** 활동에서와 같이, 단일 보강 속성, 컬렉션 링크 및 표현식을 추가할 수 있습니다.

[자세히 알아보기](../workflows/activities/build-audience.md)

## 2026년 3월 릴리스 {#26-3-release}

2026년 _3월_ 24일

### 새로운 기능 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>스키마 작성(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 모든 고객이 스키마 작성 기능을 사용할 수 있습니다(GA). 이 기능을 사용하면 Campaign Web 사용자 인터페이스에서 직접 스키마를 만들고 관리할 수 있습니다. 새 테이블을 만들고, 기존 스키마를 확장하고, 사용자 정의 양식을 만들 수 있습니다. 클라이언트 콘솔에 액세스하지 않고도 특정 비즈니스 요구 사항을 지원하기 위해 사용자 정의 데이터 구조를 정의할 수 있습니다.</p>
<p>자세한 내용은 <a href="../administration/schemas.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>이메일 디자이너의 테마(LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>테마는 브랜드 가이드라인에 맞는 재사용 가능한 테마 스타일을 정의하여 이메일에 대한 향상된 작성 환경을 제공합니다. 이제 조각에서 테마 변수를 사용하여 이메일 템플릿 간에 일관적인 스타일을 유지할 수 있습니다. 이 기능을 사용하면 제목, 설명, 이미지, 링크와 같은 콘텐츠 요소를 추상화한 미리 정의된 모듈을 사용하여 브랜드 일관성을 유지하면서 이메일을 더 빠르게 작성할 수 있습니다.</p>
<p>참고: 이 기능은 조직 집합에만 사용할 수 있으며(제한된 가용성), 향후 릴리스를 통해 전역적으로 출시될 예정입니다.</p>
<p>자세한 내용은 <a href="../email/apply-email-themes.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>사용자 정의 Firefly 모델과 서드파티 이미지 생성 모델의 통합</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>승인된 서드파티 이미지 모델과 함께 표준 및 사용자 정의 Firefly 모델의 원활한 통합을 활성화하여 이미지 생성 시 더 큰 유연성, 컨트롤 및 브랜드 정렬을 제공합니다.</p>
<p>요구 사항에 맞는 모델을 선택하십시오.</p>
<ul><li> 별도의 설정 없이 즉시 이미지 생성을 위한 <strong>Adobe 모델</strong>(Firefly Image Model 4 기반)</li><li> 특수 기능을 위한 <strong>파트너 모델</strong>(Gemini 2.5 Flash 기반)</li><li>브랜드 정체성, 스타일 및 시각적 가이드라인에 정확히 일치하는 브랜드 콘텐츠 생성을 위한 <strong>사용자 정의 모델</strong>(사용자 고유의 에셋에 대해 학습된 브랜드 전용 모델)</li></ul>
<p>자세한 내용은 <a href="../content/generative-models.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>자동화된 게재 활동</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 워크플로 팔레트에서 <strong>자동화된 게재</strong> 워크플로 활동을 사용할 수 있습니다. 이를 워크플로 내에서 바로 사용하여 게재 액션(준비, 교정쇄 보내기, 준비 및 시작 등)을 만들거나 실행할 수 있습니다. 워크플로 외부에서 만든 기존의 게재를 선택하여 실행할 때마다 재사용하거나, 활동이 실행될 때마다 템플릿에서 새로운 게재를 만들 수 있습니다.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>자세한 내용은 <a href="../workflows/activities/automated-delivery.md">세부 설명서를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>여러 워크플로 분기 및 조인 활동</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>이제 <strong>여러 분기</strong>가 지원됩니다. <strong>포크</strong>를 사용하는 대신 도구 모음에서 <strong>분기 추가</strong>를 클릭할 수 있습니다. <strong>AND-조인</strong> 활동도 개선되었습니다. 이제 AND와 OR 조인 옵션 중에서 선택할 수 있는 일반 <strong>조인</strong> 활동입니다.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>자세한 내용은 <a href="../workflows/orchestrate-activities.md#toolbar">활동 오케스트레이션</a> 및 <a href="../workflows/activities/join.md">조인</a> 설명서 페이지를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#26-3-improvements}

* 클라이언트 콘솔과의 호환성을 개선하기 위해 **시작** 워크플로 활동이 추가되었습니다. 이 활동은 선택 사항이며 기본적으로 새 워크플로에 삽입되지 않습니다. 단, 기존 워크플로에는 자동으로 추가됩니다.
  [자세히 알아보기](../workflows/activities/about-activities.md#flow-control)
* 게재의 **일정** 설정에서 시간대 선택 필드가 **연락 날짜** 필드 아래로 이동되었습니다. [자세히 알아보기](../msg/create-deliveries.md#gs-schedule)