---
title: 타기팅 차원
description: Adobe Campaign 웹의 타겟팅 차원에 대해 자세히 알아보십시오
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 16%

---

# 타기팅 차원 {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="타기팅 차원 선택"
>abstract="타기팅 차원을 사용하면 수신자, 약정 수혜자, 운영자, 구독자 등 작업에서 타기팅하는 집단을 정의할 수 있습니다. 기본적으로 이메일 및 SMS의 경우 기본 제공 수신자 테이블에서 타깃이 선택됩니다. 푸시 알림의 경우 기본 타기팅 차원은 구독자 애플리케이션입니다."

대상 매핑이라고도 하는 타겟팅 차원은 작업에서 처리하는 데이터 유형입니다. 프로필, 계약 수혜자, 운영자 또는 구독자와 같은 대상 모집단을 정의합니다.

## 워크플로우의 타겟팅 차원 {#workflow}

워크플로우의 타겟팅 차원은 첫 번째 **[!UICONTROL 대상자 작성]** 활동에 의해 정의되며, 워크플로우가 끝날 때까지 모든 후속 활동에 사용됩니다. 예를 들어 데이터베이스에서 프로필을 쿼리할 때 아웃바운드 전환에는 다음 활동으로 전송되는 &#39;recipient&#39; 유형의 데이터가 포함됩니다.

[차원 활동 변경](../workflows/activities/change-dimension.md)을 사용하여 워크플로우에서 타겟팅 차원을 전환합니다. 이렇게 하면 구매 또는 구독과 같은 특정 테이블에 대해 데이터베이스를 쿼리한 다음 타겟팅 차원을 수신자로 변경하여 해당 프로필로 게재를 보낼 수 있습니다.

타겟팅 차원(**대상자 빌드**, **조정** 또는 **차원 변경**&#x200B;과 같은 활동 또는 워크플로우 설정에서)을 선택하면 기본적으로 일반적으로 사용되는 스키마 목록이 표시됩니다. 사용 가능한 모든 스키마를 표시하려면 **[!UICONTROL 모든 스키마 표시]** 단추를 전환합니다. 옵션 선택은 각 사용자에 대해 저장됩니다.

![모든 스키마 표시 단추가 활성화된 타겟팅 차원 인터페이스를 표시하는 스크린샷입니다.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## 타기팅 차원 {#list}

기본적으로 이메일 및 SMS 게재 템플릿은 프로필을 타겟팅합니다. 대상 차원이 **nms:recipient** 테이블의 필드를 사용합니다. 푸시 알림의 경우 기본 대상 차원은 수신자 테이블에 연결된 **구독자 응용 프로그램 nms:appSubscriptionRcp**&#x200B;입니다.

아래 나열된 대로 워크플로우 및 게재에서 다른 내장 대상 매핑을 사용합니다.

| 이름 | 을(를) 게재에 사용 | 스키마 |
|-----------------------|-------------------------------------------------------|-------------------------|
| 수신자 | 프로필/수신자 (기본 제공 수신자 테이블) | nms:recipient |
| 방문자 | 레퍼러(예: 바이럴 마케팅)를 통해 프로필을 수집한 방문자 | mns:visitor |
| 구독 | 뉴스레터 등 정보 서비스를 구독한 프로필 | nms:subscription |
| 방문자 구독 | 정보 서비스를 구독한 방문자 | nms:visitorSub |
| 연산자 | Adobe Campaign 연산자 | nms:operator |
| 외부 파일 | 모든 필수 정보가 포함된 파일을 통한 게재 | 연결된 스키마 없음, 입력된 대상 없음 |
| 구독자 애플리케이션 | 응용 프로그램을 구독한 프로필 | nms:appSubscriptionRcp |

또한 특정 요구 사항에 따라 새 타겟 매핑을 만듭니다. 이 작업은 클라이언트 콘솔에서만 수행합니다. 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ko#new-mapping){target="_blank"}를 참조하세요.