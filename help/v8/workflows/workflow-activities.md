---
audience: end-user
title: 워크플로우 활동 작업
description: 워크플로우 활동 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ebd119a38129f8576ad9b4e4b9301b116a255c9b
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 51%

---


# 워크플로 활동 {#workflow-activities}

## 타겟팅 활동 {#targeting}

이러한 활동을 통해 집합을 정의하고 교차, 결합 또는 제외 작업을 사용하여 이러한 집합을 분할 또는 결합하여 하나 이상의 대상을 빌드할 수 있습니다.

### 대상자 빌드 {#build-audience}

이 활동을 통해 대상자를 정의할 수 있습니다. 기존 Campaign 콘텐츠를 선택하거나 규칙 빌더를 사용하여 쿼리를 정의할 수 있습니다.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

다음 단계에 따라 **대상자 작성** 활동:

1. 대상자 작성 활동을 추가합니다.
1. 레이블을 정의합니다.
1. 대상자 유형 정의: **나만의 콘텐츠 만들기** 또는 **대상자 읽기**.

자신만의 쿼리를 만들려면 다음 추가 단계를 수행합니다.

1. 선택 **나만의 쿼리 만들기**.
1. 다음을 선택합니다. **타겟팅 차원**. 타겟팅 차원을 사용하면 수신자, 약정 수혜자, 운영자, 구독자 등 작업에서 타겟팅하는 모집단을 정의할 수 있습니다. 기본적으로 대상은 수신자에서 선택됩니다. 다음을 참조하십시오. [v8 설명서](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. 클릭 **계속**.
1. 새 이메일을 디자인할 때 대상을 만드는 것과 같은 방식으로 규칙 빌더를 사용하여 쿼리를 정의합니다. 이 [섹션](../audience/segment-builder.md)을 참조하십시오.

기존 대상자를 선택하려면 다음 단계를 따르십시오.

1. 선택 **대상자 읽기**.
1. 클릭 **계속**.
1. 새 이메일을 디자인할 때 대상을 사용하는 것과 동일한 방법으로 대상을 선택합니다. 이 [섹션](../audience/add-audience.md)을 참조하십시오.

### 결합 {#combine}

이 활동을 사용하면 인바운드 데이터에 대한 세트를 처리할 수 있습니다. 따라서 여러 모집단을 결합하고 일부를 제외하거나 데이터를 여러 대상에 공통된 상태로 유지할 수 있습니다. 사용 가능한 세분화 유형은 다음과 같습니다.

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* 다음 **합집합** 여러 활동의 결과를 하나의 타겟으로 다시 그룹화할 수 있습니다.
* 다음 **교차** 에서는 활동에서 다른 인바운드 모집단에 공통되는 요소만 유지할 수 있습니다.
* 다음 **제외** 특정 기준에 따라 한 모집단에서 요소를 제외할 수 있습니다.

다음 단계에 따라 **결합** 활동:

1. 사용자 추가 **결합** 활동을 이전 세그먼테이션 전환에 추가합니다.
1. 세분화 유형(결합, 교차 또는 제외)을 선택합니다.
1. 클릭 **계속**.
1. 다음에서 **가입하도록 설정** 섹션에서 가입하고자 하는 이전 활동을 모두 확인합니다.

의 경우 **합집합** 및 **교차**, 다음을 선택해야 합니다. **조정 유형** 중복 처리 방법을 정의하려면 다음을 수행합니다.

    * 키만 해당: 기본 모드입니다. 다른 인바운드 전환의 요소가 동일한 키를 가지면 활동은 한 요소만 유지합니다. 이 옵션은 인바운드 모집단이 동질적일 경우에만 사용할 수 있습니다.
    * 열 선택: 데이터 조정을 적용할 열 목록을 정의하려면 이 옵션을 선택합니다. 기본 세트(소스 데이터가 있는 세트)를 먼저 선택한 다음 결합에 사용할 열을 선택해야 합니다.

의 경우 **교차** 및 **제외**, 다음을 확인할 수 있습니다. **완료 생성** 나머지 모집단을 처리하려면 옵션을 선택합니다. 보충 자료에는 교차를 제외한 모든 인바운드 활동의 결과의 합집합도 포함됩니다. 그러면 추가 아웃바운드 전환이 활동에 추가됩니다.

의 경우 **제외**&#x200B;를 선택하고 **기본 세트** 인바운드 전환에서 **가입하도록 설정** 섹션. 요소가 제외되는 집합입니다. 다른 집합은 기본 집합에서 제외되기 전에 요소와 일치합니다.

### 보강 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="보강 활동"
>abstract="보강 활동을 사용하면 데이터베이스의 추가 정보로 타겟팅된 데이터를 보강할 수 있습니다. 일반적으로 활동을 타겟팅한 후 워크플로에서 사용됩니다.<br/>보강 데이터를 워크플로에 추가한 다음에는 이를 보강 활동 다음에 추가된 활동에서 사용하여 고객을 행동, 선호도 및 요구 사항에 따라 고유한 그룹으로 세분화하거나, 타겟 대상자의 마음을 움직일 수 있는 개인화된 마케팅 메시지 및 캠페인을 만들 수 있습니다."

보강 활동을 사용하면 데이터베이스의 추가 정보로 타겟팅된 데이터를 보강할 수 있습니다. 일반적으로 활동을 타겟팅한 후 워크플로에서 사용됩니다.

보강 데이터의 출처는 다음 중 하나일 수 있습니다.

* 워크플로로 타겟팅된 것과 **동일한 작업 테이블**:

   *고객 그룹 타겟팅 후 현재 작업 테이블에 “생년월일” 필드 추가*

* **다른 작업 테이블**:

   *고객 그룹 타겟팅 후 “구매” 테이블의 “수량” 및 “제품 유형” 필드 추가*

보강 데이터를 워크플로에 추가한 다음에는 이를 보강 활동 다음에 추가된 활동에서 사용하여 고객을 행동, 선호도 및 요구 사항에 따라 고유한 그룹으로 세분화하거나, 타겟 대상자의 마음을 움직일 수 있는 개인화된 마케팅 메시지 및 캠페인을 만들 수 있습니다.

예를 들어 고객의 구매와 관련된 워크플로 작업 테이블 정보를 추가한 다음, 이 데이터를 사용하여 해당 고객의 최근 구매 또는 이러한 구매에 지출한 금액으로 이메일을 개인화할 수 있습니다.

보강 활동을 워크플로에 추가하려면 다음 단계를 따르십시오.

1. 활동 추가
1. 보강 데이터로 사용할 속성 선택

   고급 필드 표시 옵션
i 버튼

   참고: 대상 차원의 속성

1. 데이터 수집 방법 선택
1. 여러 레코드 컬렉션을 검색하는 경우 검색할 레코드 수
1. 필터 적용 및 규칙 작성

   기존 필터 선택
재사용을 위해 필터 저장
필터 결과를 시각적으로 또는 코드 보기에서 보기

1. 속성을 사용하여 레코드 정렬

캠페인에서 보강 데이터 활용

보강 데이터를 사용할 수 있는 상황: 이메일 개인화, 기타 사용 사례?

## 채널 활동 {#channel}

Adobe Campaign 웹을 사용하면 이메일, SMS 또는 푸시와 같은 여러 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. Adobe Campaign 워크플로우를 사용하면 채널 활동을 캔버스에 결합하여 고객 행동에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로우를 만들 수 있습니다.

예를 들어 이메일, SMS 및 푸시와 같은 다양한 채널에 걸친 일련의 메시지를 포함하는 환영 이메일 캠페인을 만들 수 있습니다. 또한 고객이 구매를 완료한 후 후속 이메일을 보내거나 SMS를 통해 고객에게 개인화된 생일 메시지를 보낼 수도 있습니다.

채널 활동을 사용하면 여러 접점에서 고객을 참여시키고 전환을 유도하는 종합적이고 개인화된 캠페인을 만들 수 있습니다.

채널 활동은 화면 왼쪽에 있는 팔레트의 채널 섹션에서 사용할 수 있습니다.

### 이메일 {#email}

설명, 수행할 수 있는 사용 사례 (활동 전후에 연결할 수 있는 일반적인 기타 활동)

활동 추가 및 구성 방법

워크플로 내에서 구성된 활동의 예


이메일 게재 활동을 사용하면 워크플로우에서 이메일 전송을 구성할 수 있습니다.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

이메일 수신자는 대상자 타겟팅 활동을 통해 동일한 워크플로우에서 활동의 업스트림으로 정의됩니다.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### 푸시 알림 (Android) {#push-android}

### 푸시 알림 (iOS) {#push-ios}

## 흐름 제어 활동 {#flow-control}

콘텐츠 TBD

<!--à reformuler-->이러한 활동을 통해 집합을 정의하고 교차, 결합 또는 제외 작업을 사용하여 이러한 집합을 분할 또는 결합하여 하나 이상의 대상을 빌드할 수 있습니다.

흐름 제어 활동은 워크플로 활동을 조정하는 데 사용됩니다.

### 포크 {#fork}

### AND-결합 {#join}


### 대기 {#wait}

### 종료 {#end}

## 데이터 관리 활동 {#data-management}

개요: 채널 활동 사용의 목적
채널 활동으로 수행한 사용 사례

사용 가능한 활동 목록 + 간단한 설명 + 섹션 참조

