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
source-git-commit: 071900a6c0b717161ae123097aeae8bf9e97898c
workflow-type: tm+mt
source-wordcount: '649'
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
| Campaign Standard에서 DM 활동의 아웃바운드 전환은 생성된 파일도 전달합니다. Campaign v8에서는 대상 모집단만 전달합니다. 파일을 서버로 보내려면 **데이터 추출** 활동을 추가한 다음 **파일 전송** 활동을 추가하십시오. | [DM](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

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
| PKEY 값은 마이그레이션 후 변경됩니다. Campaign 외부에 PKEY를 저장하는 경우 API에서 반환되는 href를 대신 따릅니다. | [REST API](admin-developers.md#acs-gs-admin-apis) |
| 표준 시간대 및 `ccpaOptOut`과(와) 같은 일부 마이그레이션된 프로필 필드는 `profileAndServicesExt/profile` API에서만 반환됩니다. | [REST API](admin-developers.md#acs-gs-admin-apis) |
| Adobe은 Adobe Analytics 및 Audience Manager 구성을 마이그레이션합니다. 트리거 및 Adobe Target 통합을 다시 설정해야 합니다. | [Adobe Campaign 통합 관리](admin-developers.md#acs-gs-integrations) |
