---
audience: end-user
title: 대기 워크플로우 활동 사용
description: 대기 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 42%

---


# 대기 {#wait}

다음 **대기** 활동은 워크플로우 특정 부분의 실행을 잠시 미룹니다. 몇 초에서 몇 달까지 대기한 후 아웃바운드 전환을 활성화하여 그 다음으로 배치한 활동을 실행합니다.

다음 **대기** 활동은 실행할 두 활동 사이에 일정 시간이 지나도록 하는 데 사용됩니다. 예를 들어 이메일 게재 활동 후 며칠 동안 대기하고, 후속 작업(리마인더 이메일, 대상자 만들기 등)을 수행하기 전에 대기 기간 동안 발생한 오픈 및 클릭을 분석하려 할 때 사용할 수 있습니다.

## 구성

다음 단계에 따라 **대기** 활동:

1. 추가 **대기** 활동을 워크플로우에 추가합니다.

1. 다음을 지정합니다. **기간** 활동의 인바운드 및 아웃바운드 전환이 활성화될 때까지의 대기 시간.

1. 시간 단위 선택 **기간**: 초, 분, 시간.

## 예제

