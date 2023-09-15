---
audience: end-user
title: 캠페인 시작하기
description: 크로스 채널 캠페인 시작 방법 알아보기
badge: label="Beta"
source-git-commit: 2afec0260566c2393c96063037adbf1902497289
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 93%

---


# 캠페인 액세스 및 관리{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="캠페인 일정"
>abstract="캠페인 일정을 설정하거나 수정합니다."

새 캠페인을 만들거나 기존 캠페인을 관리하려면 왼쪽 탐색 영역에서 **[!UICONTROL 캠페인]** 메뉴를 클릭합니다.

## 캠페인 목록 {#access-campaigns}


캠페인 목록에서 두 개의 탭을 사용할 수 있습니다.

* **찾아보기** 탭에는 기존 캠페인이 모두 나열됩니다. 캠페인을 클릭하여 대시보드를 열거나 **캠페인 만들기** 버튼을 클릭하여 새 캠페인을 만들 수 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오.

* **템플릿 탭**&#x200B;에는 사용 가능한 캠페인 템플릿이 모두 나열됩니다. 캠페인 템플릿은 새 캠페인을 만들 때 재사용할 수 있도록 사전 구성됩니다. 클라이언트 콘솔에서 생성됩니다. [자세히 보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html)

![캠페인 목록](assets/campaign-list.png)

기본적으로 목록의 각 캠페인에는 현재 상태, 생성일, 마지막 수정 시간 등에 대한 정보가 표시됩니다.

목록의 오른쪽 상단에 있는 **사용자 정의 레이아웃에 대한 열 구성** 아이콘을 클릭하여 표시된 열을 사용자 정의할 수 있습니다. 이를 통해 목록에 추가 정보를 추가할 수 있습니다. 또한 목록에서 쉽게 검색할 수 있도록 검색 창과 필터를 사용할 수 있습니다. [자세히 알아보기](../get-started/user-interface.md#list-screens).

예를 들어 캠페인 예약을 필터링할 수 있습니다. 필터 패널을 열고 **시작 - 종료 일자** 섹션 사용:

![캠페인 필터](assets/campaign-filter-on-dates.png)

## 캠페인 대시보드{#campaign-dashboard}


>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="캠페인의 게재 목록"
>abstract="**게재** 탭에는 현재 캠페인에 연결된 게재가 모두 나열됩니다. 편집할 게재 이름을 클릭합니다. 게재 만들기 버튼을 사용하여 이 캠페인에 대한 새 게재를 추가합니다."

캠페인 목록의 **찾아보기** 탭에서 캠페인을 클릭하면 세부 정보가 &#x200B;&#x200B;표시됩니다.

![캠페인 대시보드](assets/campaign-dashboard.png)

캠페인의 상태 및 예약이 화면 상단에 표시됩니다. **캠페인 설정 구성** 아이콘을 사용하여 캠페인 생성 시 정의된 캠페인 속성을 수정할 수 있습니다. 세 가지 버튼을 사용하여 로그와 보고를 확인하고 캠페인을 복제하거나 삭제할 수 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오

사용 가능한 두 가지 탭은 다음과 같습니다.

* **워크플로** 탭에는 캠페인에 연결된 워크플로가 모두 나열됩니다. 이 탭을 통해 캠페인에서 새 워크플로를 만들 수 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오.

* **게재** 탭에는 현재 캠페인에 연결된 게재가 모두 나열됩니다. 캠페인 내에서 새 게재를 만들 수도 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오.

## 캠페인 복제 및 삭제

캠페인을 복제하거나 삭제할 수 있습니다.

* 캠페인 목록에서 줄임표 버튼을 클릭한 다음 **복제** 또는 **삭제**&#x200B;를 선택합니다.
* 캠페인 자체에서 **자세히** 버튼을 클릭한 다음 **복제** 또는 **삭제**&#x200B;를 선택합니다.

>[!NOTE]
>
>**게재** 탭에는 캠페인에 연결된 게재가 모두 표시됩니다. 그러나 워크플로에서 생성된 게재는 여기에서 삭제할 수 없습니다. 워크플로 컨텍스트에서 생성된 게재를 삭제하려면 워크플로에서 게재 활동을 삭제해야 합니다. [자세히 알아보기](../msg/gs-messages.md#delivery-delete)
