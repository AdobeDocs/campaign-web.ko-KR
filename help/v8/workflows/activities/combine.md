---
audience: end-user
title: 결합 워크플로 활동 사용
description: 결합 워크플로 활동을 사용하는 방법에 대해 알아봅니다.
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 32%

---

# 결합 {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="활동 결합"
>abstract="**결합** 활동을 통해 인바운드 모집단에 대한 세분화를 수행할 수 있습니다. 여러 모집단을 결합하거나, 일부를 제외하거나, 여러 대상에 공통되는 데이터만 유지할 수 있습니다."

**결합** 활동은 **타깃팅** 활동입니다. 이 활동을 통해 인바운드 모집단에 대한 세분화를 수행할 수 있습니다. 여러 모집단을 결합하거나, 일부를 제외하거나, 여러 대상에 공통되는 데이터만 유지할 수 있습니다. 사용 가능한 세분화 유형은 다음과 같습니다.

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* **Union**&#x200B;이(가) 여러 작업의 결과를 하나의 대상으로 다시 그룹화합니다.
* **교차**&#x200B;은(는) 활동에서 다른 인바운드 모집단에 공통되는 요소만 유지합니다.
* **Exclusion**&#x200B;은(는) 특정 기준에 따라 하나의 모집단에서 요소를 제외합니다.

## 결합 활동 구성 {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="교차 병합 옵션"
>abstract="교차는 활동에서 다른 인바운드 모집단에 공통되는 요소만 유지합니다. 가입할 설정 섹션에서 가입하려는 이전 활동을 모두 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="제외 병합 옵션"
>abstract="제외는 특정 기준에 따라 한 모집단에서 요소를 제외합니다. 가입할 설정 섹션에서 가입하려는 이전 활동을 모두 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="세분화 유형 선택"
>abstract="대상자 결합 방법을 선택합니다. **Union**&#x200B;이(가) 여러 작업의 결과를 하나의 대상으로 다시 그룹화합니다. **교차**&#x200B;은(는) 활동에서 다른 인바운드 모집단에 공통되는 요소만 유지합니다. **Exclusion**&#x200B;은(는) 특정 기준에 따라 하나의 모집단에서 요소를 제외합니다."

다음과 같은 일반적인 단계에 따라 **결합** 활동을 구성하십시오.

![](../assets/workflow-combine.png)

