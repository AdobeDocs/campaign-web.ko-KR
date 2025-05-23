---
audience: end-user
title: 속성을 선택하여 즐겨찾기에 추가
description: 속성을 사용하는 방법과 자주 사용하는 속성 및 최근 사용한 속성에 간편하게 액세스 하는 방법을 알아봅니다.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: 6ed904273453ad355c615d330c234462cf3985e8
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# 속성을 선택하여 즐겨찾기에 추가 {#folders}

Campaign Web 사용자 인터페이스를 사용하면 수행하는 액션에 따라 다양한 위치에서 데이터베이스에서 속성을 선택할 수 있습니다. 예를 들어 다이렉트 메일(DM) 게재나 추출할 파일에 대한 출력 열을 정의할 때 속성을 선택할 수 있습니다. 마찬가지로 쿼리 모델러를 사용하여 규칙, 필터를 만들거나 대상자를 작성할 때에도 속성을 선택할 수 있습니다.

![데이터베이스 인터페이스에서 속성을 선택하고 속성 옵션을 표시합니다.](assets/attributes-list.png)

자주 사용하는 속성을 빠르게 재사용하려면 즐겨찾기에 추가합니다. 이렇게 하면 향후 작업에 간편하게 액세스할 수 있습니다. 즐겨찾기 외에도 가장 최근에 선택한 속성을 조회하고 사용할 수 있습니다.

이 인터페이스는 테이블 내에 있는 속성 값의 분포를 시각화하는 데 사용할 수 있는 값 분포 도구도 제공합니다. 이 도구를 사용하면 값의 범위와 빈도를 식별하고 쿼리나 표현식을 만들 때 데이터 일관성을 유지할 수 있습니다.

## 즐겨찾기 및 최근 속성 {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="즐겨찾기 및 최근 항목"
>abstract="속성 선택기의 **[!UICONTROL 즐겨찾기 및 최근 항목]** 메뉴는 즐겨찾기에 추가한 속성과 최근에 사용된 속성 목록을 체계적으로 볼 수 있도록 합니다. 즐겨찾기 속성이 먼저 나타나고, 최근에 사용한 속성이 차례로 나타나 필요한 속성을 쉽게 찾을 수 있습니다."

속성 선택기의 **[!UICONTROL 즐겨찾기 및 최근 항목]** 메뉴는 즐겨찾기에 추가한 속성과 최근에 사용된 속성 목록을 체계적으로 볼 수 있도록 합니다. 즐겨찾기 속성이 먼저 나타나고, 최근에 사용한 속성이 차례로 나타나 필요한 속성을 쉽게 찾을 수 있습니다.

![즐겨찾기 및 최근 속성 메뉴에는 즐겨찾기 및 최근에 사용된 속성이 표시됩니다.](assets/attributes-favorite.png)

즐겨찾기에 속성을 추가하려면 확장 버튼을 클릭하고 **[!UICONTROL 즐겨찾기에 추가]**&#x200B;를 선택합니다. 그러면 해당 속성이 자동으로 즐겨찾기 목록에 추가됩니다. 즐겨찾기에서 속성을 제거하려면 별표 아이콘을 다시 선택합니다.

최대 20개의 속성을 즐겨찾기에 추가할 수 있습니다. 즐겨 찾는 속성과 최근 속성은 조직 내 각 사용자와 연결되어 다양한 기기 간 접근성을 보장하고 여러 디바이스에 걸쳐 원활한 경험을 제공합니다.

## 테이블 내 값의 분포 식별 {#distribution}

속성 옆에 있는 확장 버튼을 클릭하면 표시되는 **값 분포** 버튼을 사용하면 테이블 내에 있는 해당 속성의 값 분포를 분석할 수 있습니다. 이 기능은 사용 가능한 값, 그 개수, 백분율을 이해하는 데 유용합니다. 또한 쿼리를 작성하거나 표현식을 만들 때 대문자 사용이나 맞춤법이 일관되지 않은 것과 같은 문제를 방지하는 데도 도움이 됩니다.

![속성 값의 개수와 백분율을 보여 주는 값 분포 도구 인터페이스입니다.](assets/attributes-distribution-values.png)

값이 많은 속성의 경우 도구에는 처음 20개만 표시됩니다. 이 경우 이러한 제한을 나타내는 **[!UICONTROL 부분 로드]** 알림이 표시됩니다. 고급 필터를 적용하면 표시되는 결과를 구체화하고 특정 값이나 데이터 하위 집합에 초점을 맞출 수 있습니다. 필터 사용에 대한 자세한 지침은 [여기](../get-started/work-with-folders.md#filter-the-values)에서 확인할 수 있습니다.

다양한 컨텍스트에서 값 분포 도구를 사용하는 것에 대한 추가 정보는 다음 섹션을 참조하십시오.

* [폴더 내 값의 분포](../get-started/work-with-folders.md##distribution-values-folder)
* [쿼리 내 값의 분포](../query/build-query.md#distribution-values-query)