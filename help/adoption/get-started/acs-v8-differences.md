---
title: Campaign Standard과 Campaign v8 간의 차이점
description: Campaign Standard에서 Campaign v8로 전환할 때 변경되는 사항 및 세부 정보를 찾을 수 있는 위치를 알아봅니다
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 64a07e65b7e6d933288b10117aae99f48d13a8d8
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 2%
---
# Campaign Standard과 Campaign v8 간의 차이점 {#acs-v8-differences}

대부분의 개념은 Campaign Standard 및 Campaign v8에서도 동일합니다. 이 페이지에서는 전환 후에 영향을 주는 차이점과 각 차이점을 설명하는 페이지에 대한 링크를 수집합니다. [마케터](marketers.md) 및 [관리자 및 개발자](admin-developers.md)용 안내서를 보완합니다.

* 용어 변경에 대해서는 [Campaign Standard과 Campaign v8 간의 주요 차이점](overview.md#experiences)을 참조하십시오.
* 실행 확인 및 전환 후 보고된 문제에 대해서는 [전환 후 확인 및 문제 해결](post-transition-checks.md)을 참조하십시오.
* 클라이언트 콘솔에서만 사용할 수 있는 기능은 [Campaign 웹 및 Campaign 클라이언트 콘솔](../../v8/get-started/capability-matrix.md)을 참조하십시오.

## 채널 및 콘텐츠 {#channels}

메시지를 만들고 보내는 단계는 [마케터용 안내서](marketers.md)에 설명된 대로 두 제품에서 비슷합니다. 아래의 차이점은 채널 가용성, 테스트 게재, 랜딩 페이지 및 DM 워크플로우와 관련이 있습니다.

| 변경 사항 | 자세히 알아보기 |
|---|---|
| Campaign v8에서는 인앱 채널을 사용할 수 없습니다. | [인앱 채널](marketers.md#acs-gs-marketers-in-app) |
| 기존 푸시 워크플로우 및 게재를 전환하려면 Adobe Campaign 전환 관리자에게 문의하십시오. | [푸시 알림](marketers.md#acs-gs-marketers-push) |
| Campaign Standard에서 테스트 프로필을 **트랩**(으)로 표시하여 최종 전송을 받을 수 있습니다. Campaign v8에서 게재의 대상 설정에 **트랩 그룹**&#x200B;을(를) 추가합니다. | [트랩 그룹](../../v8/audience/trap-group.md) |
| Campaign 웹 사용자 인터페이스에서 만든 랜딩 페이지는 숨겨진 입력 필드 또는 사용자 지정 JavaScript을 지원하지 않습니다. | [랜딩 페이지](../../v8/landing-pages/get-started-lp.md) |
| Campaign Standard에서 DM 활동의 아웃바운드 전환은 생성된 파일도 전달합니다. Campaign v8에서는 대상 모집단만 전달합니다. 파일을 서버로 보내려면 **데이터 추출** 활동을 추가한 다음 **파일 전송** 활동을 추가하십시오. | [DM](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## 대상자, 워크플로우 및 게재 {#data-and-workflows}

이러한 차이는 Campaign Standard에서 마이그레이션된 대상 및 워크플로, 반복 게재 및 **파일 전송** 활동의 일부 옵션, 동적 보고 범위에 영향을 줍니다.

| 변경 사항 | 자세히 알아보기 |
|---|---|
| 대상자는 전환 중에 변형됩니다. 예를 들어 쿼리 활동으로 생성된 대상은 사전 정의된 필터가 되고 파일 유형 대상은 차원이 없는 목록 유형 대상이 됩니다. | [대상자 관리](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standard에서 실행된 워크플로의 기록 로그는 마이그레이션되지 않습니다. | [워크플로 만들기](marketers.md#acs-gs-marketers-wf) |
| Campaign Standard에서 반복 이메일의 집계 기간을 선택할 수 있습니다. Campaign v8에서는 이 옵션을 사용할 수 없습니다. | [채널 활동](../../v8/workflows/activities/channels.md) |
| 동적 보고는 이메일 게재, 이메일 게재 캠페인 및 트랜잭션 메시지를 다룹니다. | [보고](marketers.md#acs-gs-marketers-reporting) |

## 액세스 및 보안 {#access}

Campaign Standard 보안 그룹, 역할 및 조직 단위는 전환되는 동안 명명된 권한 및 폴더 권한으로 운영자 그룹에 매핑됩니다. 특히 일부 사용자가 이전보다 더 광범위하거나 더 좁은 권한을 보유하고 있는 경우 아래 사항을 검토하십시오.

| 변경 사항 | 자세히 알아보기 |
|---|---|
| 보안 그룹, 역할 및 조직 단위는 운영자 그룹(권한 및 폴더 권한)에 매핑됩니다. 사용자 정의 역할은 마이그레이션되지 않습니다. | [사용자 액세스 관리](user-management-acs.md) |
| **데이터 모델** 역할이 있지만 **관리** 역할이 없는 사용자는 **관리** 액세스 권한을 갖습니다. | [사용자 액세스 관리](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 병렬 조직 단위를 사용하는 보안 그룹에 할당된 사용자는 Campaign v8에서 더 광범위한 액세스 권한을 가질 수 있습니다. | [병렬 조직 단위 할당](user-management-acs.md#parallel-assignments) |
| 실행 인스턴스에서 트랜잭션 API에 액세스하려면 새 제품 프로필이 필요합니다. | [제품 프로필 매핑](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 개인 정보 보호 요청은 Campaign Standard 환경이 활성 상태를 유지하는 기간 동안 Campaign Standard 및 Campaign v8 모두에 도착할 수 있습니다. | [개인 정보 및 동의](admin-developers.md#privacy-and-consent) |

## API 및 통합 {#apis-and-integrations}

이러한 차이는 REST API를 통해 Campaign을 호출하는 통합 및 다른 Adobe 솔루션 및 도구와의 통합에 영향을 줍니다.

| 변경 사항 | 자세히 알아보기 |
|---|---|
| PKEY 값은 마이그레이션 후 변경됩니다. Campaign 외부에 PKEY를 저장하는 경우 API에서 반환되는 href를 대신 따릅니다. | [키 사용](#key-usage) |
| 표준 시간대 및 `ccpaOptOut`과(와) 같은 일부 마이그레이션된 프로필 필드는 `profileAndServicesExt/profile` API에서만 반환됩니다. | [프로필 시간대](#profile-timezone) |
| Adobe은 Adobe Analytics 및 Audience Manager 구성을 마이그레이션합니다. 트리거 및 Adobe Target 통합을 다시 설정해야 합니다. | [Adobe Campaign 통합 관리](admin-developers.md#acs-gs-integrations) |

## REST API 권장 사항 및 제한 사항 {#rest-api-limitations}

아래 권장 사항 및 제한 사항은 Campaign Standard에서 Campaign v8로 전환할 때 REST API에 적용됩니다.

### 권한 및 보안 {#permissions}

#### 제품 프로필 매핑 {#rest-product-profiles}

Campaign Standard에서는 할당된 제품 프로필과 관계없이 API에 대한 관리자 역할 액세스 권한이 부여되었습니다. Campaign v8에서는 Campaign Standard에서 Campaign v8 제품 프로필로의 매핑이 필요한 다양한 제품 프로필 세트를 도입했습니다.

마이그레이션을 수행하면 기존 또는 미리 만든 기술 계정에 두 개의 제품 프로필이 추가됩니다(트랜잭션 API에 액세스하기 위한 관리자 및 메시지 센터). 제품 프로필 매핑을 검토하고 관리자 제품 프로필을 기술 계정과 매핑하지 않으려는 경우 필요한 제품 프로필을 할당합니다.

#### 테넌트 ID

마이그레이션 후 향후 통합을 위해 이전 Campaign Standard 테넌트 ID를 대체하여 REST URL의 **Campaign v8 테넌트 ID**&#x200B;를 사용하는 것이 좋습니다.

#### 키 사용

PKey 값 관리는 Campaign Standard과 Campaign v8에서 다릅니다. Campaign Standard과 함께 PKeys를 저장하는 경우 이전 API 호출에서 가져온 PKeys 또는 href를 사용하여 구현이 후속 API 호출을 동적으로 형성하는지 확인하십시오.

### 사용 가능한 API {#available-apis}

현재 아래에 나열된 REST API를 사용할 수 있습니다.

* **프로필**
* **서비스 및 구독**
* **사용자 정의 리소스**
* **워크플로**
* **트랜잭션 메시지**

>[!AVAILABILITY]
>
>지금은 **트랜잭션 메시지** REST API를 사용할 수 없습니다.
>
>아래에 나열된 REST API는 더 이상 사용되지 않으며 사용할 수 없습니다.
>* 마케팅 기록
>* 조직 단위
>* 개인 정보 보호 관리

### 필터링 {#rest-filtering}

* REST API 페이로드에서 필터를 사용하려면 Campaign v8에서 편집하고 페이로드에 사용할 이름을 제공해야 합니다. 이렇게 하려면 **[!UICONTROL 매개 변수]** 탭에서 필터의 추가 매개 변수에 액세스하고 **[!UICONTROL REST API의 필터 이름]** 필드에 원하는 이름을 제공합니다.

  ![](assets/api-filtering.png)


* 사용자 지정 필터를 사용하는 데 필요한 &quot;by&quot; 접두사는 더 이상 필요하지 않습니다. 필터 이름은 요청에 있는 그대로 사용해야 합니다.

  예:

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### 삭제된 데이터베이스 필드 {#dropped-fields}

마이그레이션 도중 데이터베이스의 일부 필드가 삭제됩니다. 삭제된 필드를 사용할 때 REST API는 빈 값을 반환합니다. 앞으로 삭제된 모든 필드는 더 이상 사용되지 않으며 제거됩니다.

### 연결된 리소스가 있는 POST {#post-linked}

다음 요청 본문 형식을 사용할 때 &quot;vehicleOwner&quot;는 &quot;nms:recipient&quot;에 대한 링크를 나타냅니다.

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

링크 정보는 무시됩니다. 따라서 &quot;vehicleNumber&quot; 및 &quot;vehicleName&quot; 값만 포함된 &quot;cusVehicle&quot;에 새 레코드가 생성됩니다. 하지만 링크는 null로 유지되므로 &quot;vehicleOwner&quot;가 null로 설정됩니다.

Campaign v8에서 동일한 요청 본문 구조를 사용하고 &quot;차량&quot;이 프로필에 연결되어 있으면 오류가 발생합니다. 이 오류는 &quot;firstName&quot; 속성이 &quot;cusVehicle&quot;에 대해 유효한 것으로 인식되지 않기 때문에 발생합니다. 하지만 링크가 없는 속성만 구성하는 요청 본문은 문제 없이 작동합니다.

### PATCH 작업 {#patch}

* Campaign v8은 빈 요청 본문이 있는 PATCH을 지원하지 않습니다. 204 콘텐츠 없음 상태를 반환합니다.
* Campaign Standard은 스키마 내의 요소/특성에 대해 PATCH을 지원하지만, 위치에 대한 PATCH 작업은 Campaign v8에서 지원되지 않습니다. 위치에서 PATCH을 시도하면 &#39;zipCode&#39; 속성이 &#39;profile&#39; 리소스에 유효하지 않다는 오류 메시지와 함께 500 내부 서버 오류가 발생합니다.

### 나머지 응답 {#rest-responses}

아래 섹션에는 Campaign Standard과 v8 REST 응답 간의 사소한 차이점이 나열되어 있습니다.

* 단일 GET 레코드의 경우, 응답은 응답에 href를 포함한다.
* 속성을 사용하여 쿼리하면 Campaign v8은 응답에서 카운트 및 페이지 매김 기능을 제공합니다.
* POST 작업 후 연결된 리소스의 값이 응답에서 반환됩니다.

### 오류 코드 및 메시지 {#rest-errors}

아래 섹션에는 Campaign Standard과 Campaign v8 오류 코드 및 메시지의 차이점이 나와 있습니다.

| 시나리오 | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| 요청 본문에 잘못된 PKey 사용 | 500 - &#39;O5iRp40EGA&#39; 특성을 알 수 없습니다(&#39;프로필(nms:recipient)&#39; 스키마 정의 참조). XTK-170036 표현식 &#39;@id = @O5iRp40EGA&#39;을(를) 구문 분석할 수 없습니다. | 404 - PKey를 해독할 수 없습니다. (PKey=@jksad) |
| URI에 잘못된 PKey 사용 | 500 - &#39;O5iRp40EGA&#39; 특성을 알 수 없습니다(&#39;프로필(nms:recipient)&#39; 스키마 정의 참조). XTK-170036 표현식 &#39;@id = @O5iRp40EGA&#39;을(를) 구문 분석할 수 없습니다. | 404 - PKey를 해독할 수 없습니다. (PKey=@jksad) 지원되지 않는 끝점입니다. (endpoint=rest/profileAndServices/profile/@jksad) |
| URI 및 요청 본문에서 두 개의 서로 다른 원시 Pkey 사용 | 500 - RST-360011 오류가 발생했습니다. 관리자에게 문의하십시오. RST-360012 리소스 &#39;서비스&#39;에서 일관성이 없는 작업 - 키 &#39;SVC3&#39;을(를) &#39;SVC4&#39;로 업데이트할 수 없습니다. | 500 - 오류가 발생했습니다. 관리자에게 문의하십시오. |
| URI에서 PKey를 사용하고 요청 본문에서 다른 원시 PKey 사용 | 500 - 동일한 키 &quot;SVC4&quot;의 &quot;서비스&quot;가 이미 있습니다. PGS-220000 PostgreSQL 오류: 오류: 중복 키 값이 고유 제약 조건 &quot;nmsservice_name&quot;을 위반합니다. DETAIL: 키(sname)=(SVC4)가 이미 있습니다. | 500 - 오류가 발생했습니다. 관리자에게 문의하십시오. |
| URI에 존재하지 않는 원시 ID 사용 | 404 - RST-360011 오류가 발생했습니다. 관리자에게 문의하십시오. &#39;adobe_nl:0&#39; 키(스키마가 &#39;service&#39;이고 이름이 &#39;adobe_nl&#39;인 문서)에서 경로가 &#39;Service&#39;인 문서를 찾을 수 없음 | 404 - &#39;adobe_nl&#39; 키(스키마가 &#39;service&#39;이고 이름이 &#39;adobe_nl&#39;인 문서)에서 &#39;Service&#39; 경로가 있는 문서를 찾을 수 없음 |
| 요청 본문에 존재하지 않는 원시 ID 사용 | 404 - RST-360011 오류가 발생했습니다. 관리자에게 문의하십시오. 경로가 &#39;Service&#39;인 문서를 &#39;adobe_nl&#39; 키(스키마가 &#39;service&#39;이고 이름이 &#39;adobe_nl&#39;인 문서)에서 찾을 수 없습니다. | 404 - &#39;adobe_nl&#39; 키(스키마가 &#39;service&#39;이고 이름이 &#39;adobe_nl&#39;인 문서)에서 &#39;Service&#39; 경로가 있는 문서를 찾을 수 없음 |
| - | 500 - RST-360011 오류가 발생했습니다. 관리자에게 문의하십시오. | 500 - 오류가 발생했습니다. 관리자에게 문의하십시오. |
| 잘못된 성별(또는 기타) 열거형 값이 있는 프로필/서비스 삽입 | 500 - RST-360011 오류가 발생했습니다. 관리자에게 문의하십시오. &#39;invalid&#39; 값은 &#39;@gender&#39; 필드의 &#39;nms:recipient:gender&#39; 열거에 사용할 수 없습니다. | 500 - 오류가 발생했습니다. 관리자에게 문의하십시오. |

### 프로필 시간대 {#profile-timezone}

Campaign Standard을 사용하면 시간대가 **profileAndServices/profile** REST API 호출의 JSON 응답의 일부로 표시됩니다.

Campaign v8에서 시간대는 **profileAndServicesExt/profile** REST API 호출의 일부로만 표시됩니다. 확장 스키마에 추가되고 있으므로 **profileAndServices/profile** REST API 호출의 일부가 아닙니다.

### 워크플로우 외부 신호 {#workflow-signals}

Campaign Standard Workflow GET API는 워크플로 인스턴스 변수 및 해당 데이터 유형(부울, 문자열 등)과 같은 매개 변수 이름을 반환합니다. POST API 호출을 통해 신호를 트리거할 때 적절한 포맷의 JSON 요청 본문을 만드는 데 사용됩니다.

Campaign v8은 광고 워크플로 인스턴스 변수를 지원하지 않지만 개발자는 해당 변수를 알고 있어야 합니다. 따라서 마이그레이션 후 GET API 응답에서 매개 변수 정보를 사용할 수 없으면 POST 요청 본문의 매개 변수 정보를 구성해야 합니다.
