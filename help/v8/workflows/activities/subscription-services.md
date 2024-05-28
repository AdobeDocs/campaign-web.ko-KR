---
audience: end-user
title: 구독 서비스 활동 사용
description: 구독 서비스 워크플로우 활동을 사용하는 방법 알아보기
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 9cd2d3c7ac4c0ff3c9939cd43606400011fce739
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 17%

---

# 구독 서비스 {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="구독 서비스 활동"
>abstract="구독 서비스 활동을 통해 한 번의 작업으로 서비스에서 여러 프로필을 구독하거나 구독 취소할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="구독 서비스 일반 매개변수"
>abstract="원하는 서비스를 선택하고 수행할 작업(구독 또는 구독 취소)을 선택합니다. **확인 메시지 보내기** 옵션을 토글하여 선택한 서비스에 구독하거나 또는 구독 취소되었음을 모집단에 알립니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="아웃바운드 전환 생성"
>abstract="**아웃바운드 전환 생성** 옵션을 토글하여 활동 뒤에 전환을 추가합니다."

다음 **구독 서비스** 활동은 입니다. **데이터 관리** 활동. 전환에 지정된 모집단에 대한 정보 서비스 구독을 만들거나 삭제할 수 있습니다.

## 구독 서비스 활동 구성 {#subscription-services-configuration}

다음 단계에 따라 **구독 서비스** 활동:

1. 추가 **구독 서비스** 활동을 워크플로우에 추가합니다. 프로필을 타겟팅하거나 식별된 데이터가 있는 파일을 가져온 후 이 활동을 사용할 수 있습니다.

1. 다음 옵션 중 하나를 사용하여 구독을 관리할 서비스를 선택합니다.

   * **[!UICONTROL 특정 서비스 선택]**: 다음을 사용하여 서비스를 수동으로 선택합니다 **[!UICONTROL 서비스]** 필드.

   * **[!UICONTROL 인바운드 전환에서]**: 인바운드 전환에 지정된 서비스를 사용합니다. 예를 들어 각 행에 대해 관리할 서비스를 지정하는 파일을 가져올 수 있습니다. 그런 다음 각 프로필에 대해 작업을 수행할 서비스가 동적으로 선택됩니다.

   ![](../assets/workflow-subscription-service.png)

1. 수행할 작업을 선택합니다. **구독** 또는 **구독 취소**.

   서비스가 인바운드 전환에서 정의된 경우 이 작업을 검색하는 방법을 선택할 수 있습니다.

   * **특정 작업 유형 선택**: 수행할 작업을 수동으로 선택합니다(**구독** 또는 **구독 취소**)

   * **인바운드 전환 경로에서 작업 유형 선택**: 각 레코드에 대해 수행할 작업을 지정하는 인바운드 데이터의 열을 선택합니다. 예를 들어 &quot;작업&quot; 열의 각 행에 대해 수행할 작업을 지정하는 파일을 가져올 수 있습니다.

     >[!NOTE]
     >
     >여기에서는 부울 또는 정수 필드만 선택할 수 있습니다. 수행할 작업이 포함된 데이터가 이 형식과 일치하는지 확인하십시오. 예를 들어 파일 로드 활동에서 데이터를 로드하는 경우 의 작업이 포함된 열의 형식을 올바르게 설정했는지 확인합니다. **[!UICONTROL 파일 로드]** 활동. 예는에 나와 있습니다. [이 섹션](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. 수신자에게 선택한 서비스에 대해 구독 또는 구독 취소를 알리려면 **[!UICONTROL 확인 메시지 보내기]** 옵션입니다. 이 알림의 콘텐츠는 정보 서비스와 연결된 게재 템플릿에 정의됩니다.

1. 인바운드 전환의 데이터를 사용하는 경우 **[!UICONTROL 추가 정보]** 각 레코드에 대한 구독의 데이터와 출처를 지정할 수 있는 섹션이 표시됩니다. 이 섹션을 비워 둘 수 있습니다. 이 경우 워크플로우를 실행할 때 날짜 또는 출처가 설정되지 않습니다.

   * 인바운드 데이터에 프로필의 서비스 구독 날짜를 표시하는 열이 포함되어 있는 경우 **[!UICONTROL 날짜]** 필드.

   * 다음에서 **[!UICONTROL 원본 경로]** 필드에서 구독의 출처를 정의합니다. 다음을 확인하여 인바운드 데이터의 필드 중 하나 또는 선택한 상수 값으로 설정할 수 있습니다. **[!UICONTROL 상수를 원점으로 설정]** 옵션을 선택합니다.

   ![](../assets/workflow-subscription-service-additional.png)

1. 활동 뒤에 아웃바운드 전환을 추가하려면 **[!UICONTROL 아웃바운드 전환 생성]** 옵션입니다.

## 예제 {#example}

### 특정 서비스에 대상자 가입 {#uc1}

아래의 이 워크플로우는 대상자를 기존 서비스에 구독하는 방법을 보여 줍니다.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL 대상자 작성]** 활동은 기존 대상자를 타깃팅합니다.

* A **[!UICONTROL 구독 서비스]** 활동을 통해 프로필을 구독해야 하는 서비스를 선택할 수 있습니다.

<!--
### Updating multiple subscription statuses from a file {#uc2}

The workflow below shows how to import a file containing profiles and update their subscription to several services specified in the file.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Load file]** activity loads a CSV file containing the data and defines the structure of the imported columns. The "service" and "operation" columns specify the service to update and the operation to perform (subscription or unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  As you may have noticed, the operation is specified in the file as "sub" or "unsub". The system expects a **Boolean** or **Integer** value to recognize the operation to perform: "0" to unsubscribe and "1" to subscribe. To match this requirement, a remapping of values must be performed in the detail of the "operation" column in the sample file configuration screen.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  If your file already uses "0" and "1" to identify the operation, you don't need to remap those values. Only make sure that the column is processed as a **Boolean** or **Integer** in the sample file columns.

* A **[!UICONTROL Reconciliation]** activity identifies the data from the file as belonging to the profile dimension of the Adobe Campaign database. The **email** field of the file is matched to the **email** field of the profile resource.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL Enrichment]** activity creates a link to the "Services (nms)" table and creates a simple join between the "service" column of the uploaded file, and the services "internal name" field in the database.

    ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplication]** based on the **email** field identifies duplicates. It is important to eliminate duplicates since the subscription to a service will fail for all data in case of duplicates.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)
  
* A **[!UICONTROL Subscription Services]** identifies the services to update as coming from the transition, through the link created in the **[!UICONTROL Reconciliation]** activity.

  The **[!UICONTROL Operation type]** is identified as coming from the **operation** field of the file. Only Boolean or Integer fields can be selected here. If the column of your file that contains the operation to perform does not appear in the list, make sure that you have correctly set your column format in the **[!UICONTROL Load file]** activity, as explained earlier in this example.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)-->
