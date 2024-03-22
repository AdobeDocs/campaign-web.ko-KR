---
title: 최신 릴리스 정보
description: Campaign Web 사용자 인터페이스에서 제공하는 새로운 기능 살펴보기
source-git-commit: 5b0e59e8bb7e4a8ee3ce648c4af7dd9e41be7a81
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 85%

---

# 릴리스 정보 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="새로운 기능"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 릴리스 정보는 월별로 여러 차례 업데이트됩니다. **3월 릴리스가 현재 공개**&#x200B;되었으며, 여기에는 다이렉트 메일 채널, 새로운 데이터 소스 변경 워크플로 활동 및 기타 개선 사항이 포함되어 있습니다."


<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

>[!AVAILABILITY]
>
>이 버전은 [Campaign (콘솔) v8.6 릴리스](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko)를 시작하는 모든 사용자가 사용할 수 있습니다. [Campaign v8 (콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=ko){target="_blank"}에서 Adobe Campaign 클라이언트 콘솔 릴리스 및 업그레이드에 대해 자세히 알아보십시오.

## 3월 릴리스 정보 {#24-3-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="DM"
>abstract="이제 워크플로우 및 독립 실행형 게재에서 DM 채널을 사용할 수 있습니다. DM 오프라인 채널을 사용하여 추출 파일을 만들고, 개인화하고, 생성한 다음 DM 공급자와 공유하여 고객에게 메일을 보낼 수 있습니다."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="릴리스 정보 참조"

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="데이터 소스 변경"
>abstract="새로운 데이터 소스 변경 워크플로우 타깃팅 활동을 사용하여 워크플로우의 작업 테이블에서 사용되는 데이터 소스를 변경합니다. 이 활동을 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상할 수 있어 유연성이 향상됩니다."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="릴리스 정보 참조"


**릴리스 일자**: 2024년 3월 19~20일

### 다이렉트 메일 채널 {#24-3-dm}

이제 **다이렉트 메일** 채널을 워크플로 및 독립 실행형 게재에 사용할 수 있습니다. 다이렉트 메일은 다이렉트 메일 공급자가 고객에게 메일을 보내는 데 사용하는 추출 파일을 만들고, 개인화하고, 생성하여 해당 공급자와 공유할 수 있는 오프라인 채널입니다. [자세히 보기](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 데이터 소스 워크플로 활동 신규 변경 {#24-3-change-data-source}

**데이터 소스 변경** 타겟팅 활동을 사용하면 워크플로의 작업 테이블에서 사용하는 데이터 소스를 변경할 수 있습니다. 이 활동을 통해 다양한 데이터베이스에서 데이터를 관리하고 성능을 향상할 수 있어 유연성이 향상됩니다. [자세히 보기](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 분할 워크플로 활동 개선 {#24-3-split}

이제 **분할** 워크플로 활동의 **동일한 테이블에서 모든 하위 집합 생성** 옵션을 사용하여 모든 하위 집합을 단일 출력 전환으로 그룹화할 수 있습니다. [자세히 보기](../workflows/activities/split.md)

### 쿼리 모델러 {#24-3-query-modeler}

* 이제 이메일 디자이너에서 쿼리 모델러를 사용할 수 있습니다. 이를 통해 조건부 콘텐츠를 생성할 때 조건을 빌드할 수 있습니다. [자세히 보기](../personalization/conditions.md)
* 이제 사용자 정의 조건을 생성할 때 날짜 유형 속성에 대해 사전 정의된 값을 사용할 수 있습니다. [자세히 보기](../query/build-query.md)
* 더 이상 다이어그램의 새 전환에 연산자를 추가할 수 없습니다. 구성 요소를 필터링하여 함께 그룹화하기 전에는 기존 전환에만 추가할 수 있습니다. [자세히 보기](../query/build-query.md)
