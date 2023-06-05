---
audience: end-user
title: 대상자 작성 워크플로우 활동 사용
description: 대상자 작성 워크플로우 활동을 사용하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 11%

---


# 대상자 빌드 {#build-audience}

다음 **대상자 작성** 활동은 입니다. **타겟팅** 활동. 이 활동을 통해 워크플로우에 들어갈 대상자를 정의할 수 있습니다. 캠페인 워크플로우의 컨텍스트에서 메시지를 보낼 때 메시지 대상자는 채널 활동에 정의되지 않고 **대상자 작성** 활동.

대상자 모집단을 정의하려면 다음을 수행할 수 있습니다.

* 클라이언트 콘솔에서 목록으로 작성된 기존 대상자를 선택합니다.
* Adobe Experience Platform 대상자를 선택합니다.
* 필터링 기준을 정의하고 결합하여 규칙 빌더로 새 대상을 작성합니다.

>[!NOTE]
>
>이 컨텍스트에서는 파일에서 대상을 로드할 수 없습니다. 이를 위해 독립 실행형 게재를 만들어야 합니다. [자세히 알아보기](../../audience/about-audience.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 구성

다음 단계에 따라 **대상자 작성** 활동:

1. 추가 **대상자 작성** 활동.
1. 레이블을 정의합니다.
1. 대상자 유형 정의: **나만의 콘텐츠 만들기** 또는 **대상자 읽기**.

자신만의 쿼리를 만들려면 다음 추가 단계를 수행합니다.

1. 선택 **나만의 쿼리 만들기**.
1. 다음을 선택합니다. **타겟팅 차원**. 타겟팅 차원을 사용하면 수신자, 약정 수혜자, 운영자, 구독자 등 작업에서 타겟팅하는 모집단을 정의할 수 있습니다. 기본적으로 대상은 수신자에서 선택됩니다. 다음을 참조하십시오. [v8 설명서](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. 클릭 **계속**.
1. 새 이메일을 디자인할 때 대상을 만드는 것과 같은 방식으로 규칙 빌더를 사용하여 쿼리를 정의합니다. 이 [섹션](../../audience/segment-builder.md)을 참조하십시오.

기존 대상자를 선택하려면 다음 단계를 따르십시오.

1. 선택 **대상자 읽기**.
1. 클릭 **계속**.
1. 새 이메일을 디자인할 때 대상을 사용하는 것과 동일한 방법으로 대상을 선택합니다. 이 [섹션](../../audience/add-audience.md)을 참조하십시오.

## 예제

다음은 두 개가 있는 워크플로의 예입니다 **대상자 작성** 활동. 첫 번째 대상은 포커 플레이어의 대상이며, 이메일 게재가 그 다음입니다. 두 번째 타겟은 VIP 클라이언트 대상, 그 다음 SMS 게재입니다.

![](../assets/workflow-audience-example.png)