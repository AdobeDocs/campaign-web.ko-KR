---
title: Campaign v8 Web 사용자 인터페이스 초기 릴리스 정보
description: 다음 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 126ebed5066bbc8c20d58d24e237b13f096b9d02
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 32%

---

# 초기 릴리스 정보 {#e-release}

Adobe Campaign Web 사용자 인터페이스는 지속적으로 새로운 기능, 기존 기능 개선, 버그 해결을 제공합니다. 모든 변경 사항은 매달 말에 [릴리스 정보](release-notes.md)에 통합됩니다.

**아래의 초기 릴리스 정보는 릴리스 예정일까지 사전 예고 없이 변경될 수 있습니다**. 링크, 화면 및 업데이트된 설명서는 릴리스 일자에 [릴리스 정보](release-notes.md)에 게시됩니다.

## 2025년 1월 릴리스 {#25-1-release}

**릴리스 날짜**: 2025년 2월 5일

다음 기능 및 개선 사항은 1월 릴리스부터 사용할 수 있습니다.

### 기능 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>시각적 조각 만들기 및 사용</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>시각적 조각은 여러 이메일 게재 간에 또는 콘텐츠 템플릿에서 재사용할 수 있는 사전 정의된 시각적 블록입니다. 이제 이 기능은 서버 빌드 8.6.4 이상에서 실행하는 모든 고객이 사용할 수 있습니다.</p>
<p>자세한 내용은 <a href="../content/use-visual-fragments.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>서드파티 시스템을 사용하여 게재 보내기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign 웹 사용자 인터페이스에서 외부 게재 및 외부 게재 템플릿을 정의할 수 있습니다. 이 모드에서는 메시지가 입력 파일에 생성되어 외부 공급자와 공유할 수 있습니다. 외부 게재 모드는 다이렉트 메일 채널의 기본 모드입니다.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>유형화를 사용하여 게재 전송 제어 및 필터링</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign 웹 사용자 인터페이스에서 유형화 및 유형화 규칙을 만들 수 있습니다. 유형화는 게재 전송에 대해 제어, 필터링 및 우선순위 지정을 수행할 수 있는 유형화 규칙 모음입니다. 유형화를 통해 게재에는 항상 필수 요소(예: 구독 취소 링크 또는 제목 줄) 또는 그룹을 의도한 타겟에서 제외하는 필터링 규칙(예: 구독 취소자, 경쟁업체 또는 비충성도 고객)이 포함되어 있는지 확인합니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>열거형 관리</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign 웹 사용자 인터페이스를 통해 직접 열거형을 만들 수 있습니다. 열거형은 필드를 채우기 위해 시스템에서 제안하는 값 목록입니다. 열거형을 사용하여 이러한 필드의 값을 표준화하고 데이터 입력 또는 쿼리 내에서 사용합니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>사용자 지정 옵션 만들기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign 웹 사용자 인터페이스 내의 기술 옵션에 액세스하고 필요에 따라 고유한 사용자 지정 옵션을 만들 수 있습니다. 이 기능은 JavaScript 코드 워크플로우 활동을 사용하여 중간 데이터를 저장할 때 특히 유용합니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Javascript 코드 정의 및 호출</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign 웹 사용자 인터페이스에서 JavaScript 코드를 만들 수 있습니다. 이를 통해 라이브러리와 유사하게 워크플로 전체에서 활용할 수 있는 재사용 가능한 기능을 만들 수 있습니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#25-1-improvements}

* 인터페이스에서 사용자 정의 필드 표시를 사용자 지정합니다.

   * 이제 인터페이스에 표시할 추가 사용자 정의 필드를 선택할 수 있습니다
   * 이제 다른 필드의 입력을 기준으로 목록 값을 제한하는 것과 같이, 링크 유형 사용자 정의 필드를 표시하기 위한 규칙을 설정할 수 있습니다
   * 이제 인터페이스에서 필드를 보다 유연하게 정렬할 수 있습니다. 필드는 단일 열에 걸쳐 있거나 하위 섹션으로 그룹화하여 구성을 높일 수 있습니다
   * 이제 특정 필드를 읽기 전용으로 설정할 수 있습니다.

* 최근 및 즐겨찾기 필터: 이제 자주 사용하는 속성을 빠르게 재사용하기 위해 즐겨찾기에 추가할 수 있습니다. 이를 통해 향후 작업을 위해 언제든지 액세스할 수 있습니다. 즐겨찾기 외에도 가장 최근에 선택한 속성을 보고 사용할 수도 있습니다.


