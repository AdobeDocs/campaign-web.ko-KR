---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 944fbbdd273cc402b88f2beaef5b15f2ce80cc6b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 83%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [이 페이지에](release-notes-24.md) 나열되어 있습니다.

## 2025년 1월 릴리스 {#25-1-release}

**릴리스 일자**: 2025년 2월 5일

1월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

### 기능 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>시각적 조각 만들기 및 사용하기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>시각적 조각은 여러 이메일 게재 또는 콘텐츠 템플릿에서 재사용할 수 있는 사전 정의된 시각적 블록입니다. 이 기능은 이제 서버 빌드 8.6.4 이상을 실행하는 모든 고객이 사용할 수 있습니다.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>자세한 내용은 <a href="../content/use-visual-fragments.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>서드파티 시스템을 사용하여 게재 전송</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign 웹 인터페이스에서 외부 게재와 외부 게재 템플릿을 정의할 수 있습니다. 이 모드에서 메시지는 출력 파일로 컴파일되며 외부 공급자와 공유할 수 있습니다. 기본적으로 외부 게재 모드는 다이렉트 메일(DM) 채널에 사용됩니다.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>자세한 내용은 <a href="../msg/send-external-deliveries.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

<table>
<thead>
<tr>
<th><strong>열거 관리</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스를 통해 직접 열거를 만들 수 있습니다. 열거는 필드를 채우기 위해 시스템이 제안하는 값의 목록입니다. 열거를 사용하여 이러한 필드의 값을 표준화하고, 쿼리 내에서 데이터 입력이나 사용을 돕습니다.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>자세한 내용은 <a href="../administration/enumerations.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>사용자 정의 옵션 만들기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 기술 옵션에 액세스하여 요구 사항에 맞는 사용자 정의 옵션을 직접 만들 수 있습니다. 이 기능은 특히 중간 데이터를 저장하기 위해 JavaScript 코드 워크플로 활동을 수행할 때 유용합니다.</p>
<img src="assets/do-not-localize/options.gif">
<p>자세한 내용은 <a href="../administration/options.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>JavaScript 코드 정의 및 호출</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 JavaScript 코드를 만들 수 있습니다. 이를 통해 라이브러리처럼 여러 워크플로에서 활용할 수 있는 재사용 가능한 함수를 만들 수 있습니다.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>자세한 내용은 <a href="../administration/javascript-codes.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>AI Assistant Content Accelerator를 사용하여 랜딩 페이지 생성</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 랜딩 페이지 게재에서 AI Assistant Content Accelerator를 사용하여 텍스트, 이미지 또는 전체 페이지 레이아웃을 생성할 수 있습니다.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>AI Assistant Content Accelerator에 대한 자세한 내용은 <a href="../email/generative-lp.md">자세한 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>




### 개선 사항 {#25-1-improvements}

* 인터페이스에서 사용자 정의 필드의 표시 사용자 정의:

   * 이제 인터페이스에서 표시할 추가 사용자 정의 필드를 선택할 수 있습니다.
   * 이제 다른 필드의 입력에 따라 목록 값을 제한하는 것과 같이 링크 유형 사용자 정의 필드를 표시하기 위한 규칙을 설정할 수 있습니다.
   * 이제 인터페이스에서 필드를 보다 유연하게 배열할 수 있습니다. 필드를 단일 열에 걸쳐 배치하거나 더 나은 구성을 위해 하위 섹션으로 그룹화할 수 있습니다.
   * 이제 특정 필드를 읽기 전용으로 설정할 수 있습니다.

* 최근 항목 및 즐겨찾기 필터: 자주 사용되는 속성을 빠르게 재사용하기 위해 이제 이를 즐겨찾기에 추가할 수 있습니다. 이렇게 하면 향후 작업에 간편하게 액세스할 수 있습니다. 즐겨찾기 외에도 가장 최근에 선택한 속성을 조회하고 사용할 수 있습니다.

* 외부 계정: 새 외부 계정을 만들 때 새 **[!UICONTROL 라우팅]** 유형을 선택할 수 있습니다. 외부 게재에서 사용할 특정 외부 계정을 구성할 수 있습니다. [자세히 알아보기](../administration/external-account.md#routing)