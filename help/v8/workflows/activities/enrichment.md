---
audience: end-user
title: 데이터 보강 워크플로우 활동 사용
description: 데이터 보강 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 28%

---


# 보강 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="보강 활동"
>abstract="보강 활동을 사용하면 데이터베이스의 추가 정보로 타겟팅된 데이터를 보강할 수 있습니다. 일반적으로 타겟팅 활동 후 워크플로우에서 사용됩니다.<br/>보강 데이터를 워크플로에 추가한 다음에는 이를 보강 활동 다음에 추가된 활동에서 사용하여 고객을 행동, 선호도 및 요구 사항에 따라 고유한 그룹으로 세분화하거나, 타겟 대상자의 마음을 움직일 수 있는 개인화된 마케팅 메시지 및 캠페인을 만들 수 있습니다."

다음 **데이터 보강** 활동은 입니다. **타겟팅** 활동. 데이터베이스의 추가 정보로 타겟팅된 데이터를 향상시킬 수 있습니다. 일반적으로 세분화 활동 후 워크플로우에서 사용됩니다.

보강 데이터의 출처는 다음 중 하나일 수 있습니다.

* 워크플로로 타겟팅된 것과 **동일한 작업 테이블**:

   *고객 그룹 타겟팅 후 현재 작업 테이블에 “생년월일” 필드 추가*

* **다른 작업 테이블**:

   *고객 그룹 타겟팅 후 “구매” 테이블의 “수량” 및 “제품 유형” 필드 추가*

데이터 보강 데이터가 워크플로우에 추가되면 이후에 추가된 활동에서 사용할 수 있습니다. **데이터 보강** 활동은 고객의 비헤이비어, 환경 설정 및 요구 사항을 기반으로 고객을 개별 그룹으로 세분화하거나 타겟 대상자에게 반향을 일으킬 수 있는 개인화된 마케팅 메시지 및 캠페인을 만들기 위한 것입니다.

예를 들어 고객의 구매와 관련된 워크플로 작업 테이블 정보를 추가한 다음, 이 데이터를 사용하여 해당 고객의 최근 구매 또는 이러한 구매에 지출한 금액으로 이메일을 개인화할 수 있습니다.

## 일반 구성

다음 단계에 따라 **데이터 보강** 활동:

1. 다음과 같은 활동 추가 **대상자 작성** 및 **결합** 활동.
1. 추가 **데이터 보강** 활동.
1. 클릭 **데이터 보강 추가**.

![](../assets/workflow-enrichment1.png)

대상 차원의 단일 속성 또는 컬렉션 링크의 두 가지 데이터 유형을 선택할 수 있습니다.

## 단일 속성

여기에서는 하나의 데이터 보강 속성(예: 출생 데이터)을 추가하기만 하면 됩니다. 다음 단계를 수행하십시오.

1. 내부를 클릭합니다. **속성** 필드.
1. 타겟팅 차원에서 단순 필드를 선택합니다. 이 예제에서는 생년월일을 선택합니다.
1. **확인**&#x200B;을 클릭합니다.

![](../assets/workflow-enrichment2.png)

## 컬렉션 링크

이 보다 복잡한 사용 사례에서는 테이블 간에 1-N 카디널리티가 있는 링크인 컬렉션 링크를 선택합니다. 100$ 미만의 최신 구매 내역 3개를 검색해 보겠습니다. 이를 위해 다음을 정의해야 합니다.

* 속성: **총 금액** 필드
* 검색할 라인 수: 3
* 필터: 100$보다 큰 항목 필터링
* a sorting: 하위 항목 정렬 **주문 날짜** 필드.

다음 단계를 수행하십시오.

### 속성 추가

여기서 데이터 보강 데이터로 사용할 컬렉션 링크를 선택합니다.

1. 내부를 클릭합니다. **속성** 필드.
1. 클릭 **고급 속성 표시**.
1. 다음 항목 선택 **총 금액** 의 필드 **구매** 테이블.

![](../assets/workflow-enrichment3.png)

### 컬렉션 설정 정의

그런 다음 데이터 수집 방법과 검색할 레코드 수를 정의합니다.

1. 선택 **데이터 수집** 다음에서 **데이터 수집 방법 선택** 드롭다운.
1. 에 &quot;3&quot;을 입력합니다 **검색할 라인(생성할 열)** 필드.

![](../assets/workflow-enrichment4.png)

예를 들어, 고객에 대한 평균 구매 금액을 얻으려면 다음을 선택합니다. **집계된 데이터** 대신 을 선택하고 **평균** 다음에서 **집계 함수** 드롭다운.

![](../assets/workflow-enrichment5.png)

### 필터 정의

여기에서는 속성에 대한 최대값을 정의합니다. 100$보다 큰 항목을 필터링합니다.

1. 클릭 **필터 편집**.
1. 다음 두 필터를 추가합니다. **총 금액** 존재함 및 **총 금액** 은(는) 100보다 작습니다. 첫 번째 필터는 NULL 값을 가장 큰 값으로 표시되는 그대로 필터링합니다.
1. **확인**&#x200B;을 클릭합니다.

![](../assets/workflow-enrichment6.png)

### 정렬 정의

이제 세 가지를 검색하기 위해 정렬을 적용해야 합니다 **최신** 구매.

1. 활성화 **정렬 활성화** 옵션을 선택합니다.
1. 내부를 클릭합니다. **속성** 필드.
1. 다음 항목 선택 **주문 날짜** 필드.
1. **확인**&#x200B;을 클릭합니다.
1. 선택 **내림차순** 다음에서 **정렬** 드롭다운.

![](../assets/workflow-enrichment7.png)

<!--
cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->