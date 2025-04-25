---
audience: end-user
title: 조정 워크플로우 활동 사용
description: 조정 워크플로우 활동을 사용하는 방법을 알아봅니다
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 40%

---

# 조정 {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="조정 활동"
>abstract="**조정** 활동은 Adobe Campaign 데이터베이스의 데이터 간 링크와 작업 테이블의 데이터를 정의하는 **타기팅** 활동입니다. 예를 들어 **조정** 활동을 **파일 로드** 활동 뒤에 놓아 비표준 데이터를 데이터베이스로 가져옵니다. 이 경우 **조정** 활동은 Adobe Campaign 데이터베이스의 데이터와 외부 테이블에 있는 데이터 간의 링크를 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="조정 필드 선택"
>abstract="조정 필드 선택"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="조정 생성 조건"
>abstract="조정 생성 조건"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="조정 생성 여집합"
>abstract="조정 생성 여집합"

**조정** 활동은 외부 파일에서 로드한 데이터와 같이 Adobe Campaign 데이터베이스의 데이터와 작업 테이블의 데이터 간의 연결을 정의하는 **타깃팅** 활동입니다.

예를 들어 **조정** 활동을 **파일 로드** 활동 뒤에 놓아 비표준 데이터를 데이터베이스로 가져옵니다. 이 경우 **조정** 활동은 Adobe Campaign 데이터베이스의 데이터와 작업 테이블의 데이터 간의 연결을 정의합니다.

## 모범 사례 {#reconciliation-best-practices}

**데이터 보강** 활동이 워크플로우에서 처리할 추가 데이터를 정의하는 동안(예: 여러 세트의 데이터를 결합하거나 임시 리소스에 대한 링크를 만드는 경우) **조정** 활동은 미확인 데이터를 기존 리소스에 연결합니다.

>[!NOTE]
>조정 작업을 수행하려면 연결된 차원의 데이터가 데이터베이스에 이미 있어야 합니다. 예를 들어 어떤 제품을, 어떤 시간에, 어떤 고객별로 구매했는지 보여 주는 구매 파일을 가져오는 경우, 데이터베이스와 클라이언트가 이미 존재해야 합니다.

## 조정 활동 구성 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="타기팅 차원"
>abstract="새로운 타기팅 차원을 선택합니다. 차원은 대상 모집단(수신자, 앱 구독자, 운영자, 구독자 등)을 정의합니다. 기본적으로 현재 타기팅 차원이 선택됩니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="조정 규칙"
>abstract="중복 제거를 위한 조정 규칙을 선택합니다. 속성을 사용하려면 **단순 속성** 옵션을 선택하고 소스 및 대상 필드를 선택합니다. 쿼리 모델러를 사용하여 자체 조정 조건을 만들려면 **고급 조정 조건** 옵션을 선택합니다."
>additional-url="https://experienceleague.adobe.com/ko/docs/campaign-web/v8/query-database/query-modeler-overview" text="쿼리 모델러로 작업"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="타기팅 차원 선택"
>abstract="조정할 인바운드 데이터의 타기팅 차원을 선택합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?#targeting-dimensions" text="타기팅 차원"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="조정되지 않은 데이터 유지"
>abstract="기본적으로 조정되지 않은 데이터는 아웃바운드 전환에 보관되며, 나중에 작업 테이블에서 사용할 수 있습니다. 조정되지 않은 데이터를 제거하려면 **조정되지 않은 데이터 유지** 옵션을 비활성화합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="조정 속성"
>abstract="데이터 조정에 사용할 속성을 선택하고 확인을 클릭합니다."

**조정** 활동을 구성하려면 다음 단계를 따르십시오.

1. 워크플로우에 **조정** 활동을 추가합니다. 이 활동은 타겟팅 차원이 Adobe Campaign에서 바로 제공되지 않는 모집단을 포함하는 전환을 따라야 합니다.

1. 새로운 타기팅 차원을 선택합니다. 차원은 대상 모집단(수신자, 앱 구독자, 운영자, 구독자 등)을 정의합니다. [타겟팅 차원에 대해 자세히 알아보세요](../../audience/about-recipients.md#targeting-dimensions).

1. 조정에 사용할 필드를 선택합니다. 조정 기준을 하나 이상 사용할 수 있습니다.

   1. 특성을 사용하여 데이터를 조정하려면 **단순 특성** 옵션을 선택하십시오. **Source** 필드에는 조정할 입력 전환에서 사용할 수 있는 필드가 나열됩니다. **대상** 필드는 선택한 타겟팅 차원의 필드에 해당합니다. 소스와 대상이 같을 때 데이터가 조정됩니다. 예를 들어 **이메일** 필드를 선택하여 이메일 주소를 기반으로 프로필을 중복 제거합니다.

      다른 조정 기준을 추가하려면 **규칙 추가** 단추를 클릭하십시오. 여러 조인 조건이 지정된 경우 데이터가 함께 링크되도록 모든 조인 조건을 확인해야 합니다.

      ![조정 기준 예](../assets/workflow-reconciliation-criteria.png)

   1. 다른 특성을 사용하여 데이터를 조정하려면 **고급 조정 조건** 옵션을 선택하십시오. 그런 다음 쿼리 모델러를 사용하여 자신의 조정 조건을 만들 수 있습니다. [쿼리 모델러를 사용하여 작업하는 방법을 알아봅니다](../../query/query-modeler-overview.md).

1. **필터 만들기** 단추를 사용하여 조정할 데이터를 필터링합니다. 이렇게 하면 쿼리 모델러를 사용하여 사용자 지정 조건을 만들 수 있습니다. [쿼리 모델러를 사용하여 작업하는 방법을 알아봅니다](../../query/query-modeler-overview.md).

기본적으로 조정되지 않은 데이터는 아웃바운드 전환에 보관되며, 나중에 작업 테이블에서 사용할 수 있습니다. 조정되지 않은 데이터를 제거하려면 **조정되지 않은 데이터 유지** 옵션을 비활성화합니다.

## 예제 {#reconciliation-example}

다음 예제에서는 새로운 고객을 포함하는 파일을 가져와 직접 대상자 프로필을 만드는 워크플로를 보여줍니다. 여기에는 다음 활동이 포함됩니다.

워크플로는 다음과 같이 디자인됩니다.

![워크플로 예제](../assets/workflow-reconciliation-sample-1.0.png)

이 템플릿은 다음 활동을 통해 빌드됩니다.

* [파일 로드](load-file.md) 활동에서 외부 도구에서 추출한 프로필 데이터가 포함된 파일을 업로드합니다.

  예제:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* **조정** 활동에서는 조정 기준으로 **전자 메일** 및 **생년월일** 필드를 사용하여 들어오는 데이터를 프로필로 식별합니다.

  ![조정 활동 예](../assets/workflow-reconciliation-sample-1.1.png)

* [대상자 저장](save-audience.md) 활동은 이러한 업데이트를 기반으로 새 대상자를 만듭니다. 특정 대상을 만들거나 업데이트할 필요가 없는 경우 **대상자 저장** 활동을 **종료** 활동으로 바꿀 수도 있습니다. 수신자 프로필은 워크플로우를 실행할 때 업데이트됩니다.

## 호환성 {#reconciliation-compat}

**조정** 활동이 클라이언트 콘솔에 없습니다. 조정 옵션이 활성화된 클라이언트 콘솔에서 만든 모든 **데이터 보강** 활동이 Campaign 웹 사용자 인터페이스에 **조정** 활동으로 표시됩니다.