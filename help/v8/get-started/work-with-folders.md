---
audience: end-user
title: 폴더 작업
description: Adobe Campaign에서 폴더를 관리하는 방법 알아보기
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 25%

---

# 폴더 작업 {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="폴더 속성"
>abstract="폴더 속성"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="폴더 보안"
>abstract="폴더 보안"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="폴더 제한 사항"
>abstract="폴더 제한 사항"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="폴더 일정"
>abstract="폴더 일정"

## 폴더 정보 {#about-folders}

폴더는 Adobe Campaign의 오브젝트로, 구성 요소와 데이터를 구성하는 데 사용할 수 있습니다.

탐색 트리에서 폴더를 만들고, 이름을 바꾸고, 순서를 바꾸고, 이동할 수 있습니다. 자신의 권한에 따라 삭제할 수도 있습니다.

![폴더 조직을 표시하는 폴더 인터페이스](assets/folders.png){zoomable="yes"}

폴더 유형을 설정할 수 있습니다. (예: 게재 폴더) 폴더 아이콘은 유형에 따라 변경됩니다.

## 새 폴더 만들기 {#create-a-folder}

Adobe Campaign Web UI에서 새 폴더를 만들려면 다음 단계를 따릅니다.

1. **[!UICONTROL 탐색기]**&#x200B;에서 새 폴더를 만들 폴더로 이동합니다. **[!UICONTROL ..]** 메뉴에서 **[!UICONTROL 새 폴더 만들기]**&#x200B;를 선택합니다.

![탐색기 메뉴에서 새 폴더 만들기 옵션](assets/folder_create.png){zoomable="yes"}

새 폴더를 만들 때 폴더 유형은 기본적으로 상위 폴더의 유형으로 설정됩니다. 이 예제에서는 폴더가 **[!UICONTROL Deliveries]** 폴더에 만들어집니다.

![게재 폴더에 새 폴더를 만들었습니다](assets/folder_new.png){zoomable="yes"}

1. 필요한 경우 폴더 유형 아이콘을 클릭하여 폴더 유형을 변경하고 아래와 같이 표시된 목록에서 원하는 유형을 선택합니다.

![폴더 유형 선택 인터페이스](assets/folder_type.png){zoomable="yes"}

**[!UICONTROL 확인]** 단추를 클릭하여 폴더 유형을 설정합니다.

특정 형식 없이 폴더를 만들려면 **[!UICONTROL 일반 폴더]** 형식을 선택하십시오.

[Adobe Campaign 콘솔에서 폴더를 만들고 관리](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/config/configuration/folders-and-views)할 수도 있습니다.

## 폴더 재정렬 {#reorder-folders}

필요에 따라 폴더 순서를 변경할 수 있습니다. 이렇게 하려면 아래와 같이 **[!UICONTROL 폴더 순서 바꾸기]**&#x200B;를 클릭하세요.

이 예제에서는 **Deliveries** 폴더에 4개의 하위 폴더가 있습니다.

![폴더 계층 구조를 표시하는 폴더 인터페이스 순서 바꾸기](assets/folder-reorder.png){zoomable="yes"}

**끌어다 놓기** 또는 **위쪽 및 아래쪽 화살표**&#x200B;를 사용하여 폴더 순서를 변경할 수 있습니다.

![폴더 순서 재지정을 위한 끌어서 놓기 기능](assets/folder-draganddrop.png){zoomable="yes"}

## 폴더 삭제 {#delete-a-folder}

>[!CAUTION]
>
>폴더를 삭제하면 해당 폴더에 저장된 모든 데이터도 삭제됩니다.

폴더를 삭제하려면 **[!UICONTROL 탐색기]** 트리에서 폴더를 선택하고 **[!UICONTROL ..]** 메뉴를 클릭합니다. **[!UICONTROL 폴더 삭제]**&#x200B;를 선택합니다.

![탐색기 메뉴의 폴더 삭제 옵션](assets/folder_delete.png){zoomable="yes"}

## 폴더 내 값의 분포 {#distribution-values-folder}

값 분포를 통해 테이블 내 열에 있는 값의 백분율을 이해할 수 있습니다.

폴더의 값 분포를 보려면 아래 설명된 대로 진행하십시오.

예를 들어 게재 중 **채널** 열의 값 분포를 알 수 있습니다.

이 정보를 보려면 **[!UICONTROL 게재]** 폴더로 이동하여 **[!UICONTROL 열 구성]** 아이콘을 클릭하십시오.

**[!UICONTROL 열 구성]** 창에서 분석할 열과 관련된 **[!UICONTROL 정보]** 아이콘을 클릭합니다. 그런 다음 **[!UICONTROL 값 분포]** 버튼을 클릭합니다.

![게재에 대한 값 분배 인터페이스](assets/values_deliveries.png){zoomable="yes"}

**[!UICONTROL 채널]** 열에 값의 백분율이 표시됩니다.

![채널 열의 값 분포 비율](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
>값이 많은 열의 경우 처음 20개의 값만 표시됩니다. **[!UICONTROL 부분 로드]** 알림이 경고합니다.

링크에 대한 값 분포를 볼 수도 있습니다.

아래에 표시된 대로 속성 목록에서 원하는 링크 옆에 있는 **+** 버튼을 클릭합니다. 이렇게 하면 **[!UICONTROL 출력 열]**&#x200B;에 대한 링크가 추가됩니다. 이제 **[!UICONTROL 정보]** 아이콘에 액세스하여 해당 값의 분포를 볼 수 있습니다. **[!UICONTROL 출력 열]**&#x200B;에 링크를 유지하지 않으려면 **[!UICONTROL 취소]** 단추를 클릭하십시오.

![출력 열의 링크 값 분포](assets/values_link.png){zoomable="yes"}

쿼리 모델러의 값 분포를 볼 수도 있습니다. [여기에서 자세히 알아보십시오](../query/build-query.md#distribution-of-values-in-a-query).

### 값 필터링 {#filter-values}

값 분포 창에서 **[!UICONTROL 고급 필터]**&#x200B;를 사용하면 지정된 조건을 기반으로 결과를 필터링할 수 있습니다.

채널별 분포를 보여 주는 위의 게재 목록의 예제에서 **완료됨** 상태의 게재만 표시하도록 필터링할 수 있습니다.

![값 배포에 적용된 고급 필터](assets/values_filter.png){zoomable="yes"}