---
audience: end-user
title: 게재를 위한 일회성 대상 구축
description: 게재를 위한 일회성 대상을 구축하는 방법을 알아봅니다.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 31%

---

# 일회성 대상자 빌드 {#one-time}

이 섹션에서는 새 게재를 만들 때 대상을 구축하는 방법을 설명합니다. 이 경우 쿼리 모델러를 사용하여 데이터베이스를 쿼리하여 게재 대상자에 포함할 프로필을 타겟팅합니다.

결과 대상자는 이 게재에 한 번만 사용됩니다. 대상자 목록에 저장되지 않습니다.

게재의 기본 대상을 정의할 때 다음을 수행할 수도 있습니다.

* [기존 대상자 선택](add-audience.md) 다음에서 **[!UICONTROL 대상]** 목록을 표시합니다.
* [외부 파일에서 대상자 로드](file-audience.md) (이메일에만 해당).

게재에서 직접 새 대상을 작성하려면 다음 단계를 수행합니다.

1. 게재 생성 도우미의 **대상자** 섹션에서 **[!UICONTROL 대상자 선택]** 버튼을 클릭합니다.

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. **직접 만들기**&#x200B;를 선택합니다. 쿼리 모델러가 표시됩니다. 데이터베이스에 포함된 데이터를 필터링하여 게재 대상의 모집단을 정의할 수 있습니다. [쿼리 모델러를 사용하는 방법 알아보기](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. 쿼리가 준비되면 **확인** 게재의 주요 타겟으로 대상자를 사용합니다.

   캠페인의 영향을 측정하기 위해 컨트롤 그룹을 설정할 수도 있습니다. 컨트롤 그룹은 메시지를 받지 않습니다. 그러면 메시지를 받은 모집단과 메시지를 받지 않은 연락처의 동작을 비교할 수 있습니다. [자세히 알아보기](control-group.md)
