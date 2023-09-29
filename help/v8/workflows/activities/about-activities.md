---
audience: end-user
title: 워크플로 활동을 사용하여 작업
description: 워크플로 활동을 사용하는 방법 알아보기
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: a8b73ba5664eedf473f09050602a61895993663e
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 86%

---


# 워크플로 활동 정보 {#workflow-activities}

워크플로 활동은 세 가지 카테고리로 그룹화됩니다. 컨텍스트에 따라 사용 가능한 활동이 다를 수 있습니다.

모든 활동은 아래 섹션에 자세히 설명되어 있습니다.

* [타겟팅 활동](#targeting)
* [채널 활동](#channel)
* [흐름 제어 활동](#flow-control)

![](../assets/workflow-activities.png)

## 타겟팅 활동 {#targeting}

이러한 활동은 모집단 데이터의 타겟팅, 조작 및 강화에만 해당됩니다. 이를 통해 대상자를 정의하고 교차, 합집합 또는 제외 작업을 사용하여 이러한 대상자를 분할 또는 결합하여 하나 이상의 대상을 빌드할 수 있습니다.

* 다음 [대상자 저장](save-audience.md) 활동을 사용하면 워크플로우에서 업스트림으로 계산한 모집단에서 기존 대상자를 업데이트하거나 새 대상자를 만들 수 있습니다.
* [대상자 빌드](build-audience.md) 활동을 통해 대상 모집단을 정의할 수 있습니다. 기존 대상자를 선택하거나 규칙 빌더를 사용하여 자체 쿼리를 정의할 수 있습니다.
* [결합](combine.md) 활동을 통해 인바운드 모집단에 대한 세분화를 수행할 수 있습니다. 합집합, 교차 또는 제외를 사용할 수 있습니다.
* [분할](split.md) 활동을 통해 수신 모집단을 여러 하위 집합으로 세그먼트화할 수 있습니다.
* [보강](enrichment.md) 활동을 사용하면 워크플로에서 처리할 추가 데이터를 정의할 수 있습니다. 이 활동을 사용하여 인바운드 전환을 활용하고 추가 데이터로 출력 전환을 완료하도록 활동을 구성할 수 있습니다.
* 다음 [중복 제거](deduplication.md) 활동을 통해 인바운드 활동의 결과에서 중복을 삭제할 수 있습니다.
* 다음 [차원 변경](change-dimension.md) 활동을 사용하면 워크플로우를 빌드할 때 타겟팅 차원을 변경할 수 있습니다.

## 채널 활동 {#channel}

Adobe Campaign Web을 사용하여 이메일, SMS 또는 푸시 등 여러 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. 채널 활동을 캔버스에 결합하여 고객 행동에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로를 만들 수 있습니다.

다음 **채널** 활동을 사용할 수 있습니다.

* 이메일
* 푸시
* SMS

이 [섹션](channels.md)을 참조하십시오.

## 흐름 제어 활동 {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="종료 활동"
>abstract="**종료** 활동을 사용하여 워크플로의 끝을 그래픽으로 표시할 수 있습니다. 이 활동은 기능에 영향을 미치지 않으므로 선택 사항입니다."

다음 활동은 워크플로의 구성 및 실행에만 적용됩니다. 주요 작업은 다음과 같은 다른 활동을 조정하는 것입니다.

* [스케줄러](scheduler.md) 활동을 사용하면 워크플로가 시작되는 시기를 예약할 수 있습니다.
* [AND-결합](and-join.md) 활동을 사용하면 워크플로의 여러 실행 분기를 동기화할 수 있습니다.
* **종료** 활동을 사용하여 워크플로의 끝을 그래픽으로 표시할 수 있습니다. 이 활동은 기능에 영향을 미치지 않으므로 선택 사항입니다.
* [포크](fork.md) 활동을 사용하면 아웃바운드 전환을 만들어서 여러 활동을 동시에 시작할 수 있습니다.
* [대기](wait.md) 활동은 워크플로 특정 부분의 실행을 잠시 미룹니다.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