1. **대상자 작성** 활동 등 여러 활동을 추가하여 두 개 이상의 실행 분기를 만듭니다.
1. 이전 분기에 **결합** 활동을 추가합니다.
1. 세분화 유형: [유니온](#union), [교차](#intersection) 또는 [제외](#exclusion)를 선택하십시오.
1. **계속**&#x200B;을 클릭합니다.
1. **가입하도록 설정** 섹션에서 가입하려는 이전 활동을 모두 확인하십시오.

## 합집합 {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="조정 옵션"
>abstract="중복 처리 방법을 정의하려면 **조정 유형**&#x200B;을 선택합니다. 기본적으로 **Keys** 옵션이 활성화됩니다. 즉, 다른 인바운드 전환의 요소가 동일한 키를 가지면 활동에서 한 요소만 유지합니다. 데이터 조정을 적용할 열 목록을 정의하려면 **열 선택** 옵션을 사용합니다."

**결합** 활동에서 **조정 유형**&#x200B;을(를) 선택하여 **결합**&#x200B;을(를) 구성하여 중복 처리 방법을 정의합니다.

* **키만**: 기본 모드입니다. 다른 인바운드 전환의 요소가 동일한 키를 가지면 활동은 한 요소만 유지합니다. 이 옵션은 인바운드 모집단이 동질적일 경우에만 사용할 수 있습니다.
* **열 선택**: 데이터 조정을 적용할 열 목록을 정의하려면 이 옵션을 선택하십시오. 먼저 기본 세트(소스 데이터)를 선택한 다음 결합에 사용할 열을 선택합니다.

## 교차 {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="교집합 조정 옵션"
>abstract="중복 처리 방법을 정의하려면 **조정 유형**&#x200B;을 선택합니다. 기본적으로 **Keys** 옵션이 활성화됩니다. 즉, 다른 인바운드 전환의 요소가 동일한 키를 가지면 활동에서 한 요소만 유지합니다. 데이터 조정을 적용할 열 목록을 정의하려면 **열 선택** 옵션을 사용합니다."

**결합** 활동에서 다음 추가 단계를 수행하여 **교차**&#x200B;을 구성하십시오.

1. 중복 처리 방법을 정의하려면 **조정 유형**&#x200B;을 선택합니다. [합집합](#union) 섹션을 참조하십시오.
1. 나머지 모집단을 처리하려면 **보조 항목 생성** 옵션을 선택하십시오. 보충 자료에는 모든 인바운드 활동의 결과에서 교차를 뺀 합집합도 포함됩니다. 그런 다음 추가적인 아웃바운드 전환이 활동에 추가됩니다.

## 제외 {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="제외 규칙"
>abstract="필요한 경우 인바운드 테이블을 조작합니다. 다른 차원에서 대상을 제외하려면 이 대상을 주 대상과 동일한 타겟팅 차원으로 되돌립니다. 제외 규칙 섹션에서 규칙 추가 를 클릭하고 차원 변경 조건을 지정합니다. 데이터 조정은 속성 또는 참여를 통해 수행됩니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="결합할 세트 선택"
>abstract="**참여 설정** 섹션에서 인바운드 전환의 **기본 세트**&#x200B;를 선택합니다. 요소가 제외되는 집합입니다. 다른 집합은 기본 집합에서 제외되기 전에 요소와 일치합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="제외 규칙"
>abstract="필요한 경우 인바운드 테이블을 조작합니다. 다른 차원에서 대상을 제외하려면 이 대상을 주 대상과 동일한 타겟팅 차원으로 되돌립니다. 제외 규칙 섹션에서 규칙 추가 를 클릭하고 차원 변경 조건을 지정합니다. 데이터 조정은 속성 또는 참여를 통해 수행됩니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="여집합 결합 생성"
>abstract="추가 전환에서 나머지 집단을 처리하려면 ‘여집합 생성’ 옵션을 토글합니다."

**결합** 활동에서 다음 추가 단계를 수행하여 **제외**&#x200B;을(를) 구성하십시오.

1. **참여 설정** 섹션에서 인바운드 전환의 **기본 세트**&#x200B;를 선택합니다. 요소가 제외되는 집합입니다. 다른 집합은 기본 집합에서 제외되기 전에 요소와 일치합니다.
1. 필요한 경우 인바운드 테이블을 조작합니다. 다른 차원에서 대상을 제외하려면 이 대상을 주 대상과 동일한 타겟팅 차원으로 되돌립니다. **제외 규칙** 섹션에서 **규칙 추가**&#x200B;를 클릭하고 차원 변경 조건을 지정하십시오. 데이터 조정은 속성 또는 참여를 통해 수행됩니다.
1. 나머지 모집단을 처리하려면 **보조 항목 생성** 옵션을 선택하십시오. [교차](#intersection) 섹션을 참조하십시오.

## 예제 {#combine-examples}

다음 예제에서는 **Combine** 활동에서 **Union**&#x200B;을(를) 사용하여 두 쿼리의 모든 프로필을 검색합니다. 18세에서 27세 사이의 사용자 및 34세에서 40세 사이의 사용자.

![](../assets/workflow-union-example.png)

다음 예제에서는 두 쿼리 활동 간의 **교차**&#x200B;를 보여 줍니다. 18세에서 27세 사이의 프로필 및 이메일 주소가 제공된 프로필을 검색합니다.

![](../assets/workflow-intersection-example.png)

다음 **제외** 예제는 18세에서 27세 사이의 프로필로 필터링하도록 구성된 두 개의 쿼리와 Adobe 이메일 도메인을 보여 줍니다. Adobe 이메일 도메인이 있는 프로필은 첫 번째 집합에서 제외됩니다.

![](../assets/workflow-exclusion-example.png)