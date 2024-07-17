---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0c3eb0c20f348442ad28e1e9a801c83d1ab3681f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 6월 릴리스 정보 {#24-6-release}

**릴리스 일자**: 2024년 6월 18~19일

다음은 6월 릴리스 이후 모든 사용자가 이용할 수 있는 기능 및 개선 사항입니다.

### 게재 경고 {#24-6-3}

게재 경고 기능은 사용자 그룹이 게재 실행에 대한 정보가 포함된 알림을 자동으로 수신할 수 있는 경고 관리 시스템입니다. [자세히 보기](../msg/delivery-alerting.md)

### 플랜 및 프로그램 {#24-6-4}

이제 캠페인을 구성하기 위한 플랜과 프로그램을 만들 수 있습니다. 폴더 계층 구조를 정의하면 캠페인을 프로그램으로, 프로그램을 플랜으로 구성할 수 있습니다. [자세히 보기](../administration/plans-programs.md)

### 개선 사항 {#improvements-24-6}

* **보강 활동 조정**: 이제 **보강** 활동을 사용하여 Campaign 데이터베이스 스키마의 데이터를 다른 스키마의 데이터와 조정하거나 파일 로드 활동을 사용하여 업로드한 데이터 등 임시 스키마에서 가져온 데이터와 조정할 수 있습니다. 예를 들면 이 옵션을 사용하여 업로드된 파일에 지정된 프로필 국가를 Campaign 데이터베이스의 전용 테이블에 있는 국가 중 하나와 조정할 수 있습니다. [자세히 보기](../workflows/activities/enrichment.md)

## 5월 릴리스 정보 {#24-5-release}

**릴리스 일자**: 2024년 5월 21일

다음 기능 및 개선 사항은 5월 릴리스 이후 모든 사용자가 이용할 수 있습니다.

### 감사 추적  {#24-5-1}

새로운 **감사 추적** 기능은 Adobe Campaign 인스턴스에 발생한 모든 액션과 이벤트에 대한 자세한 시간순 기록을 실시간으로 제공합니다. 이는 캠페인 데이터의 모든 변경 사항을 추적하고 워크플로 상태, 최근 수정한 개인 또는 인스턴스 내에서 사용자가 수행한 활동과 같은 쿼리를 처리하는 편리한 방법을 제공합니다. [자세히 보기](../reporting/audit-trail.md)

### 사용자 정의 필드 {#24-5-2}

**사용자 정의 필드**&#x200B;는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가되는 추가 속성입니다. Campaign 웹 사용자 인터페이스에서 이러한 사용자 정의 필드는 이제 프로필 또는 테스트 프로필의 세부 정보와 같은 다양한 화면에 표시됩니다. 웹 사용자 인터페이스에서는 사용자 정의 필드를 만들 수 없지만 이제 사용자 정의 필드가 표시되는 방식을 수정할 수 있습니다. [자세히 보기](../administration/custom-fields.md)

### 테이블 간 링크 만들기 {#24-5-3}

이제 **보강** 워크플로 활동에서 다른 테이블과의 링크를 생성할 수 있습니다. 활동 매개변수에서 새로운 **링크 정의** 섹션을 사용하여 작업 테이블 데이터와 Adobe Campaign 데이터베이스 간의 링크를 생성합니다. 예를 들어 수신자의 계정 번호, 국가 및 이메일이 포함된 파일에서 데이터를 로드하는 경우 이제 국가 테이블에 대한 링크를 생성하여 프로필에서 이 정보를 업데이트할 수 있습니다. [자세히 보기](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### 일반 개선 사항 {#improvements-24-5}

* **다이렉트 메일** - 이제 표현식 편집기를 활용하여 다이렉트 메일 추출 파일에 표시할 속성을 선택할 수 있습니다. [자세히 보기](../direct-mail/content-direct-mail.md)

* **폴더 관리** - 이제 상위 폴더와 다른 유형의 하위 폴더를 생성할 수 있습니다. [자세히 보기](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **글로벌화** - 통합된 사용자 경험을 제공하기 위한 지속적인 노력의 일환으로 Adobe Experience Cloud 제품 및 앱에서 사용되는 용어가 통합되었습니다. 이는 오브젝트의 이름과 관련될 때 “레이블”로 변경되는 독일어 용어 “Titel”에 영향을 미칩니다. 변경 사항은 UI와 설명서에 점진적으로 적용됩니다.


## 4월 릴리스 정보 {#april-24-4-release}

**릴리스 일자**: 2024년 5월 2일

### 새로운 기능 {#new-24-4}

다음 기능은 4월 릴리스 이후 모든 사용자가 사용할 수 있습니다.

**새 워크플로 활동**

* **데이터 업데이트** - 이 활동을 통해 데이터베이스의 필드에 대한 대량 업데이트를 수행할 수 있습니다. 데이터 업데이트를 개인화할 수 있는 몇 가지 옵션을 제공합니다. [자세히 보기](../workflows/activities/update-data.md)
* **구독 서비스** - 이 활동을 통해 한 번의 작업으로 여러 프로필을 서비스에 구독하거나 구독 취소할 수 있습니다. [자세히 보기](../workflows/activities/subscription-services.md)
* **파일 추출** - 이 활동을 통해 Adobe Campaign의 데이터를 외부 파일로 다른 시스템으로 내보낼 수 있습니다. [자세히 보기](../workflows/activities/extract-file.md)
* **파일 전송** - 이 활동을 통해 파일을 수신 또는 전송하거나, 파일 존재 여부를 테스트하거나, 서버에서 파일을 나열할 수 있습니다. 사용되는 프로토콜은 서버 간 프로토콜 또는 HTTP 프로토콜일 수 있습니다. [자세히 보기](../workflows/activities/transfer-file.md)
* **테스트** - 이 활동을 통해 지정된 조건에 따라 전환을 활성화할 수 있습니다. [자세히 보기](../workflows/activities/test.md)
* **JavaScript 코드** - 이 활동을 통해 워크플로의 컨텍스트에서 JavaScript 코드 스니펫을 실행할 수 있습니다. [자세히 보기](../workflows/activities/javascript-code.md)
* **외부 신호** - 이 활동을 통해 다른 워크플로 또는 API 호출에서 워크플로 실행을 트리거할 수 있습니다. [자세히 보기](../workflows/activities/external-signal.md)
* **증분 쿼리** - 이 활동을 통해 예약에 따라 데이터베이스를 쿼리할 수 있습니다. 이 활동이 실행될 때마다 이전 실행의 결과가 제외됩니다. 이를 통해 새 요소만 타겟팅할 수 있습니다. [자세히 보기](../workflows/activities/incremental-query.md)

**리치 푸시 알림 템플릿**

이제 Android를 통해 리치 푸시 알림을 보낼 수 있습니다. 리치 푸시 알림은 이미지, 대화형 버튼 또는 기타 리치 미디어 콘텐츠와 같은 멀티미디어 요소를 통합하여 단순한 문자 메시지를 넘어서는 향상된 형태의 모바일 알림입니다. [자세히 보기](../push/rich-push.md)

이 기능은 **제한 공개**(LA)되어 있습니다.


### 제한 공개된 새로운 기능 {#acs-24-4}

>[!AVAILABILITY]
>
>다음 기능은 제한 공개(LA)로 제공됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8로** 마이그레이션하는 고객으로 제한되며 다른 환경에는 배포할 수 없습니다.
>
>[Campaign Standard에서 Campaign v8로의 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ko) 설명서 페이지를 참조하십시오.

* **브랜딩** - Campaign Standard의 마이그레이션된 사용자로서 기술 관리자는 이제 브랜드의 정체성에 영향을 미치는 매개변수를 중앙 집중화하기 위해 하나 이상의 브랜드를 정의할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=ko)

* **Rest API** - Campaign Standard를 마이그레이션한 사용자는 Rest API를 사용하여 Adobe Campaign을 위한 통합을 만들고 사용하는 기술 패널과 Adobe Campaign을 연결하여 고유한 에코시스템을 구축할 수 있습니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=ko)

* **다이내믹 보고** - Campaign Standard를 마이그레이션한 사용자는 완전히 맞춤화가 가능한 실시간 보고서를 제공하는 다이내믹 보고에 액세스하여 마케팅 활동의 영향을 측정할 수 있습니다. 이 기능은 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 기능적 이메일 캠페인 데이터 외에도 성별, 도시, 연령과 같은 프로필 차원별로 인구통계학적 분석을 지원합니다. [자세히 보기](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=ko)

* **랜딩 페이지** - 랜딩 페이지에 대한 다음과 같은 개선 사항은 Campaign Standard에서 전환하는 사용자에게만 제공됩니다.

   * 이제 서비스를 구성할 때 기본 구독/구독 취소 랜딩 페이지를 참조할 수 있습니다. 이메일을 설계할 때 해당 랜딩 페이지에 대한 링크를 정의하면 랜딩 페이지 양식을 제출하는 사용자는 자동으로 이 서비스에 구독하거나 구독 취소됩니다. [자세히 보기](../audience/manage-services.md#create-service)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 익명의 방문자가 랜딩 페이지에 액세스할 수 있습니다. 이 옵션을 선택 취소하면 식별된 사용자만 양식에 액세스하여 제출할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 랜딩 페이지가 제출될 때 추가 내부 데이터를 저장할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 새로운 옵션을 사용하면 여러 서비스에 랜딩 페이지를 사용할 수 있으므로 동적으로 변경할 수 있습니다. 이메일에 링크를 추가할 때 동적 랜딩 페이지를 선택하면 모든 서비스를 선택할 수 있습니다. 특정 서비스가 연결된 랜딩 페이지를 선택하면 해당 서비스가 자동으로 사용됩니다(다른 서비스를 선택할 수 없음). [자세히 보기](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 이제 랜딩 페이지에서 조건부 콘텐츠가 지원됩니다. [자세히 보기](../landing-pages/lp-content.md)

### 일반 개선 사항 {#improvements-24-4}

아래의 개선 사항은 4월 릴리스부터 모든 고객이 이용할 수 있습니다.
<!--**Workflow - Copy/Paste into another tab**: -->

* **파일 로드** 활동은 작업을 실행한 후 샘플 파일을 업로드하고 오류 및 거부를 관리하며 업로드된 파일을 삭제할 수 있는 여러 섹션으로 향상되었습니다. [자세히 보기](../workflows/activities/load-file.md)


* 이제 다른 브라우저 탭에서 한 워크플로의 활동을 다른 워크플로로 **복사/붙여넣기**&#x200B;할 수 있습니다. [자세히 보기](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 이제 모든 워크플로 활동을 통해 **실행 옵션**&#x200B;을 관리할 수 있습니다. 이를 통해 오류 발생 시 활동의 실행 모드 및 동작을 정의할 수 있습니다. [자세히 보기](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* **분할 활동**&#x200B;의 “모집단이 비어 있는 경우 전환을 활성화하지 않음” 옵션을 사용하면 세그먼트 결과가 비어 있는 경우 워크플로를 다음 활동으로 전환할지 여부를 선택할 수 있습니다. [자세히 보기](../workflows/activities/split.md)



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

이제 **분할** 워크플로 활동의 **동일한 테이블에서 모든 하위 집합 생성** 옵션을 사용하여 모든 하위 집합을 단일 출력 전환으로 그룹화할 수 있습니다.

### 쿼리 모델러 {#24-3-query-modeler}

* 이제 이메일 디자이너에서 쿼리 모델러를 사용할 수 있습니다. 이를 통해 조건부 콘텐츠를 생성할 때 조건을 빌드할 수 있습니다.
* 이제 사용자 정의 조건을 생성할 때 날짜 유형 속성에 대해 미리 정의된 값을 사용할 수 있습니다.
* 더 이상 다이어그램의 새 전환에 연산자를 추가할 수 없습니다. 구성 요소를 필터링하여 함께 그룹화하기 전에는 기존 전환에만 추가할 수 있습니다.
