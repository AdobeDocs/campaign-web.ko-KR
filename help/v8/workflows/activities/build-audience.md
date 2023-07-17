---
audience: end-user
title: 대상자 빌드 워크플로 활동 사용
description: 대상자 빌드 워크플로 활동을 사용하는 방법에 대해 알아봅니다.
badge: 레이블=“Alpha”
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '312'
ht-degree: 100%

---


# 대상자 빌드 {#build-audience}

**대상자 빌드** 활동은 **타겟팅** 활동입니다. 이 활동을 통해 워크플로에 참여할 대상자를 정의할 수 있습니다. 캠페인 워크플로 컨텍스트에서 메시지를 전송할 때 메시지 대상자는 채널 활동에서 정의되지 않고 **대상자 빌드** 활동에서 정의됩니다.

대상자 모집단을 정의하기 위해 수행할 수 있는 작업은 다음과 같습니다.

* 클라이언트 콘솔의 목록으로 생성된 기존 대상자를 선택합니다.
* Adobe Experience Platform 대상자를 선택합니다.
* 필터링 기준을 정의 및 결합하여 규칙 빌더를 통해 새로운 대상자를 빌드합니다.

>[!NOTE]
>
>이 컨텍스트에서는 파일에서 대상자를 로드할 수 없습니다. 이를 수행하려면 독립 실행형 게재를 만들어야 합니다. [자세히 알아보기](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 구성

**대상자 빌드** 활동을 구성하려면 다음 단계를 따르십시오.

1. **대상자 빌드** 활동을 추가합니다.
1. 레이블을 정의합니다.
1. **직접 만들기** 또는 **대상자 읽기 만들기**&#x200B;로 대상자 유형을 정의합니다.

자체 쿼리를 만들려면 다음 추가 단계를 따르십시오.

1. **직접 만들기(쿼리)**&#x200B;를 선택합니다.
1. **차원 타겟팅**&#x200B;을 선택합니다. 타겟팅 차원을 사용하면 수신자, 약정 수혜자, 운영자, 구독자 등 작업에서 타겟팅하는 모집단을 정의할 수 있습니다. 기본적으로 대상은 수신자 중에서 선택됩니다. [v8 설명서](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}를 참조하십시오.
1. **계속**&#x200B;을 클릭합니다.
1. 규칙 빌더를 사용하여 새 이메일을 디자인할 때, 대상자를 만드는 것과 같은 방식으로 쿼리를 정의하십시오. 이 [섹션](../../audience/segment-builder.md)을 참조하십시오.

기존 대상자를 선택하려면 다음 단계를 따르십시오.

1. **대상자 읽기**&#x200B;를 선택합니다.
1. **계속**&#x200B;을 클릭합니다.
1. 새 이메일을 디자인할 때 대상자를 사용하는 것과 같은 방식으로 대상자를 선택합니다. 이 [섹션](../../audience/add-audience.md)을 참조하십시오.

## 예제

다음은 두 가지 **대상자 빌드** 활동이 포함된 워크플로의 예입니다. 첫 번째는 포커 플레이어 대상자를 대상으로 하며 이메일 게재로 이어집니다. 두 번째는 VIP 클라이언트 대상자를 대상으로 하며 SMS 게재로 이어집니다.

![](../assets/workflow-audience-example.png)