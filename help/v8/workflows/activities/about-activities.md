---
audience: end-user
title: 워크플로우 활동 작업
description: 워크플로우 활동 방법 알아보기
badge: label="알파"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: b66afeedbfcb342102c833899756afc35de9d504
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 6%

---


# 워크플로우 활동 기본 정보 {#workflow-activities}

워크플로우 활동은 세 가지 범주로 그룹화됩니다. 컨텍스트에 따라 사용 가능한 활동이 다를 수 있습니다.

모든 활동은 아래 섹션에 자세히 설명되어 있습니다.

* [타겟팅 활동](#targeting)
* [채널 활동](#channel)
* [흐름 제어 활동](#flow-control)

![](../assets/workflow-activities.png)

## 타겟팅 활동 {#targeting}

이러한 활동은 모집단 데이터를 타겟팅, 조작 및 보강하는 데 특정적입니다. 대상을 정의하고 교차, 결합 또는 제외 작업을 사용하여 이러한 대상을 분할 또는 결합하여 하나 이상의 대상을 작성할 수 있습니다.

* 다음 [대상자 작성](build-audience.md) 활동을 통해 대상 모집단을 정의할 수 있습니다. 기존 대상자를 선택하거나 규칙 빌더를 사용하여 쿼리를 정의할 수 있습니다.
* 다음 [결합](combine.md) 활동을 통해 인바운드 모집단에서 세분화를 수행할 수 있습니다. 유니온, 교집합 또는 제외를 사용할 수 있습니다.
* 다음 [데이터 보강](enrichment.md) 활동을 사용하면 워크플로우에서 처리할 추가 데이터를 정의할 수 있습니다. 이 활동을 사용하여 인바운드 전환을 활용하고 추가 데이터로 출력 전환을 완료하도록 활동을 구성할 수 있습니다.

## 채널 활동 {#channel}

Adobe Campaign 웹을 사용하면 이메일, SMS 또는 푸시와 같은 여러 채널에서 마케팅 캠페인을 자동화하고 실행할 수 있습니다. 채널 활동을 캔버스에 결합하여 고객 행동에 따라 작업을 트리거할 수 있는 크로스 채널 워크플로우를 만들 수 있습니다.

다음 **채널** 활동을 사용할 수 있습니다.

* 이메일
* 푸시
* SMS

이 [섹션](enrichment.md)을 참조하십시오.

## 흐름 제어 활동 {#flow-control}

다음 활동은 워크플로우 구성 및 실행과 관련이 있습니다. 이들의 주요 임무는 다른 활동을 조정하는 것입니다.

* 다음 [And-결합](and-join.md) 활동을 사용하면 워크플로우의 여러 실행 분기를 동기화할 수 있습니다.
* 다음 **종료** 활동을 사용하면 워크플로우의 끝을 그래픽으로 표시할 수 있습니다. 이 활동은 기능에 영향을 주지 않으므로 선택 사항입니다.
* 다음 [포크](fork.md) 활동을 사용하면 아웃바운드 전환을 만들어서 여러 활동을 동시에 시작할 수 있습니다.
* 다음 [대기](wait.md) 활동은 워크플로우 특정 부분의 실행을 잠시 미룹니다.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

