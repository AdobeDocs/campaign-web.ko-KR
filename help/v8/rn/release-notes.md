---
title: 최신 릴리스 정보
description: Campaign Web 사용자 인터페이스에서 제공하는 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f6a1ebcb5a77798f738e2a4ac0b45454d941d7c7
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 25%

---

# 릴리스 정보 {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 4월 릴리스 정보 {#april-24-4-release}

**릴리스 날짜**: 2024년 5월 2일

### 새로운 기능 {#new-24-4}

다음 기능은 4월 릴리스부터 모든 사용자가 사용할 수 있습니다.

**새 워크플로우 활동**

* **데이터 업데이트** - 이 활동을 사용하여 데이터베이스의 필드에 대한 대량 업데이트를 수행합니다. 몇 가지 옵션을 사용하여 데이터 업데이트를 개인화할 수 있습니다. [자세히 보기](../workflows/activities/update-data.md)
* **구독 서비스** - 이 활동을 사용하여 한 번의 작업으로 여러 프로필을 서비스에 가입하거나 서비스에서 가입할 수 있습니다. [자세히 보기](../workflows/activities/subscription-services.md)
* **파일 추출** - 이 활동을 사용하여 Adobe Campaign에서 다른 시스템으로 데이터를 외부 파일로 내보냅니다. [자세히 보기](../workflows/activities/extract-file.md)
* **파일 전송** - 이 활동을 사용하여 파일을 받거나 보내고, 파일의 존재를 테스트하거나, 서버에 있는 파일을 나열합니다. 사용되는 프로토콜은 서버 간 프로토콜 또는 HTTP 프로토콜일 수 있습니다. [자세히 보기](../workflows/activities/transfer-file.md)
* **테스트** - 이 활동을 사용하여 지정된 조건을 기반으로 전환을 활성화합니다. [자세히 보기](../workflows/activities/test.md)
* **JavaScript 코드** - 이 활동을 사용하여 워크플로우 컨텍스트에서 JavaScript 코드 스니펫을 실행합니다. [자세히 보기](../workflows/activities/javascript-code.md)
* **외부 신호** - 이 활동을 사용하여 다른 워크플로우 또는 API 호출에서 워크플로우 실행을 트리거합니다. [자세히 보기](../workflows/activities/external-signal.md)
* **증분 쿼리** - 이 활동을 사용하여 일정에 따라 데이터베이스를 쿼리합니다. 이 활동이 실행될 때마다 이전 실행의 결과가 제외됩니다. 이를 통해 새 요소만 타겟팅할 수 있습니다. [자세히 보기](../workflows/activities/incremental-query.md)

**리치 푸시 알림 템플릿**

이제 Android를 통해 리치 푸시 알림을 전송할 수 있습니다. 리치 푸시 알림은 이미지, 대화형 버튼 또는 기타 리치 미디어 컨텐츠와 같은 멀티미디어 요소를 통합하여 간단한 텍스트 메시지를 넘어 향상된 형태의 모바일 알림입니다. [자세히 보기](../push/rich-push.md)

이 기능은에 있습니다. **제한된 가용성** (LA)

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### 제한된 가용성의 새로운 기능 {#acs-24-4}

