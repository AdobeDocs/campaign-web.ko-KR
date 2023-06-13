---
audience: end-user
title: 대상자 시작
description: Campaign Web UI에서 대상자를 사용하는 방법 알아보기
badge: label="알파"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 30%

---


# 대상자 시작 {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


대상자는 게재의 주요 타겟인 메시지를 받는 수신자입니다. 대상자의 유형은 게재 템플릿에 정의된 대상 매핑에 따라 다릅니다. 게재 템플릿이란 무엇입니까? [이 섹션에서](../msg/delivery-template.md).

대상자 모집단을 정의하려면 다음을 수행할 수 있습니다.

* 클라이언트 콘솔에서 목록으로 작성된 기존 대상자를 선택합니다. [자세히 알아보기](add-audience.md)
* Adobe Experience Platform 대상자를 선택합니다. [자세히 알아보기](aep-audience.md)
* 필터링 기준을 정의하고 결합하여 규칙 빌더로 새 대상을 작성합니다. [자세히 알아보기](segment-builder.md)
* 외부 파일의 대상자 사용: 이 옵션은 독립 실행형 이메일 게재에만 사용할 수 있으며 캠페인 게재에는 사용할 수 없습니다. [자세히 알아보기](file-audience.md)

캠페인 워크플로우의 컨텍스트에서 메시지를 보낼 때 대상자는 특정 대상에 정의됩니다 **대상자 읽기** 워크플로우 활동. 이 컨텍스트에서는 이메일 게재를 위해 파일에서 대상자를 로드할 수 없으며 대상자는 이 전용 활동에서만 정의됩니다. 캠페인 워크플로우에서 게재 대상을 정의하는 방법을 알아봅니다 [이 섹션에서](../workflows/orchestrate-activities.md).

또한 대상자의 일부에 메시지를 전송하지 않도록 컨트롤 그룹을 정의하고 캠페인의 영향력을 측정할 수도 있습니다. [자세히 알아보기](control-group.md)

![](assets/about-audience.png)

