---
audience: end-user
title: 조정 워크플로우 활동 사용
description: 조정 워크플로우 활동을 사용하는 방법을 알아봅니다
badge: label="제한 공개"
source-git-commit: 89372e4a6c60937c646de59eb1a65b86fa1b2528
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 15%

---

# 조정 {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="조정 활동"
>abstract="다음 **조정** 활동은 입니다. **타겟팅** 활동. 식별되지 않은 데이터를 기존 리소스에 연결할 수 있습니다. 예를 들어 **조정** 활동은 다음 뒤에 배치할 수 있습니다. **대상자 로드** 비표준 데이터를 데이터베이스로 가져오는 활동. 이 경우 **조정** 활동을 사용하면 Adobe Campaign 데이터베이스의 데이터와 작업 테이블의 데이터 간의 링크를 정의할 수 있습니다."


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
>title="조정 보조 항목 생성"
>abstract="조정 보조 항목 생성"



다음 **조정** 활동은 입니다. **타겟팅** 활동. 식별되지 않은 데이터를 기존 리소스에 연결할 수 있습니다. 예를 들어 **조정** 활동은 다음 뒤에 배치할 수 있습니다. **대상자 로드** 비표준 데이터를 데이터베이스로 가져오는 활동. 이 경우 **조정** 활동을 사용하면 Adobe Campaign 데이터베이스의 데이터와 작업 테이블의 데이터 간의 링크를 정의할 수 있습니다.


## 모범 사례 {#reconciliation-best-practices}

동안 **데이터 보강** 활동을 통해 워크플로우에서 처리할 추가 데이터를 정의할 수 있습니다( **데이터 보강** 활동은 여러 세트에서 가져온 데이터를 결합하거나 임시 리소스에 대한 링크를 만듭니다. **조정** 활동을 사용하면 미식별 데이터를 기존 리소스에 연결할 수 있습니다.

>[!NOTE]
>조정 작업은 연결된 차원의 데이터가 이미 데이터베이스에 있음을 의미합니다.  예를 들어 어떤 제품을, 어떤 시간에, 어떤 고객이 구매했는지 등을 표시하는 구매 파일을 가져올 경우, 데이터베이스에는 이미 고객과 제품이 존재할 것입니다.
>

## 조정 활동 구성 {#reconciliation-configuration}


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="타겟팅 차원"
>abstract="새 타겟팅 차원을 선택합니다. 차원을 사용하면 타겟팅된 모집단(수신자, 앱 구독자, 연산자, 구독자 등)을 정의할 수 있습니다. 기본적으로 현재 타겟팅 차원이 선택되어 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="조정 규칙"
>abstract="중복 제거에 사용할 조정 필드를 선택합니다. 하나 이상의 조정 기준을 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="타겟팅 차원 선택"
>abstract="조정할 인바운드 데이터의 타겟팅 차원을 선택합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/about-recipients.html?lang=en#targeting-dimensions" text="타겟팅 차원"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="조정되지 않은 데이터 유지"
>abstract="조정되지 않은 데이터는 기본적으로 아웃바운드 전환에 유지되고 나중에 사용할 수 있도록 작업 테이블에서 사용할 수 있습니다. 조정되지 않은 데이터를 제거하려면 **조정되지 않은 데이터 유지** 옵션을 선택합니다."


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="조정 속성"
>abstract="데이터 조정에 사용할 속성을 선택하고 확인을 누릅니다."

다음 단계에 따라 **조정** 활동:

1. 드래그 앤 드롭 **조정** 활동을 워크플로우에 추가합니다. 이 활동은 타겟팅 차원이 Adobe Campaign에서 바로 제공되지 않는 모집단이 포함된 전환 후에 추가해야 합니다.

1. 새 타겟팅 차원을 선택합니다. 차원을 사용하면 타겟팅된 모집단(수신자, 앱 구독자, 연산자, 구독자 등)을 정의할 수 있습니다. 에서 차원 타깃팅에 대해 자세히 알아보기 [이 페이지](../../audience/about-recipients.md#targeting-dimensions).

1. 중복 제거에 사용할 조정 필드를 선택합니다. 하나 이상의 조정 기준을 사용할 수 있습니다.

   1. 속성을 사용하여 데이터를 조정하려면 **단순 속성** 옵션을 선택합니다. 예를 들어 **이메일** 이메일 주소를 기반으로 프로필을 중복 제거하는 필드입니다. 다음 **소스** 필드는 조정할 입력 전환에서 사용할 수 있는 필드를 나열합니다. 다음 **대상** 필드는 선택한 타겟팅 차원의 필드에 해당합니다. 소스와 대상이 같을 때 데이터가 조정됩니다.

      다른 조정 기준을 추가하려면 **규칙 추가** 단추를 클릭합니다. 여러 조인 조건이 지정된 경우 데이터를 함께 연결할 수 있도록 모두 를 확인해야 합니다.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. 다른 속성을 사용하여 데이터를 조정하려면 **고급 조정 조건** 옵션을 선택합니다. 그런 다음 쿼리 모델러를 사용하여 자신의 조정 조건을 만들 수 있습니다. 에서 쿼리 모델러를 사용하는 방법 알아보기 [이 섹션](../../query/query-modeler-overview.md).

1. 를 사용하여 조정할 데이터를 필터링할 수 있습니다. **필터 만들기** 단추를 클릭합니다. 이렇게 하면 를 사용하여 사용자 지정 조건을 만들 수 있습니다. [쿼리 모델러](../../query/query-modeler-overview.md).

기본적으로, 조정되지 않은 데이터는 아웃바운드 전환에 유지되고 나중에 사용할 수 있도록 작업 테이블에서 사용할 수 있습니다. 조정되지 않은 데이터를 제거하려면 **조정되지 않은 데이터 유지** 옵션을 선택합니다.

## 예제 {#reconciliation-example}

다음 예제에서는 새로운 고객을 포함하는 파일을 가져와 직접 대상자 프로필을 만드는 워크플로우를 보여줍니다. 워크플로우는 다음 활동으로 구성됩니다.

워크플로우는 다음과 같이 디자인됩니다.

![](../assets/workflow-reconciliation-sample-1.0.png)


이 템플릿은 다음 활동을 통해 빌드됩니다.

* [파일 로드](load-file.md) 활동으로 외부 도구에서 추출한 프로필 데이터가 포함된 파일을 업로드합니다.

  예제:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **조정** 활동은 다음을 사용하여 들어오는 데이터를 프로필로 식별합니다 **이메일** 조정 기준으로 필드.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [대상자 저장](save-audience.md) 활동은 이러한 업데이트를 기반으로 새 대상자를 만듭니다. 다음을 바꿀 수도 있습니다. **대상자 저장** 의 활동 **종료** 특정 대상자를 만들거나 업데이트할 필요가 없는 경우 활동. 수신자 프로필은 워크플로우를 실행할 때 업데이트됩니다.


## 호환성 {#reconciliation-compat}

다음 **조정** 활동이 클라이언트 콘솔에 없습니다. 모두 **강화** 조정 옵션이 활성화된 클라이언트 콘솔에서 생성된 활동은 다음과 같이 표시됩니다. **조정** Campaign 웹 UI의 활동.
