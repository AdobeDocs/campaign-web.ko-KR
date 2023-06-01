---
audience: end-user
title: AND-join 워크플로우 활동 사용
description: AND-join 워크플로우 활동을 사용하는 방법을 알아봅니다
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 4%

---


# AND-결합 {#join}

다음 **And-결합** 활동을 사용하면 워크플로우의 여러 실행 분기를 동기화할 수 있습니다.

AND-join 활동은 모든 인바운드 전환이 활성화되었을 때, 즉 앞선 활동이 모두 완료된 다음에만 아웃바운드 전환을 트리거합니다.

## 구성

다음 단계에 따라 **AND-결합** 활동:

1. 다음과 같은 여러 활동 추가 **결합** 활동은 두 개 이상의 서로 다른 실행 분기를 형성합니다.
1. 추가 **AND-결합** 모든 분기에 대한 활동.
1. 다음에서 **병합 옵션** 섹션에서 가입하고자 하는 이전 활동을 모두 확인합니다.
1. 다음 항목 선택 **기본 세트** 아웃바운드 전환에 남습니다.

## 예제

다음 예제는 이메일 및 SMS 게재를 사용하는 두 개의 워크플로우 분기를 보여 줍니다. 두 인바운드 전환이 모두 활성화되면 AND-join이 트리거됩니다. 그러면 두 게재가 모두 완료된 후에만 푸시 알림이 전송됩니다.

![](../assets/workflow-andjoin-example.png)