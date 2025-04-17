---
title: 기술 사용자를 Adobe Developer 콘솔로 마이그레이션
description: 사용자 액세스 관리를 Campaign Standard에서 Campaign V8로 마이그레이션하는 방법에 대해 알아봅니다.
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: cc1f89fe5a67898e0905bd2823f73aa8b9424164
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 2%

---

# Campaign Standard에서 Campaign V8로의 사용자 액세스 관리 {#user-management-acs}

Adobe Campaign Standard과 Adobe Campaign V8 모두 사용자가 다양한 사용자/운영자에 대한 권한을 정의하고 관리할 수 있도록 해줍니다. 이러한 권한은 사용자에게 제품의 다양한 기능에 대한 액세스 권한을 부여하는 특정 권한으로 구성됩니다. 그러나 두 제품은 사용자 액세스를 관리하기 위해 서로 다른 접근 방식과 구현을 사용합니다.

다음 개념은 Adobe Campaign Standard 및 Campaign V8에서 사용자 액세스 관리를 수행하는 데 사용됩니다.

| Campaign Standard | Campaign V8 |
|---------|----------|
| 사용자 | 운영자 |
| 역할 | 명명된 권한 |
| 보안 그룹 | 운영자 그룹 |
| 조직 유닛 | 폴더 권한 |

## 보안 그룹에서 운영자 그룹으로 마이그레이션 접근 방식

>[!CAUTION]
>
>이러한 역할/명명된 권한의 기능은 구현에 따라 달라질 수 있으며, 이로 인해 권한 부여 문제(예: 권한 상승 또는 기능 중단)가 발생할 수 있습니다. 적절한 액세스 제어를 위해 전환 후 이러한 매핑을 검토하는 것이 좋습니다. [권한에 대해 자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

아래 표는 Adobe Campaign Standard에서 Campaign V8로 전환할 때 사용자 역할 그룹에 대한 마이그레이션 접근 방식을 간략하게 설명합니다. Campaign Standard에서는 Campaign V8에서 **연산자 그룹**&#x200B;이라고 하는 **보안 그룹**&#x200B;을(를) 사용하여 사용자에게 역할 집합을 할당합니다. 일부 보안 그룹/운영자 그룹은 즉시 사용할 수 있지만, 사용자는 필요한 경우 새 그룹을 만들거나 기존 그룹을 수정할 수 있습니다.

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **용어**  | 보안 그룹 | 운영자 그룹 |

Adobe Campaign Standard과 Campaign V8 모두에서 **보안 그룹** 및 **운영자 그룹**&#x200B;은(는) Admin Console의 제품 프로필에 매핑됩니다. 사용자에게 **보안 그룹** 또는 **운영자 그룹**&#x200B;을(를) 할당하려면 Admin Console에서 해당 **제품 프로필**&#x200B;을 연결할 수 있습니다. 이 연결은 사용자가 로그인할 때 동기화됩니다. [제품 프로필에 대해 자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard 보안 그룹** | **Campaign V8 연산자 그룹** |
|----------|---------|
| 관리자 | 관리자 |
| 게재 감독자 | 관리자 |
| 워크플로 감독자 | 워크플로 감독자  |

## 사용자 역할에서 명명된 권한으로 마이그레이션 접근 방식

>[!CAUTION]
>
>Adobe Campaign Standard에서 Campaign V8로 마이그레이션하는 동안 **데이터 모델** 역할이 있지만 **관리**&#x200B;이(가) 아닌 사용자는 Campaign V8에서 스키마를 만들려면 관리 권한이 필요하므로 자동으로 **관리** 액세스 권한을 갖게 됩니다. 이를 방지하려면 마이그레이션 전에 **데이터 모델** 역할을 제거하십시오.

Adobe Campaign Standard에서 용어 **사용자 역할**&#x200B;은(는) Campaign V8에서 **명명된 권한**&#x200B;입니다. 아래 표는 Campaign Standard의 **사용자 역할**&#x200B;에 해당하는 Campaign V8의 **명명된 권한**&#x200B;에 사용되는 용어를 간략하게 설명합니다.

| **Campaign Standard 사용자 역할** | **Campaign V8 명명된 권한** | **설명**  |
|----------|---------|---------|
| 관리 | 관리 | 관리 권한이 있는 사용자는 인스턴스에 대한 전체 액세스 권한을 갖습니다. |
| 데이터 모델  | 관리 | 게시를 실행하고 사용자 지정 리소스를 만들 수 있는 권한. Campaign V8에서 관리자가 사용할 수 있는 스키마 만들기 관련 기능입니다.  |
| 전달성  | 관리  | 이전에 분석된 게재를 승인할 수 있는 권한.  |
| 내보내기 | 내보내기 | 데이터 내보내기 권한.  |
| 파일 액세스  | 파일 액세스  | 이전에 분석된 게재를 승인할 수 있는 권한.  |
| 일반 가져오기  | 가져오기  | 일반 데이터 가져오기에 대한 권한 |
| 게재 준비 | 게재 준비 | 게재 생성, 수정, 준비 및 삭제할 권한.  |
| SQL 스크립트 실행 | SQL 스크립트 실행 | 데이터베이스에서 직접 SQL 명령을 실행할 수 있는 권한. |
| 게재 시작  | 게재 시작  | 이전에 분석된 게재를 승인할 수 있는 권한.  |
| 시스템 명령 실행 | 프로그램 실행 | 서버에서 시스템 명령을 실행할 수 있는 권한. |
| 워크플로 | 워크플로 | 워크플로우 시작, 중지, 일시 중지 등의 실행을 관리할 수 있는 권한. |

## 조직 단위의 마이그레이션 접근 방식

### 주의 사항

직접 또는 간접 상위로 **모두(모두)**&#x200B;이(가) 없는 Adobe Campaign Standard의 조직 단위는 Campaign V8로 마이그레이션되지 않습니다.

여러 보안 그룹의 사용자에게는 최상위 보안 그룹의 조직 단위가 할당됩니다. 여러 그룹에 병렬 최상위 단위가 있는 경우, 시스템은 Campaign Standard에서 사용자에 대한 조직 단위를 선택하고 사용자는 시스템에서 선택한 조직 단위와 그 하위 단위에만 액세스할 수 있습니다. 마이그레이션 후 Campaign v8에서 사용자는 **할당된 모든 조직 단위와 하위 항목**&#x200B;에 액세스할 수 있으므로 권한이 높아질 수 있습니다. 이를 방지하려면 병렬 조직 단위를 사용하는 보안 그룹에 사용자를 할당하지 마십시오. <!--Know more about parallel organizational unit assignment here (link to ' Parallel Organizational Unit Assignment' section)-->

### 조직 단위 및 폴더 관리

Adobe Campaign Standard에서 **조직 단위**&#x200B;은(는) 유사한 액세스 제어를 유지하기 위해 Campaign V8의 기존 **폴더** 계층 구조 모델에 매핑됩니다. [폴더 관리에 대해 자세히 알아보기](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **용어**  | 조직 유닛 | 폴더 |

## 프로그램에서 마이그레이션 접근 방식

Campaign V8에서 **프로그램**&#x200B;은(는) **폴더**(으)로 표시됩니다. Campaign V8을 사용하면 폴더를 만들고 폴더 액세스를 제한할 수 있습니다.

**그룹** 및 **명명된 권한**&#x200B;을(를) 사용하면 **연산자**&#x200B;에게 탐색 계층 구조 내의 특정 **폴더**&#x200B;에 대한 액세스 권한을 부여하고 읽기, 쓰기 및 삭제 권한을 할당할 수 있습니다. [폴더 관리에 대해 자세히 알아보기](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

**Program**&#x200B;은(는) Campaign V8에서 **Folder**(으)로 처리되므로 다른 폴더와 동일한 방식으로 액세스 권한을 관리할 수 있습니다. 마이그레이션 후 Campaign Standard 관리자는 다음 단계를 수행할 수 있습니다.

1. 탐색기에서 폴더를 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 속성...]**&#x200B;을 선택합니다.

