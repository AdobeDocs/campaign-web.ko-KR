---
audience: end-user
title: 워크플로우 종료 활동 사용
description: 종료 워크플로우 활동을 사용하는 방법 알아보기
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 20%

---

# 종료 {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="종료 활동"
>abstract="**종료** 활동을 사용하여 워크플로의 끝을 그래픽으로 표시할 수 있습니다. 두 개 이상의 인바운드 전환을 사용할 수 있는 경우 **가입하도록 설정** 섹션을 사용하여 활동에 연결할 전환을 선택하십시오."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="가입 설정"
>abstract="**End** 활동의 인바운드 전환으로 연결하려는 이전 활동을 확인하십시오. 선택한 활동이 **End**&#x200B;에 연결됩니다. 이 섹션은 두 개 이상의 인바운드 전환을 활동에 연결할 수 있는 경우에만 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="외부 신호"
>abstract="종료 활동 매개변수에서 외부 신호 섹션의 플레이스홀더. 오케스트레이션된 캠페인에만 사용할 수 있습니다. DELETE 금지"

**End** 활동은 **흐름 제어** 활동입니다. 워크플로우의 끝을 그래픽으로 표시할 수 있습니다. 이 활동은 선택 사항입니다.

두 개 이상의 인바운드 전환을 사용할 수 있는 경우 활동은 여러 인바운드 전환을 지원합니다.

**가입하도록 설정** 섹션에서 **End** 활동의 인바운드 전환으로 연결하려는 이전 활동을 확인하십시오. 그러면 선택한 활동이 워크플로 캔버스에서 **End**&#x200B;에 연결됩니다.

![워크플로우 중복 제거 구성 프로세스](../assets/workflow-end.png)
