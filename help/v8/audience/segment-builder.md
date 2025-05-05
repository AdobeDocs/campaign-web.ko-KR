---
audience: end-user
title: Campaign 규칙 빌더로 대상자 빌드
description: 규칙 빌더로 작업하는 방법을 알아봅니다.
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 24%

---

# 규칙 빌더를 사용하여 작업 {#segment-builder}

규칙 빌더를 사용하면 데이터베이스에 포함된 데이터를 필터링하여 게재 대상의 모집단을 정의할 수 있습니다. **[!UICONTROL 대상자 작성]** 활동을 사용하는 워크플로우에서 대상자를 만들거나 게재를 만들 때 직접 작성하여 일회성 대상자를 만드는 데 사용합니다.

* [대상자를 만들고 저장하는 방법 알아보기](create-audience.md)
* [게재할 일회성 대상을 만드는 방법을 알아봅니다](one-time-audience.md)

## 팔레트

왼쪽에 있는 팔레트에는 대상자를 만들기 위해 필터링할 수 있는 모든 요소가 포함되어 있습니다. 검색 창을 사용하여 요소를 빠르게 찾습니다. 팔레트에 포함된 타일을 중앙 캔버스로 이동하여 구성하고 고려합니다.

![필터링 옵션 및 탭을 표시하는 팔레트 인터페이스](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

팔레트는 두 개의 탭으로 나뉩니다.

* **특성**: 이 탭에서는 스키마에서 사용 가능한 모든 필드에 액세스할 수 있습니다. 필드 목록은 이메일 템플릿에 정의된 타겟팅 스키마에 따라 다릅니다.

* **대상**: 이 탭에서는 Campaign Classic 콘솔 또는 Adobe Experience Platform에 정의된 기존 대상 중 하나를 사용하여 필터링할 수 있습니다. [이 섹션](manage-audience.md)에서 대상을 모니터링하고 관리하는 방법을 알아보세요.

  >[!NOTE]
  >
  >Adobe Experience Platform 대상을 사용하려면 대상과의 통합을 구성합니다. [Adobe Experience Platform 대상 설명서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=ko){target="_blank"}를 참조하세요.

## 캔버스

캔버스는 팔레트에서 추가한 요소를 기반으로 규칙을 구성하고 결합할 수 있는 중앙 영역입니다. 새 규칙을 추가하려면 팔레트에서 타일을 드래그하여 캔버스에 놓습니다. 추가되는 데이터 유형에 따라 컨텍스트별 옵션이 표시됩니다.

![규칙 구성 옵션을 표시하는 캔버스 인터페이스](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## 규칙 속성 창

오른쪽의 **규칙 속성** 창에서 아래 나열된 작업을 수행할 수 있습니다.

![사용 가능한 작업을 표시하는 규칙 속성 창](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **결과 보기:** 대상자가 타겟팅한 프로필 목록을 표시합니다.
* **코드 보기**: SQL에서 대상자의 코드 기반 버전을 표시합니다.
* **고급 특성 표시**: 왼쪽 팔레트에서 노드, 그룹화, 1-1 링크 및 1-N 링크를 포함한 전체 특성 목록을 보려면 이 옵션을 선택하십시오.
* **계산**: 쿼리의 대상 프로필 수를 업데이트하고 표시합니다.
* **필터 선택 또는 저장**: 미리 정의된 필터를 사용하여 쿼리를 필터링하거나 나중에 다시 사용할 수 있도록 쿼리를 새 필터로 저장합니다. [미리 정의된 필터로 작업하는 방법을 알아봅니다](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >이 제품 버전에서는 사용자 인터페이스에서 사전 정의된 일부 필터를 사용할 수 없습니다. 일반적인 사용은 가능합니다. [자세히 알아보기](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **특성**: 만들어진 대상자에 대한 설명을 표시합니다.

## 예제

이 예에서는 대상이 Atlanta 또는 Seattle에 거주하며 1980년 이후에 태어난 모든 고객을 타깃팅하도록 빌드되었습니다.

1. 팔레트의 **속성** 탭에서 **생년월일** 필드를 검색합니다. 타일을 드래그하여 캔버스에 놓습니다.

   ![생년월일 필드를 캔버스에 추가](assets/segment-builder6.png){zoomable="yes"}

1. 캔버스에서 **다음 날짜 이후** 연산자를 선택하고 원하는 날짜를 입력합니다.

   ![생년월일 필드에 대한 After 연산자 구성](assets/segment-builder7.png){zoomable="yes"}

1. 팔레트에서 **도시** 필드를 검색한 다음 첫 번째 규칙 아래 캔버스에 추가합니다.

   ![캔버스에 도시 필드 추가](assets/segment-builder8.png){zoomable="yes"}

1. 텍스트 필드에 첫 번째 도시 이름을 입력한 다음 Enter 키를 누릅니다.

   ![구/군/시 필드에 구/군/시 이름을 입력합니다](assets/segment-builder9.png){zoomable="yes"}

1. 두 번째 도시 이름에 대해 이 작업을 반복합니다.

   ![구/군/시 필드에 두 번째 구/군/시 이름을 입력합니다](assets/segment-builder10.png){zoomable="yes"}

1. **결과 보기**&#x200B;를 클릭하여 쿼리와 일치하는 수신자 목록 및 수를 표시합니다. 열을 추가하여 데이터를 시각화하고 확인합니다. 이 예제에서는 **City** 열을 추가하여 Atlanta와 Seattle을 확인합니다.

   ![구/군/시 열이 추가된 결과 보기](assets/segment-builder11.png){zoomable="yes"}

1. **확인**&#x200B;을 클릭합니다.