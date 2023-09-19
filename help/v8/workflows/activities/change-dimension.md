---
audience: end-user
title: 차원 변경 워크플로우 활동 사용
description: 차원 변경 워크플로우 활동을 사용하는 방법을 알아봅니다
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 6%

---


# 차원 변경 {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="보조 항목 생성"
>abstract="중복으로 제외된 나머지 모집단으로 추가 아웃바운드 전환을 생성할 수 있습니다. 이렇게 하려면 **보조 항목 생성** 옵션을 토글합니다"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="차원 활동 변경"
>abstract="이 활동을 통해 대상을 구축할 때 타겟팅 차원을 변경할 수 있습니다. 데이터 템플릿과 입력 차원에 따라 축을 이동합니다. 예를 들어 &quot;계약&quot; 차원에서 &quot;클라이언트&quot; 차원으로 전환할 수 있습니다."

다음 **차원 변경** 활동은 입니다. **타겟팅** 활동. 이 활동을 통해 대상을 구축할 때 타겟팅 차원을 변경할 수 있습니다. 이 활동은 데이터 템플릿과 입력 차원에 따라 축을 전환합니다. 예를 들어 &quot;계약&quot; 차원에서 &quot;클라이언트&quot; 차원으로 전환할 수 있습니다.

## 구성

다음 단계에 따라 **차원 변경** 활동:

1. 추가 **차원 변경** 활동을 워크플로우에 추가합니다.

   ![](../assets/workflow-change-dimension.png)

1. 다음을 정의합니다. **새 대상 차원**. 차원 변경 중에는 모든 레코드가 유지됩니다. 다른 옵션은 아직 사용할 수 없습니다.

1. 워크플로우를 실행하여 결과를 조회합니다. 차원 변경 활동 전후의 테이블에 있는 데이터를 비교하고 워크플로우 테이블의 구조를 비교합니다.