1. **[!UICONTROL 보안]** 탭으로 이동합니다.

1. 원하는 액세스 모델에 따라 운영자 그룹 권한을 수정합니다. 

## REST API에 액세스하기 위한 제품 프로필 매핑 

Campaign V8의 실행 인스턴스에서 트랜잭션 API에 액세스하려면 **관리자** 및 **메시지 센터** 제품 프로필 외에 새 **제품 프로필**&#x200B;이 필요합니다. 이 새 **제품 프로필**&#x200B;은(는) Campaign Standard의 기존 또는 미리 만들어진 기술 계정에 추가됩니다.

마이그레이션 후 Campaign Standard 사용자는 **제품 프로필 매핑**&#x200B;을 검토하고 **기술 계정**&#x200B;을 **관리자** 제품 프로필에 연결하지 않으려면 적절한 **제품 프로필**&#x200B;을 할당해야 합니다. 향후 통합을 위해 이전 Campaign Standard **테넌트 ID** 대신 **REST URL**&#x200B;의 Campaign V8 **테넌트 ID**&#x200B;을(를) 사용하는 것이 좋습니다.

## Campaign Standard 운영자를 위한 기본 제공 Campaign 리소스에 대한 액세스 마이그레이션

Campaign Standard에서 마이그레이션된 연산자는 Campaign V8의 특정 기본 제공 리소스에 대한 읽기 액세스 권한을 갖게 됩니다.

## 마이그레이션되지 않은 보안 그룹 및 역할 {#non-migrated-groups-roles}

다음은 전환되지 않은 Campaign Standard 역할 목록입니다.

* 기본 릴레이 계정 

* 메시지 센터 푸시 

다음은 전환되지 않은 Campaign Standard 보안 그룹 매핑 목록입니다.

* 메시지 센터 에이전트

* 메시지 센터 푸시 에이전트

* Adobe Experience Manager 애플리케이션 관리자

* 릴레이 계정

Adobe Campaign Standard에서 생성되고 사용자에게 할당된 사용자 정의 역할은 Campaign V8로 마이그레이션되지 않습니다.
