---
audience: end-user
title: 포크 워크플로우 활동 사용
description: 포크 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 1ac80ffaabea210bbc02588475ad6e81af4820b1
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 21%

---


# 포크 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="포크 활동"
>abstract="포크 활동을 사용하면 아웃바운드 전환을 만들어서 여러 활동을 동시에 시작할 수 있습니다."

## 구성

다음 단계에 따라 **포크** 활동:

1. 추가 **포크** 활동을 워크플로우에 추가합니다.
1. 클릭 **전환 추가** 새 아웃바운드 전환을 추가합니다. 기본적으로 두 개의 전환이 정의됩니다.
1. 각 전환에 레이블을 추가합니다.

## 예제

다음 예제에서는 두 가지를 사용합니다 **포크** 활동:

* 두 쿼리 앞에 한 개 추가하여 동시에 실행합니다.
* 교차 후 하나에서 타겟팅된 모집단으로 이메일과 SMS를 동시에 전송합니다.

![](../assets/workflow-fork-example.png)

