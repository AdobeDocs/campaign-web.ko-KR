---
audience: end-user
title: 예약 워크플로우 활동 사용
description: 스케줄러 워크플로우 활동을 사용하는 방법 알아보기
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 9%

---

# 예약 {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Scheduler activity"
>abstract="The **Scheduler** activity allows you to schedule when the workflow gets started. This activity should be considered as a scheduled start. It can only be used as the first activity of the workflow."

## 모범 사례 {#scheduler-best-practices}

* 워크플로우가 전체 시스템 성능을 저해하고 데이터베이스에 블록을 만들 수 있으므로 워크플로우를 15분 이상 실행하도록 예약하지 마십시오.
* 워크플로우에서 일회성 게재를 보내려면 스케줄러 활동을 추가하고 **Once**&#x200B;을(를) 실행하도록 설정하십시오. 게재 설정에서 **일정**&#x200B;을(를) 정의합니다.
* 워크플로우에서 반복 게재를 보내려면 **스케줄러** 활동을 사용하고 실행 빈도를 설정하십시오. 반복 게재 활동에서는 일정을 정의할 수 없습니다.

## 스케줄러 활동 구성 {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Scheduler validity"
>abstract="You can define a validity period for the scheduler. It can be permanent (default), or can be valid until a specific date."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler options"
>abstract="Define the frequency of the scheduler. It can be executed at a specific moment, once or several times a day, week or month."

**스케줄러** 활동을 구성하려면 다음 단계를 따르십시오.

![스케줄러 활동 구성 인터페이스](../assets/workflow-scheduler.png)

1. 워크플로우에 **스케줄러** 활동을 추가합니다.

1. **실행 빈도**&#x200B;를 구성합니다.

   * **한 번**: 워크플로우가 한 번 실행됩니다.
   * **일별**: 워크플로우가 하루에 한 번, 지정한 시간에 실행됩니다.
   * **하루에 여러 번**: 워크플로우가 하루에 여러 번 규칙적으로 실행됩니다. 특정 시간 또는 주기적으로 실행을 설정합니다.
   * **주별**: 워크플로우가 일주일에 한 번 또는 여러 번, 지정한 시점에 실행됩니다.
   * **월별**: 워크플로우가 한 달에 한 번 또는 여러 번, 지정한 시점에 실행됩니다. 워크플로우를 실행해야 하는 월을 선택합니다. 해당 월의 지정된 평일(예: 해당 월의 두 번째 화요일)에 실행을 설정할 수도 있습니다.

1. 선택한 빈도에 따라 실행의 세부 정보를 정의합니다. 세부 정보 필드는 사용되는 빈도(시간, 반복 빈도, 지정된 날짜 및 유사한 옵션)에 따라 달라질 수 있습니다.

1. **실행 시간 미리 보기**&#x200B;를 클릭하여 워크플로우의 다음 10개 실행 일정을 확인합니다.

1. 스케줄러의 유효 기간을 정의합니다.

   * **영구(만료되지 않음)**: 워크플로우가 시간 프레임이나 반복 횟수 제한 없이 지정한 빈도대로 실행됩니다.
   * **유효 기간**: 워크플로우가 특정 날짜까지 지정한 빈도대로 실행됩니다. 시작 및 종료 날짜를 지정합니다.

>[!NOTE]\
워크플로를 바로 시작하려면 예약의 상단 작업 표시줄에서 **보류 중인 작업 실행**&#x200B;을 클릭하세요. 이 단추는 워크플로우가 시작된 경우에만 사용할 수 있습니다.

## 예제 {#scheduler-example}

다음 예제에서는 워크플로우가 2023년 10월 1일부터 2024년 1월 1일까지 매일 오전 9시와 12시에 하루에 여러 번 실행되도록 구성되어 있습니다.

![스케줄러 활동 예제 구성](../assets/workflow-scheduler2.png)