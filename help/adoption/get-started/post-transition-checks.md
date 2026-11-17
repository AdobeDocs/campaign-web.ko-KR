---
title: Campaign v8로 전환한 후 확인 및 문제 해결
description: Campaign Standard에서 Campaign v8로 전환한 후 확인할 사항과 일반적인 문제를 해결하는 방법을 알아봅니다.
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%
---
# 전환 후 확인 및 문제 해결 {#post-transition-checks}

Campaign Standard에서 Campaign v8로 전환하면 일부 게재, 워크플로우 및 랜딩 페이지가 예상과 다르게 동작할 수 있습니다. 아래 표에는 전환된 사용자가 보고한 증상, 원인 및 수행할 작업이 나와 있습니다. 차이점에 대한 전체 목록을 보려면 [Campaign Standard과 Campaign v8 간의 차이점](acs-v8-differences.md)을 참조하세요.

| 증상 | 원인 및 수행할 작업 | 자세히 알아보기 |
|---|---|---|
| 게재의 링크는 직접 URL이며, 클릭 데이터는 수집되지 않습니다. | 추적은 게재 또는 이를 기반으로 하는 게재 템플릿에서 비활성화됩니다. 특히 반복 게재의 템플릿에서 **추적 활성화**&#x200B;가 활성화되어 있는지 확인하십시오. | [추적 설정](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| &quot;mailto&quot; 목록 구독 취소 방법을 통해 구독을 취소한 수신자는 격리되지 않습니다. | 이는 예상되었습니다. 이러한 수신자는 격리로 전송되지 않습니다. 게재와 연계된 서비스에 가입되거나 게재에 서비스가 없는 경우 차단 목록에 추가하다에 추가됩니다. 이러한 구독 취소를 추적하려면 서비스 구독 또는 프로필의 **더 이상 연락하지 않음** 섹션을 확인하십시오. | [격리](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| 랜딩 페이지는 스크립트로 계산되거나 숨겨진 필드에 저장된 값을 저장하지 않습니다. | Campaign 웹 사용자 인터페이스에서 만든 랜딩 페이지는 숨겨진 입력 필드 또는 사용자 지정 JavaScript을 지원하지 않습니다. 대신 클라이언트 콘솔에서 양식을 웹 애플리케이션으로 만듭니다. | [랜딩 페이지](../../v8/landing-pages/get-started-lp.md) |
| **파일 전송**&#x200B;에서 DM 활동으로 생성된 파일을 찾을 수 없습니다. | DM 활동의 아웃바운드 전환은 추출 파일이 아닌 타겟팅된 모집단을 전달합니다. **데이터 추출** 활동을 추가한 다음 **파일 전송** 활동을 추가하십시오. | [DM](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| 게재의 여러 웨이브가 함께 전송됩니다. | 예약된 예약된 예약된 예약된 예약된 예약된 예약된 배송 날짜입니다. 예약된 예약된 시간 이후에 게재가 시작되면 예약된 시간 간격을 사용하지 않고 함께 전송됩니다. | [웨이브를 사용하여 보내기](../../v8/advanced-settings/send-using-waves.md) |
| 별표 뒤에 문자가 있는 파일 마스크는 Azure Blob 저장소에서 파일을 찾을 수 없습니다. | Azure Blob 저장소는 이름 접두사로 파일을 필터링합니다. 후행 별표만 지원됩니다. | [외부 계정 전송](../../v8/administration/transfer-external-account.md) |
| 사용자 지정 JavaScript을 사용하는 랜딩 페이지 또는 콘텐츠 블록은 다르게 동작합니다. | 사용자 지정 JavaScript은 마이그레이션 중에 변환되지만 특히 `queryDef`, Campaign JavaScript API, 세션 쓰기, 조직 단위 처리 또는 사용자 지정 URL 생성을 사용하는 경우 확인하고 조정합니다. | [랜딩 페이지](../../v8/landing-pages/get-started-lp.md) |
| REST API 호출이 빈 값, 오류 또는 예기치 않은 응답을 반환합니다. | 마이그레이션 도중 일부 데이터베이스 필드가 삭제되고 빈 값이 반환됩니다. 빈 PATCH은 204를 반환하고 위치에 대한 PATCH은 500을 반환합니다. 리소스가 연결된 POST는 링크를 무시하거나 오류를 반환합니다. 잘못된 PKEY가 404를 반환합니다. | [REST API 제한](acs-v8-differences.md#rest-api-limitations) |
| 저장된 PKEY는 API 호출에서 더 이상 작동하지 않습니다. | PKEY 값은 마이그레이션 후 변경됩니다. Campaign 외부에 저장하지 마십시오. 이전 호출에서 반환된 href에서 각 호출을 생성합니다. | [키 사용](acs-v8-differences.md#key-usage) |
| 프로필 응답에 표준 시간대 또는 `ccpaOptOut`이(가) 없습니다. | 이 필드는 `profileAndServices/profile`이(가) 아닌 `profileAndServicesExt/profile`에서만 반환됩니다. 확장 끝점을 호출합니다. | [프로필 시간대 및 ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| 사용자 지정 필터가 REST API 호출에서 오류를 반환합니다. | Campaign v8에서 **REST API의 필터 이름** 필드에 필터 이름을 지정하고 &quot;by&quot; 접두사 없이 이 이름을 요청에 있는 그대로 사용합니다. | [필터링](acs-v8-differences.md#rest-filtering) |
| 워크플로우 외부 신호를 트리거하는 호출은 요청 본문을 작성할 수 없습니다. | 워크플로우 GET API는 더 이상 워크플로우 변수를 반환하지 않습니다. 워크플로우에 대한 자신의 지식으로 POST 요청 본문의 매개 변수를 작성합니다. | [워크플로 외부 신호](acs-v8-differences.md#workflow-signals) |
| 트랜잭션 API에 대한 액세스가 거부되었습니다. | 실행 인스턴스에서 트랜잭션 API에 액세스하려면 새 제품 프로필이 필요합니다. 기술 계정의 제품 프로필 매핑을 검토하십시오. | [제품 프로필 매핑](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 마이그레이션된 대상에는 최신 값만 표시되거나 파일 대상에는 차원이 없습니다. | 이는 예상되었습니다. 사전 정의된 필터는 대상자 마이그레이션 후 최신 값만 사용하며, 파일 유형 대상자는 차원이 없는 목록 유형 대상자가 됩니다. | [대상자 관리](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standard에서 실행된 워크플로우 내역이 비어 있습니다. | Campaign Standard에서 실행된 워크플로의 기록 로그는 마이그레이션되지 않습니다. Campaign v8에서 실행되는 워크플로우에는 자체 내역 및 로그가 있습니다. | [워크플로 만들기](marketers.md#acs-gs-marketers-wf) |
| 일부 사용자는 이전보다 더 많은 것을 보거나 수행할 수 있습니다. | **데이터 모델** 역할은 있지만 **관리** 역할은 없는 사용자는 **관리** 액세스 권한을 얻을 수 있으며, 조직 단위가 병렬인 보안 그룹은 더 광범위한 액세스 권한을 가질 수 있습니다. 운영자 그룹, 명명된 권한 및 폴더 권한을 검토합니다. | [사용자 액세스 관리](user-management-acs.md) |
| **Trap**(으)로 표시된 테스트 프로필이 최종 전송을 받지 않습니다. | Campaign v8에서 게재의 대상 설정에 **트랩 그룹**&#x200B;을(를) 추가합니다. | [트랩 그룹](../../v8/audience/trap-group.md) |
| 반복 이메일에는 집계 기간 옵션이 없습니다. | Campaign v8에서는 이 옵션을 사용할 수 없습니다. | [채널 활동](../../v8/workflows/activities/channels.md) |
| 동적 보고에 게재할 데이터가 표시되지 않습니다. | 동적 보고는 이메일 게재, 이메일 게재 캠페인 및 트랜잭션 메시지를 다룹니다. | [보고](marketers.md#acs-gs-marketers-reporting) |
