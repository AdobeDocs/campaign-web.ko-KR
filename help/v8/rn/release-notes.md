---
title: 최신 릴리스 정보
description: Campaign Web 사용자 인터페이스에서 제공하는 새로운 기능 살펴보기
source-git-commit: 737a2ea3f3c5ecc41c692ada7927f5e60ecb256a
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 8%

---

# 릴리스 정보 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="새로운 기능"
>abstract="Adobe Campaign 웹 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 제공 모델에서 작동합니다. 릴리스 노트는 한 달에 여러 번 업데이트됩니다. **3월 릴리스가 공개되었습니다.** DM 채널, 새로운 데이터 소스 변경 워크플로우 활동 및 기타 개선 사항을 포함합니다."


<!--Last update: **March 19, 2024**-->

Adobe Campaign 웹 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 제공 모델에서 작동합니다. 따라서 이러한 릴리스 노트는 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하십시오.

>[!AVAILABILITY]
>
>이 버전은 다음을 시작하는 모든 사용자가 사용할 수 있습니다. [Campaign(콘솔) v8.6 릴리스](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko). 에서 Adobe Campaign 클라이언트 콘솔 릴리스 및 업그레이드에 대해 자세히 알아보십시오. [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=ko){target="_blank"}.

## 3월 릴리스 {#24-3-release}

**릴리스 날짜**: 2024년 3월 19~20일

### 다이렉트 메일 채널 {#24-3-dm}

**다이렉트 메일** 이제 채널은 워크플로우에서 독립 실행형 게재로 사용할 수 있습니다. DM은 추출 파일을 만들고, 개인화하고, 생성하고, DM 공급자와 공유하여 고객에게 메일을 보낼 수 있는 오프라인 채널입니다. [자세히 보기](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 새로운 데이터 소스 변경 워크플로우 활동 {#24-3-change-data-source}

다음 **데이터 소스 변경** 타겟팅 활동을 사용하면 워크플로우의 작업 테이블에서 사용되는 데이터 소스를 변경할 수 있습니다. 이 활동을 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상시킬 수 있으므로 보다 유연하게 작업할 수 있습니다. [자세히 보기](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 분할 워크플로우 활동 개선 사항 {#24-3-split}

이제 다음을 사용할 수 있습니다. **동일한 테이블의 모든 하위 집합 생성** 의 옵션 **분할** 워크플로우 활동을 통해 모든 하위 집합을 단일 출력 전환으로 그룹화합니다. [자세히 보기](../workflows/activities/split.md)

### 쿼리 모델러 {#24-3-query-modeler}

* 이제 쿼리 모델러를 이메일 디자이너에서 사용할 수 있습니다. 조건부 콘텐츠를 만들 때 조건을 작성할 수 있도록 해 줍니다. [자세히 보기](../personalization/conditions.md)
* 이제 사용자 지정 조건을 만들 때 날짜 유형 속성에 대해 사전 정의된 값을 사용할 수 있습니다. [자세히 보기](../query/build-query.md)
* 다이어그램의 새 전환에 연산자를 더 이상 추가할 수 없습니다. 구성 요소를 필터링하여 함께 그룹화하기 전에 기존 전환에만 추가할 수 있습니다. [자세히 보기](../query/build-query.md)
