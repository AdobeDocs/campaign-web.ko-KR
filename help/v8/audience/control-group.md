---
audience: end-user
title: 컨트롤 그룹 설정
description: Campaign 웹 사용자 인터페이스에서 메시지의 컨트롤 그룹을 설정하는 방법을 알아봅니다
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 21%

---

# 컨트롤 그룹 설정 {#control-group}

컨트롤 그룹은 게재에서 제외된 하위 모집단입니다. 대상자의 일부에 메시지를 보내지 않도록 컨트롤 그룹을 정의하고 게재 후 동작을 기본 대상과 비교할 수 있습니다. 이 옵션은 캠페인의 영향을 측정하는 데 도움이 됩니다.

➡️ [비디오에서 이 기능 살펴보기](create-audience.md#video)

## 컨트롤 그룹 활성화 {#add-a-control-group}

컨트롤 그룹을 추가하려면 게재 대상을 정의할 때 옵션을 활성화합니다. 컨트롤 그룹은 주 대상에서 임의로 추출하거나 특정 모집단에서 선택할 수 있습니다. 따라서 컨트롤 그룹을 정의하는 방법에는 두 가지가 있습니다.

* 기본 대상에서 프로필을 몇 개 추출합니다.
* 목록 또는 쿼리에 정의된 기준에 따라 일부 프로필을 제외합니다.

컨트롤 그룹을 정의할 때 두 방법을 결합할 수 있습니다.

게재 준비 단계에서 컨트롤 그룹에 포함된 모든 프로필은 기본 대상에서 제거됩니다. 해당 프로필은 메시지를 받지 않습니다.

>[!CAUTION]
>
>[외부 파일](file-audience.md)에서 대상 모집단을 로드하면 컨트롤 그룹을 사용할 수 없습니다.

게재에 컨트롤 그룹을 추가하려면 게재 만들기 화면의 **대상자** 섹션에서 **[!UICONTROL 컨트롤 그룹 사용]** 토글을 활성화합니다.

![게재 만들기 화면에서 컨트롤 그룹 옵션을 사용하도록 설정](assets/control-group1.png)

## 대상에서 추출 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="추출 모드"
>abstract="컨트롤 그룹은 게재에서 제외된 프로필 세트입니다. 컨트롤 그룹을 정의하기 위해 임의로 또는 대상 모집단에서 정렬, 백분율 또는 고정된 수의 프로필을 추출하도록 선택할 수 있습니다."

### 컨트롤 그룹 만들기 {#build-extract-target}

컨트롤 그룹을 정의하려면 임의로 또는 대상 모집단에서 정렬, 백분율 또는 고정된 수의 프로필을 추출하도록 선택합니다. 추가 모집단을 추가하는 경우 **추출 안 함** 옵션을 선택하고 추가 모집단 [여기 자세히 설명된 대로](#extra-population)을(를) 선택하십시오.

먼저 대상에서 프로필을 추출하는 방법을 정의합니다. 임의로 또는 정렬을 기준으로 합니다.

**컨트롤 그룹** 섹션에서 **추출 모드**&#x200B;를 선택하세요.

* **무작위**: 게재를 준비할 때 Adobe Campaign은 크기 제한으로 설정된 백분율 또는 최대 수에 해당하는 여러 개의 프로필을 임의로 추출합니다.
* **특성별 순위**: 이 옵션은 특정 정렬 순서에서 특정 특성을 기반으로 한 프로필 집합을 제외합니다.

그런 다음 **크기 제한** 섹션을 사용하여 기본 대상에서 추출할 프로필 수를 설정합니다. 원시 숫자(예: 제외할 50개의 프로필) 또는 초기 대상의 백분율(예: 기본 대상의 5%)일 수 있습니다.

### 컨트롤 그룹 샘플 {#control-group-sample}

예를 들어 가장 최신 프로필이 100개인 컨트롤 그룹을 만들려면 다음 단계를 수행합니다.

1. **나이** 필드를 정렬 기준으로 선택합니다. **오름차순** 정렬 옵션을 그대로 둡니다.
1. **만든 날짜** 필드를 추가합니다. **내림차순** 정렬 옵션으로 변경합니다.
1. **크기 제한** 섹션에서 100을 임계값으로 정의합니다.

   ![최신 프로필에 대한 컨트롤 그룹 구성](assets/control-group2.png){zoomable="yes"}

그런 다음 이 100개의 최신 프로필은 주요 대상에서 제외됩니다.

### 컨트롤 그룹 확인 {#check-control-group}

로그를 보고 제외된 프로필을 확인 및 식별합니다. 예를 들어 5개의 프로필을 임의로 제외하는 것을 고려해 보십시오.

![로그에 제외된 프로필의 예](assets/control-group4.png){zoomable="yes"}

게재 준비 후 제외가 적용되는 방법을 검토합니다.

* 게재 대시보드에서 보내기 전에 **제외하려면** KPI를 확인하세요.

  ![제외할 KPI를 표시하는 게재 대시보드](assets/control-group5.png){zoomable="yes"}

* 게재 로그의 로그 탭에 제외 단계가 표시됩니다.

  ![제외 단계를 표시하는 게재 로그](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* **제외 원인** 탭에는 각 유형화 규칙에 대해 제외된 프로필 수가 표시됩니다.

  ![제외로 인해 탭에서 유형화 규칙 제외가 표시됨](assets/control-group7.png){zoomable="yes"}

게재 로그에 대한 자세한 내용은 이 [섹션](../monitor/delivery-logs.md)을 참조하십시오.

## 추가 모집단 추가 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="추가 모집단"
>abstract="컨트롤 그룹은 게재에서 제외된 프로필 세트입니다. 기존 대상자를 선택하거나 쿼리를 정의하여 특정 모집단을 게재 대상자에서 제외할 수 있습니다."

컨트롤 그룹을 정의하는 또 다른 방법은 기존 대상자에서 특정 모집단을 선택하거나 쿼리를 정의하는 것입니다.

**컨트롤 그룹** 정의 화면의 **추가 모집단** 섹션에서 **[!UICONTROL 대상자 선택]** 버튼을 클릭합니다.

![추가 모집단 선택 화면](assets/control-group3.png){zoomable="yes"}

* 기존 대상자를 사용하려면 **대상자 선택**&#x200B;을 클릭합니다. [이 섹션](add-audience.md)에서 자세히 알아보십시오.
* 새 쿼리를 정의하려면 **직접 만들기**&#x200B;를 선택하고 쿼리 모델러를 사용하여 제외 기준을 정의합니다. [이 섹션](../query/query-modeler-overview.md)에서 자세히 알아보십시오.

대상자에 포함되거나 쿼리 결과와 일치하는 프로필은 게재 대상에서 **제외**&#x200B;됩니다. 메시지를 받지 않습니다.

## 결과 비교 {#control-group-results}

게재가 전송되면 전송 로그를 추출하여 커뮤니케이션을 받지 않은 프로필과 유효 대상 간의 동작을 비교합니다. 게재 로그를 사용하여 새 타깃팅을 만듭니다.

대상에서 제거된 프로필을 보려면 **게재 로그**&#x200B;를 확인하세요. 자세한 내용은 [이 섹션](#check-control-group)을 참조하세요.