---
audience: end-user
title: Campaign 규칙 빌더로 대상자 빌드
description: 규칙 빌더로 작업하는 방법을 알아봅니다.
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 71%

---

# 규칙 빌더 작업 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Target 대상자"
>abstract="이제 그 어느 때보다 간단하게 게재 대상을 구축할 수 있습니다! 최신 규칙 빌더를 사용하면 데이터베이스의 수신자 또는 기타 타겟팅 차원에 대한 필터링 기준을 정의할 수 있습니다. Adobe Experience Platform 대상자를 활용하여 타깃 대상자를 더욱 세분화하고 캠페인 효과를 극대화하십시오."

규칙 빌더를 사용하면 데이터베이스에 포함된 데이터를 필터링하여 게재 대상의 모집단을 정의할 수 있습니다. 워크플로우에서 를 사용하여 대상자를 만드는 데 사용할 수 있습니다 **[!UICONTROL 대상자 작성]** 활동 또는 게재를 만들 때 일회성 대상을 직접 만들 수 있습니다.

* [대상자를 만드는 방법 알아보기](create-audience.md)
* [게재할 일회성 대상을 만드는 방법을 알아봅니다](one-time-audience.md)

## 팔레트

왼쪽에 있는 팔레트에는 대상자를 만들기 위해 필터링할 수 있는 모든 요소가 포함되어 있습니다. 검색 창을 사용하면 요소를 빠르게 찾을 수 있습니다. 팔레트에 포함된 타일을 구성하고 고려하려면 중앙 캔버스로 이동해야 합니다.

![](assets/segment-builder2.png){width="70%" align="left"}

팔레트는 두 개의 탭으로 나뉩니다.

* **속성**: 이 탭에서는 스키마에서 사용 가능한 모든 필드에 액세스할 수 있습니다. 필드 목록은 이메일 템플릿에 정의된 타겟팅 스키마에 따라 다릅니다.

* **대상자**: 이 탭에서는 Campaign Classic 콘솔 또는 Adobe Experience Platform에서 정의된 기존 대상 중 하나를 사용하여 필터링할 수 있습니다. [대상자 모니터링 및 관리 방법 알아보기](manage-audience.md)

  >[!NOTE]
  >
  >Adobe Experience Platform 대상자를 활용하려면 대상과의 통합을 구성해야 합니다. 다음을 참조하십시오. [Adobe Experience Platform 대상 설명서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html){target="_blank"}.

## 캔버스

캔버스는 팔레트에서 추가한 요소를 기반으로 규칙을 구성하고 결합할 수 있는 중앙 영역입니다. 새 규칙을 추가하려면 팔레트에서 타일을 드래그하여 캔버스에 놓습니다. 이렇게 하면 추가되는 데이터 유형에 따라 상황에 맞는 옵션을 볼 수 있습니다.

![](assets/segment-builder4.png){width="70%" align="left"}

## 규칙 속성 창

오른쪽에는 **규칙 속성** 창에서는 아래 나열된 작업을 수행할 수 있습니다.

![](assets/segment-builder5.png){width="70%" align="left"}

* **결과 보기:** 대상자에 의해 타겟팅되는 수신자 목록을 표시합니다.
* **코드 보기**: SQL에 대상자의 코드 기반 버전을 표시합니다.
* **고급 속성 표시**: 왼쪽 팔레트에서 노드, 그룹화, 1-1 링크, 1-N 링크와 같은 속성의 전체 목록을 보려면 이 옵션을 선택하십시오.
* **계산**: 쿼리가 타겟팅한 프로필 수를 업데이트하고 표시합니다.
* **필터 선택 또는 저장**: 사전 정의된 필터를 사용하여 쿼리를 필터링하거나 나중에 다시 사용할 수 있도록 쿼리를 새 필터로 저장합니다. [사전 정의된 필터로 작업하는 방법 알아보기](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >해당 버전의 제품에서는 사용자 인터페이스에서 미리 정의된 일부 필터를 사용할 수 없습니다. 계속 사용할 수 있습니다. [자세히 알아보기](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **속성**: 생성된 대상자에 대한 설명을 표시합니다.

## 예제

이 예제에서는 애틀랜타 또는 시애틀에 거주 중이며 1980년 이후 출생한 모든 고객을 대상으로 대상자를 구축합니다.

1. 팔레트의 **속성** 탭에서 **생년월일** 필드를 검색합니다. 타일을 드래그하여 캔버스에 놓습니다.

   ![](assets/segment-builder6.png)

1. 캔버스에서 **다음 날짜 이후** 연산자를 선택하고 원하는 날짜를 입력합니다.

   ![](assets/segment-builder7.png)

1. 팔레트에서 **도시** 필드를 검색한 다음 첫 번째 규칙 아래 캔버스에 추가합니다.

   ![](assets/segment-builder8.png)

1. 텍스트 필드에 첫 번째 도시 이름을 입력한 다음 Enter 키를 누릅니다.

   ![](assets/segment-builder9.png)

1. 두 번째 도시 이름에 대해 이 작업을 반복합니다.

   ![](assets/segment-builder10.png)

1. **결과 보기**&#x200B;를 클릭하여 쿼리와 일치하는 수신자 목록 및 수를 표시합니다. 열을 추가하여 데이터를 시각화하고 확인할 수도 있습니다. 이 예제에서는 **도시** 열을 추가하면 “애틀랜타”와 “시애틀”이 표시되어야 합니다.

   ![](assets/segment-builder11.png)

1. **확인**&#x200B;을 클릭합니다.
