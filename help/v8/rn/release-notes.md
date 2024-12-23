---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [이 페이지에](release-notes-24.md) 나열되어 있습니다.

## 2024년 10월 릴리스 {#24-10-release}

**릴리스 일자**: 2024년 10월 29일

10월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

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
<p>이제 Adobe Campaign Web 사용자 인터페이스를 통해 외부 계정을 직접 설정하고 관리할 수 있습니다. 이 새로운 기능을 사용하면 바운스 이메일(POP3) 또는 실행 인스턴스 등 다양한 유형의 외부 계정을 간편하게 구성할 수 있습니다.</p>
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
<p>이제 Campaign web 사용자 인터페이스에서 트랜잭션 메시지(메시지 센터)를 사용할 수 있습니다. 이 추가 기능은 정보 시스템에서 트리거된 이벤트에서 생성되는 메시지를 트리거하도록 설계되었으며, 여기에는 인보이스, 주문 확인, 배송 확인, 암호 변경, 제품 사용 불가 알림, 계정 명세서, 웹 사이트 계정 생성 등이 포함될 수 있습니다.</p>
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

* **워크플로 활동** - 이제 워크플로 내에서 활동과 모든 하위 노드를 전환에서 다른 전환으로 옮길 수 있습니다. 활동의 속성 창에서 전용 **이동** 버튼을 사용하여 이 작업을 수행할 수 있습니다. [자세히 알아보기](../workflows/orchestrate-activities.md#move)

* **워크플로 보강 활동**

   * 이제 **보강** 활동에서 새 필드를 만들 때 별칭과 레이블을 정의할 수 있습니다. [자세히 알아보기](../workflows/activities/enrichment.md#collection-settings)
   * 이제 **보강** 활동에서 각 프로필에 대한 오퍼를 추가할 수 있습니다. [자세히 알아보기](../workflows/activities/enrichment.md##add-offers)

* **값 배포** - 개인화를 위해 필드 목록에 액세스할 때 이제 각 필드에 대한 값이 어떻게 배포되어 있는지 확인할 수 있습니다. 전용 팝업 창에 각 값에 대한 숫자와 백분율이 표시됩니다. [자세히 알아보기](../query/build-query.md#distribution-values-query)

* **버전 및 시스템 정보** - 이제 클라이언트 콘솔과 Web 사용자 인터페이스 모두에서 인스턴스 버전에 대한 세부 정보에 액세스할 수 있습니다. 이 새로운 섹션에는 사용자 환경에 설치된 모든 기본 제공 패키지도 나열됩니다. [자세히 알아보기](../get-started/user-interface.md#user-interface-about)

* **목록** - 이제 목록의 값을 간편하게 재정렬할 수 있습니다. [자세히 알아보기](../get-started/work-with-folders.md)

* **게재** - 이제 개인화 필드에서 게재 변수에 액세스할 수 있습니다. [자세히 알아보기](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)