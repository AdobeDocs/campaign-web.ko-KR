---
audience: end-user
title: 데이터 소스 변경 워크플로우 활동 사용
description: 데이터 소스 변경 워크플로우 활동을 사용하는 방법을 알아봅니다
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 21%

---

# 데이터 소스 변경 {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="데이터 소스 변경"
>abstract="새로운 데이터 소스 변경 워크플로우 타깃팅 활동을 사용하여 워크플로우의 작업 테이블에서 사용되는 데이터 소스를 변경합니다. 이 활동을 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상할 수 있어 유연성이 향상됩니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="릴리스 정보 참조"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="데이터 소스 변경"
>abstract="**데이터 소스 변경** 활동을 사용하면 워크플로의 작업 테이블에 대해 다른 데이터 소스를 선택할 수 있습니다."

다음 **데이터 소스 변경** 활동은 입니다. **타겟팅** 활동. 이 활동을 사용하면 워크플로우의 작업 테이블에서 사용되는 데이터 소스를 변경할 수 있습니다. 이를 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상시킬 수 있으므로 보다 유연하게 작업할 수 있습니다.

워크플로우에서 전환을 통해 한 활동에서 다른 활동으로 전송된 데이터는 임시로 저장됩니다 **작업 테이블**. 기본적으로 작업 테이블은 처리된 데이터의 소스와 동일한 데이터베이스에 생성됩니다. 예를 들어 클라우드 데이터베이스에 저장된 &quot;프로필&quot; 테이블을 쿼리할 때 동일한 클라우드 데이터베이스에 작업 테이블이 만들어집니다.

경우에 따라 현재 데이터베이스에서 데이터를 사용할 수 없거나 단일 작업을 수행하기에 충분히 효율적이지 않습니다. 따라서 워크플로우가 를 추가하여 다른 데이터베이스를 사용하도록 해야 할 수 있습니다 **[!UICONTROL 데이터 소스 변경]** 활동.

Campaign 아키텍처에 대한 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## 데이터 소스 변경 활동 구성 {#configure}

다음 단계에 따라 **차원 변경** 활동:

![](../assets/workflow-change-data-source-add.png)

1. 추가 **데이터 소스 변경** 활동을 워크플로우에 추가합니다.

1. 작업 테이블을 이동할 데이터 소스를 정의합니다.

   * **[!UICONTROL 기본 캠페인 데이터베이스(PostgreSQL)]**: 기본 Campaign 로컬 데이터베이스 사용
   * **[!UICONTROL FDA 외부 계정]**: 페더레이션 데이터 액세스 기능을 통해 Adobe Campaign에 연결된 외부 클라우드 데이터베이스를 사용합니다.

     >[!AVAILABILITY]
     >
     >Campaign 구성 및 외부 시스템에 대한 연결은 고급 사용자로 제한되며 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=ko){target="_blank"}

1. 새 데이터 소스를 사용하여 원하는 작업을 수행하도록 워크플로우를 구성합니다.

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
