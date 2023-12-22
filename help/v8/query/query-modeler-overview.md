---
audience: end-user
title: 쿼리 모델러로 작업
description: Adobe Campaign 웹 쿼리 모델러를 사용하여 작업하는 방법을 알아봅니다.
source-git-commit: 9992ae7007b5af80e927dd96b6fff25840d8c3e1
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 14%

---

# 쿼리 모델러로 작업 {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="새 쿼리 모델러"
>abstract="Adobe Campaign Web에는 다양한 기준에 따라 특정 대상을 선택하기 위해 데이터베이스를 필터링하는 프로세스를 단순화하는 쿼리 모델러가 있습니다. 여기에는 고급 표현식 및 연산자 사용이 포함됩니다. 쿼리 모델러는 데이터를 필터링할 규칙을 정의해야 하는 모든 컨텍스트에서 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="쿼리 모델러"
>abstract="데이터베이스의 수신자 또는 기타 타겟팅 차원에 대한 필터링 기준을 정의합니다. Adobe Experience Platform 대상자를 활용하여 타깃 대상자를 더욱 세분화하고 캠페인 효과를 극대화하십시오."

Adobe Campaign Web에는 다양한 기준에 따라 특정 대상을 선택하기 위해 데이터베이스를 필터링하는 프로세스를 단순화하는 쿼리 모델러가 있습니다. 여기에는 고급 표현식 및 연산자 사용이 포함됩니다.

## 쿼리 모델러에 액세스

쿼리 모델러는 데이터를 필터링할 규칙을 정의해야 하는 모든 컨텍스트에서 사용할 수 있습니다.

| 사용 | 예제 |
|  ---  |  ---  |
| **대상자 정의**: 메시지 또는 워크플로우에서 타겟팅할 모집단을 지정하고 필요에 따라 새로운 대상자를 손쉽게 만들 수 있습니다. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **워크플로우 활동 사용자 지정**: 특정 요구 사항에 맞게 분할 및 조정과 같은 워크플로우 활동 내에 규칙을 적용합니다. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **사전 정의된 필터**: 데이터 목록을 사용하거나 게재 대상을 구성하는 경우와 상관없이 다양한 필터링 작업 중에 바로 가기 역할을 하는 사전 정의된 필터를 만듭니다. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **보고서 데이터 필터링**: 보고서에 표시되는 데이터를 필터링하는 규칙을 추가합니다. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **목록 사용자 지정**: 사용자 지정 규칙을 만들어 수신자, 게재 목록 등과 같은 목록에 표시되는 데이터를 필터링합니다. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |



<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->


## 쿼리 모델러 인터페이스 {#interface}

쿼리 모델러는 쿼리를 작성하는 다른 구성 요소를 추가하고 결합할 수 있는 중앙 캔버스를 제공합니다.

오른쪽의 규칙 속성 창에는 쿼리에 대한 정보가 있습니다. 다양한 작업을 수행하여 쿼리를 확인하고 요구 사항에 맞는지 확인할 수 있습니다. 쿼리 확인 및 유효성 검사 방법 알아보기

![](assets/query-interface.png)
