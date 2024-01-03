---
title: 프로필 및 대상자 시작
description: Campaign 웹에서 프로필 및 대상자를 사용하여 작업하는 방법을 알아봅니다
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
badge: label="제한 공개"
source-git-commit: 9e6f0a5894ae0b31d275f978553d7fc73ba9c2eb
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 4%

---

# 프로필 및 대상자 시작 {#about-profiles}

## 프로필 및 대상자 {#about}

Adobe Campaign에서 게재의 대상 모집단은 대상자입니다. 대상자는 유사한 행동 및/또는 특성을 공유하는 프로필 세트입니다. 이 사람 컬렉션은 생성, 선택 또는 로드될 수 있습니다. [아래에 자세히 설명됨](#audiences).

## 타겟팅 차원 {#targeting-dimensions}

타겟팅 차원(예: ) 대상 매핑은 작업에서 처리하는 데이터 유형입니다. 대상 모집단(프로필, 계약 수혜자, 운영자, 구독자 등)을 정의할 수 있습니다.

워크플로우의 타겟팅 차원은 첫 번째 **[!UICONTROL 대상자 작성]** 활동 및 은 워크플로우가 끝날 때까지 모든 추가 활동에서 사용됩니다. 예를 들어, 데이터베이스의 프로필에 대해 쿼리를 수행하면 아웃바운드 전환에 &#39;recipient&#39; 유형의 데이터가 포함되며 다음 활동으로 전송됩니다.

를 사용하여 워크플로우에서 타겟팅 차원을 전환할 수 있습니다. [차원 활동 변경](../workflows/activities/change-dimension.md). 예를 들어 구매 또는 구독과 같은 특정 테이블에서 데이터베이스를 쿼리한 다음 타겟팅 차원을 수신자로 변경하여 해당 프로필로 게재를 보낼 수 있습니다.

기본적으로 이메일 및 SMS 게재 템플릿은 프로필을 타겟팅합니다. 따라서 대상 차원은 의 필드를 사용합니다 **nms:recipient** 테이블. 푸시 알림의 경우 기본 대상 차원은 입니다. **가입자 애플리케이션 nms:appSubscriptionRcp**: 수신자 테이블에 연결됩니다.

아래에 나열된 워크플로우 및 게재에서 다른 내장 대상 매핑을 사용할 수도 있습니다.

| 이름 | 사용 대상 | 스키마 |
|---|---|---|
| 수신자 | 수신자에게 게재(기본 제공 수신자 테이블) | nms:recipient |
| 방문자 | 참조(바이럴 마케팅)를 통해 프로필이 수집된 방문자에게 제공합니다. | mns:visitor |
| 구독 | 뉴스레터 등 정보 서비스를 구독한 수신자에게 게재 | nms:subscription |
| 방문자 구독 | 정보 서비스를 구독한 방문자에게 게재 | nms:visitorSub |
| 연산자 | Adobe Campaign 운영자에게 게재 | nms:operator |
| 외부 파일 | 게재에 필요한 모든 정보가 포함된 파일을 통해 게재 | 연결된 스키마 없음, 입력된 대상 없음 |
| 구독자 애플리케이션 | 애플리케이션을 구독한 수신자에게 게재 | nms:appSubscriptionRcp |

또한 필요에 따라 새 대상 매핑을 만들 수 있습니다. 이 작업은 클라이언트 콘솔에서 수행됩니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
