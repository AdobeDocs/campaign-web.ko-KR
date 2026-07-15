---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: b8cf1d45b1a69efbe8e055d57b430d0fa04f8494
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 93%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 2026년 6월 릴리스 {#26-6-release}

_2026년 6월 16일_

### 개선 사항 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* 이제 추적 로그를 포함한 모든 목록 화면에서 데이터를 내보낼 수 있습니다. 목록을 찾아 내보내기 버튼을 클릭하면 됩니다. 내보내기에는 현재 로드된 행이 포함되며 화면에 표시되는 열과 모든 활성 검색 또는 필터가 고려됩니다. [자세히 알아보기](../get-started/list-filters.md)

* 이제 **중복 제거** 및 **종료** 워크플로 활동이 여러 인바운드 전환을 지원합니다. 두 개 이상의 인바운드 전환을 사용할 수 있는 경우 활동에서 **가입할 집합** 섹션을 사용하십시오.
연결할 전환을 선택할 수 있습니다. 다음 페이지에서 자세히 알아보기: [중복 제거](../workflows/activities/deduplication.md), [종료](../workflows/activities/end.md)

* 이제 고급 매개변수가 **대상자 빌드**(쿼리 유형) 및 **보강** 워크플로 활동의 **데이터 보강** 섹션에 표시됩니다. 이들 매개변수를 사용하면 그룹화, 중복 제거, 기본 키 처리 및 인바운드 이벤트 데이터를 포함하여 데이터 보강 방법을 세부적으로 조정할 수 있습니다. [자세히 알아보기](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