>[!AVAILABILITY]
>
>다음 기능은 LA(Limited Availability)에 있습니다. 고객은 마이그레이션하는 것으로 제한됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8까지**, 및 은 다른 환경에 배포할 수 없습니다.
>
>다음 설명서 페이지를 참조하십시오. [Campaign v8로 Campaign Standard 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **브랜딩** - 이제 기술 관리자는 Campaign Standard을 마이그레이션한 사용자로서 한 개 또는 여러 브랜드를 정의하여 브랜드 이미지에 영향을 주는 매개 변수를 중앙 집중화할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **나머지 API** - Campaign Standard을 마이그레이션한 사용자는 Rest API를 사용하여 Adobe Campaign을 위한 통합을 만들고 사용하는 기술 패널과 Adobe Campaign을 연결하여 고유한 에코시스템을 구축할 수 있습니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **다이내믹 보고** - Campaign Standard을 마이그레이션한 사용자는 완전히 맞춤화가 가능한 실시간 보고서를 제공하는 Dynamic Reporting에 액세스하여 마케팅 활동의 영향을 측정할 수 있습니다. 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 실용적인 이메일 캠페인 데이터 외에도 성별, 도시 및 연령 등의 프로필 차원별 인구 통계 분석을 활성화합니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **랜딩 페이지** - 랜딩 페이지에 대한 다음 개선 사항은 Campaign Standard에서 전환하는 사용자만 사용할 수 있습니다.

   * 이제 서비스를 구성할 때 기본 구독/구독 취소 랜딩 페이지를 참조할 수 있습니다. 이메일을 디자인할 때 해당 랜딩 페이지에 대한 링크를 정의하는 경우, 랜딩 페이지 양식을 제출하는 사용자는 이 서비스에 자동으로 가입되거나 가입이 해지됩니다. [자세히 보기](../audience/manage-services.md#create-service)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하여 익명 방문자가 랜딩 페이지에 액세스할 수 있습니다. 이 옵션의 선택을 취소하면 식별된 사용자만 양식에 액세스하고 양식을 제출할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 랜딩 페이지가 제출될 때 추가 내부 데이터를 저장할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 새 옵션을 사용하면 여러 서비스의 랜딩 페이지를 동적으로 사용할 수 있습니다. 이메일에 링크를 추가할 때 동적 랜딩 페이지를 선택하면 원하는 서비스를 선택할 수 있습니다. 특정 서비스가 연결된 랜딩 페이지를 선택하면 이 서비스가 자동으로 사용됩니다(다른 서비스를 선택할 수 없음). [자세히 보기](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 이제 조건부 콘텐츠가 랜딩 페이지에서 지원됩니다. [자세히 보기](../landing-pages/lp-content.md)

### 일반 개선 사항 {#improvements-24-4}

아래 개선 사항은 4월 릴리스부터 모든 고객이 사용할 수 있습니다.
<!--**Workflow - Copy/Paste into another tab**: -->

* 다음 **파일 로드** 활동이 실행된 후 샘플 파일을 업로드하고, 오류 및 거부를 관리하고, 업로드된 파일을 삭제할 수 있는 몇 개의 섹션으로 활동이 개선되었습니다. [자세히 보기](../workflows/activities/load-file.md)


* 이제 다음을 수행할 수 있습니다. **활동 복사/붙여넣기** 다른 브라우저 탭에서 워크플로우로 이동합니다. [자세히 보기](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 이제 모든 워크플로우 활동을 통해 **실행 옵션**. 이를 통해 오류 발생 시 활동의 실행 모드와 비헤이비어를 정의할 수 있습니다. [자세히 보기](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* 의 &quot;모집단이 비어 있는 경우 전환을 활성화하지 않음&quot; 옵션 **활동 분할** 세그먼트 결과가 비어 있을 때 워크플로우를 다음 활동으로 전환할지 여부를 선택할 수 있습니다. [자세히 보기](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **사용자 정의 필드** 는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가된 추가 속성입니다. 이제 Campaign 웹 사용자 인터페이스에서 이러한 사용자 정의 필드를 프로필 또는 테스트 프로필 세부 정보 등의 다양한 화면에 볼 수 있습니다. 웹 사용자 인터페이스에서 사용자 정의 필드를 만들 수 없지만 이제 표시되는 방식을 수정할 수 있습니다. [자세히 보기](../administration/custom-fields.md)


## 3월 릴리스 정보 {#24-3-release}

>[!AVAILABILITY]
>
>이 버전은 [Campaign (콘솔) v8.6 릴리스](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko)를 시작하는 모든 사용자가 사용할 수 있습니다. [Campaign v8 (콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=ko){target="_blank"}에서 Adobe Campaign 클라이언트 콘솔 릴리스 및 업그레이드에 대해 자세히 알아보십시오.

**릴리스 일자**: 2024년 3월 19~20일

### 다이렉트 메일 채널 {#24-3-dm}

이제 **다이렉트 메일** 채널을 워크플로 및 독립 실행형 게재에 사용할 수 있습니다. 다이렉트 메일은 다이렉트 메일 공급자가 고객에게 메일을 보내는 데 사용하는 추출 파일을 만들고, 개인화하고, 생성하여 해당 공급자와 공유할 수 있는 오프라인 채널입니다.

### 데이터 소스 워크플로 활동 신규 변경 {#24-3-change-data-source}

**데이터 소스 변경** 타겟팅 활동을 사용하면 워크플로의 작업 테이블에서 사용하는 데이터 소스를 변경할 수 있습니다. 이 활동을 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상할 수 있어 유연성이 향상됩니다.

### 분할 워크플로 활동 개선 {#24-3-split}

이제 다음을 사용할 수 있습니다. **동일한 테이블의 모든 하위 집합 생성** 의 옵션 **분할** 워크플로우 활동을 통해 모든 하위 집합을 단일 출력 전환으로 그룹화합니다.

### 쿼리 모델러 {#24-3-query-modeler}

* 이제 이메일 디자이너에서 쿼리 모델러를 사용할 수 있습니다. 조건부 콘텐츠를 만들 때 조건을 작성할 수 있도록 해 줍니다.
* 이제 사용자 지정 조건을 만들 때 날짜 유형 속성에 대해 사전 정의된 값을 사용할 수 있습니다.
* 더 이상 다이어그램의 새 전환에 연산자를 추가할 수 없습니다. 구성 요소를 필터링하여 함께 그룹화하기 전에 기존 전환에만 추가할 수 있습니다.
