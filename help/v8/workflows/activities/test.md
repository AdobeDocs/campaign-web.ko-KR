---
audience: end-user
title: 테스트 워크플로우 활동 사용
description: 테스트 워크플로우 활동을 사용하는 방법 알아보기
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 35%

---


# 테스트 {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="테스트 활동"
>abstract="**테스트** 활동은 **플로우 제어** 활동입니다. 이를 통해 지정된 조건에 따라 전환을 활성화할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="조건"
>abstract="**테스트** 활동에는 여러 개의 출력 전환이 있을 수 있습니다. 워크플로 실행 중에 각 조건은 그 중 하나가 충족될 때까지 순차적으로 테스트됩니다. 어떤 조건도 충족되지 않으면 워크플로는 **[!UICONTROL 기본 조건]** 경로를 따라 계속됩니다. 기본 조건이 활성화되어 있지 않으면 워크플로는 이 지점에서 멈춥니다."

**테스트** 활동은 **플로우 제어** 활동입니다. 이를 통해 지정된 조건에 따라 전환을 활성화할 수 있습니다.

## 테스트 활동 구성 {#test-configuration}

**테스트** 활동을 구성하려면 다음 단계를 따르십시오.

1. 워크플로우에 **Test** 활동을 추가합니다.

1. 기본적으로 **[!UICONTROL Test]** 활동은 간단한 부울 테스트를 제공합니다. &quot;참&quot; 전환에 정의된 조건이 충족되면 이 전환이 활성화됩니다. 그렇지 않으면 기본 &quot;False&quot; 전환이 활성화됩니다.

1. 전환과 연결된 조건을 구성하려면 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘을 클릭합니다. 표현식 편집기를 사용하여 이 전환을 활성화하는 데 필요한 규칙을 정의합니다. 이벤트 변수, 조건 및 날짜/시간 함수를 사용할 수도 있습니다. [이벤트 변수 및 식 편집기로 작업하는 방법을 알아봅니다](../event-variables.md).

   또한 **[!UICONTROL 레이블]** 필드를 수정하여 워크플로 캔버스에서 전환 이름을 개인화합니다.

   ![테스트 활동의 기본 구성](../assets/workflow-test-default.png)

1. **[!UICONTROL Test]** 활동에 여러 출력 전환을 추가합니다. 이렇게 하려면 **[!UICONTROL 조건 추가]** 단추를 클릭하고 각 전환에 대한 레이블과 관련 조건을 구성합니다.

1. 워크플로 실행 중에 각 조건은 그 중 하나가 충족될 때까지 순차적으로 테스트됩니다. 어떤 조건도 충족되지 않으면 워크플로는 **[!UICONTROL 기본 조건]** 경로를 따라 계속됩니다. 기본 조건이 활성화되어 있지 않으면 워크플로는 이 지점에서 멈춥니다.

## 예제 {#example}

이 예제에서 다른 전환은 **[!UICONTROL 대상자 작성]** 활동으로 타겟팅된 프로필 수에 따라 활성화됩니다.
* 타겟팅한 프로필이 10,000개가 넘는 경우 이메일 메시지가 전송됩니다.
* 1,000~10,000개의 프로필에 대해 SMS가 전송됩니다.
* 타겟팅된 프로필이 1,000개 미만이면 &quot;연락 안 함&quot; 전환으로 이동합니다.

![테스트 활동 전환의 예](../assets/workflow-test-example.png)

이를 위해 `vars.recCount` 이벤트 변수는 &quot;이메일&quot; 및 &quot;sms&quot; 조건에서 타겟팅된 프로필 수를 계산하고 적절한 전환을 활성화하는 데 사용됩니다.

![테스트 활동 구성 예](../assets/workflow-test-example-config.png)
