---
audience: end-user
title: 고급 설정
description: Campaign v8 웹 설명서
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 10%

---

# 고급 설정 {#advanced-settings}

>[!NOTE]
>
>이 설명서는 개발 중이며 자주 업데이트됩니다. 이 컨텐츠의 최종 버전은 2023년 1월에 준비될 예정입니다.

이러한 설정은 전자 메일 템플릿에 정의된 기술 게재 매개 변수입니다. 특정 게재에 대해 수정하려면 다음 단계를 신중하게 수행합니다.

## 전자 메일 게재 설정 {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

템플릿의 모든 기술 게재 매개 변수입니다.
매개 변수만 변경하고 여기에서 만들 수는 없습니다.
사용 권한에 따라, 작업자는 이를 수정해서는 안 됩니다. 템플릿에 정의된 유형화 규칙 -> rest 만 확인 및 변경합니다.

## 유형화 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="유형화"
>abstract="유형화를 통해 게재 전송을 제어, 필터링 및 모니터링할 수 있습니다."

### 압력 매개 변수 {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="게재 가중치"
>abstract="게재 가중치를 사용하면 압력 관리 프레임워크 내에서 우선 순위가 가장 높은 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선 순위가 있습니다."

### 수용작업량 설정 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="수신자의 중요도"
>abstract="TBC"


## 대상자 {#audience}

## 게재 {#delivery}

### 다시 시도 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="최대 재시도 횟수"
>abstract="일시적인 오류로 인해 메시지가 실패하면 게재 기간 동안 다시 시도됩니다."

## 승인 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="승인 모드"
>abstract="게재의 각 단계는 다양한 프로세스를 완벽하게 모니터링하고 제어하기 위해 승인을 받을 수 있습니다."

## 유효성 {#validity}

### 유효 기간 {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="게재 기간"
>abstract="게재 기간 필드를 사용하면 글로벌 게재 다시 시도의 제한을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 보낸 다음, 오류만 반환하는 메시지의 경우 유효성 제한에 도달할 때까지 정기적으로 구성 가능한 다시 시도가 수행됩니다."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="리소스 유효성 검사 제한"
>abstract="유효성 제한 필드는 주로 미러 페이지와 이미지에 대해 업로드된 리소스에 사용됩니다. 이 페이지의 리소스는 제한된 시간 동안 유효합니다."


### 추적 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="유효 기간"
>abstract="이 옵션은 URL에서 추적이 활성화되는 기간을 정의합니다."














