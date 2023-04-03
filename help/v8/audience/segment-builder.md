---
audience: end-user
title: 규칙 빌더로 대상 정의
description: 세그먼트 빌더로 작업하는 방법 알아보기
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 1%

---

# 규칙 빌더로 대상 정의 {#segment-builder}

이 섹션에서는 새 이메일을 디자인할 때 대상자를 만드는 방법을 설명합니다. 만든 대상자는 이 이메일에서만 사용할 수 있습니다.

규칙 빌더를 사용하면 데이터베이스에 포함된 데이터를 필터링하여 메시지가 타겟팅하는 모집단을 정의할 수 있습니다. 기존 대상자를 선택하려면 이 항목을 참조하십시오 [섹션](add-audience.md).

규칙 빌더에 대한 자세한 내용은 [Segmentation Service 설명서](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

이메일을 디자인할 때 새 대상자를 만들려면 다음 단계를 수행하십시오.

1. 에서 **Audience** 게재 만들기 도우미의 섹션에서 **[!UICONTROL 대상 선택]** 버튼을 클릭합니다.

   ![](assets/segment-builder0.png)

1. 선택 **직접 만들기**. 규칙 빌더가 표시됩니다.

   ![](assets/segment-builder.png)

## 팔레트

왼쪽에 있는 팔레트에는 대상자를 만들기 위해 필터링할 수 있는 모든 요소가 포함되어 있습니다. 구성 및 고려하려면 팔레트에 포함된 타일을 중앙 캔버스로 이동해야 합니다. 팔레트는 다음 두 개의 탭으로 나뉘어 있습니다.

* **속성**: 이 탭에서는 스키마에서 사용 가능한 모든 필드에 액세스할 수 있습니다. 필드 목록은 전자 메일 템플릿에 정의된 타겟팅 스키마에 따라 다릅니다.

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **대상**: 이 탭에서는 Campaign Classic 콘솔 또는 Adobe Experience Platform에서 정의된 기존 대상 중 하나를 사용하여 필터링할 수 있습니다.

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >Adobe Experience Platform 대상을 활용하려면 대상과의 통합을 구성해야 합니다. 자세한 내용은 [대상 설명서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=ko){target="_blank"}.

검색 창을 사용하여 요소를 빠르게 찾을 수 있습니다.

## 캔버스

캔버스는 팔레트에서 추가한 요소를 기반으로 규칙을 구성하고 결합할 수 있는 중앙 영역입니다. 새 규칙을 추가하려면 팔레트에서 타일을 캔버스에 끌어다 놓습니다. 그런 다음 추가되는 데이터의 유형에 따라 컨텍스트별 옵션을 제공할 수 있습니다.

![](assets/segment-builder4.png){width="70%" align="left"}

## 규칙 속성 창

오른쪽에, **규칙 속성** 창에서는 다음 작업을 수행할 수 있습니다.

![](assets/segment-builder5.png){width="70%" align="left"}

* **결과 보기:** 대상이 타겟팅한 수신자 목록을 표시합니다.
* **코드 보기**: sql에서 대상 코드 기반 버전을 표시합니다.
* **고급 속성 표시**: 왼쪽 팔레트에서 전체 속성 목록을 보려면 이 옵션을 선택합니다. 노드, 그룹화, 1-1 링크, 1-N 링크.
* **속성**: 만들어진 대상에 대한 설명을 표시합니다.

## 예제

이 예에서는 1980년 이후에 태어난 Atlanta 또는 Seattle에 거주하는 모든 고객을 타겟팅할 대상을 빌드합니다.

1. 에서 **속성** 팔레트의 탭에서 **생년월일** 필드. 타일을 캔버스에 끌어다 놓습니다.

   ![](assets/segment-builder6.png)

1. 캔버스에서 **후** 연산자를 입력하고 원하는 날짜를 입력합니다.

   ![](assets/segment-builder7.png)

1. 팔레트에서 **구/군/시** 필드를 만들어 첫 번째 규칙 아래의 캔버스에 추가합니다.

   ![](assets/segment-builder8.png)

1. 텍스트 필드에 도시 이름을 입력한 다음 Enter 키를 누릅니다.

   ![](assets/segment-builder9.png)

1. 두 번째 도시 이름에 대해 이 작업을 반복합니다.

   ![](assets/segment-builder10.png)

1. 클릭 **결과 보기** 쿼리와 일치하는 수신자 목록 및 수를 표시합니다. 열을 추가하여 데이터를 시각화하고 확인할 수도 있습니다. 이 예제에서 **구/군/시** 칼럼을 보고 애틀랜타와 시애틀도 보셔야 합니다

   ![](assets/segment-builder11.png)

1. 클릭 **확인**.

대상이 정의되고 이메일에 사용할 준비가 되었습니다.