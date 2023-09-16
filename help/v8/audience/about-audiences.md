---
audience: end-user
title: 대상자 시작하기
description: Campaign Web UI에서 대상자를 사용하는 방법 알아보기
badge: label="Beta"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: a61eb527f22346c51b935e4170e1a56bed428f78
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 98%

---


# 대상자 시작하기 {#about-audiences}

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


대상자는 게재의 기본 대상, 즉 메시지를 받는 수신자입니다. 대상자의 유형은 게재 템플릿에 정의된 대상 매핑에 따라 다릅니다. [이 섹션에서](../msg/delivery-template.md) 게재 템플릿의 정의에 대해 알아봅니다.

대상자 모집단을 정의하기 위해 수행할 수 있는 작업은 다음과 같습니다.

* 대상자를 만들고 결합합니다. [자세히 알아보기](create-audience.md)
* 클라이언트 콘솔의 목록으로 생성된 기존 대상자를 선택합니다. [자세히 알아보기](add-audience.md)
* Adobe Experience Platform 대상자를 선택합니다. [자세히 알아보기](aep-audience.md)
* 필터링 기준을 정의 및 결합하여 규칙 빌더를 통해 새로운 대상자를 빌드합니다. [자세히 알아보기](segment-builder.md)
* 외부 파일의 대상자 사용: 이 옵션은 독립 실행형 이메일 게재에만 사용할 수 있고 캠페인 게재에는 사용할 수 없습니다. [자세히 알아보기](file-audience.md)

캠페인 워크플로 컨텍스트에서 메시지를 전송할 때 대상자는 특정 **대상자 읽기** 워크플로 활동에 정의되어 있습니다. 이 컨텍스트에서는 이메일 게재용 파일에서 대상자를 로드할 수 없으며, 대상자는 이 전용 활동에서만 정의됩니다. [이 섹션](../workflows/orchestrate-activities.md)에서 캠페인 워크플로의 게재 대상자를 정의하는 방법에 대해 알아보십시오.

또한 대상자의 일부에 메시지를 전송하지 않도록 컨트롤 그룹을 정의하고 캠페인의 영향력을 측정할 수도 있습니다. [자세히 알아보기](control-group.md)

![](assets/about-audience.png)

