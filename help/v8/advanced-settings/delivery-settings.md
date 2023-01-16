---
audience: end-user
title: 전자 메일 게재 설정
description: Campaign Web UI의 이메일 게재 설정에 대해 자세히 알아보십시오
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 46d8ac555e554faef91bcc817890466780387d0d
workflow-type: tm+mt
source-wordcount: '1468'
ht-degree: 14%

---

# 전자 메일 게재 설정 {#email-del-settings}

![알파 버전](../assets/do-not-localize/badge.png)

이러한 설정은 다음과 같습니다 **기술 전달 매개 변수** 이메일 템플릿에 정의된 횟수. 이 기능은 **게재 설정 구성** 이메일 게재를 편집할 때 사용할 수 있는 아이콘.

## 전자 메일 게재 설정 {#email-delivery-settings}

>[!CAUTION]
>
> 이러한 설정은 사용자 정보에만 설명되어 있습니다. 일부는 구성 및 권한에 따라 다릅니다. 이 버전의 제품에서 수정하면 안 됩니다.

## 유형화 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="유형화"
>abstract="유형화를 통해 게재 전송을 제어, 필터링 및 모니터링할 수 있습니다."

유형화는 메시지 분석 단계 동안 실행되는 **유형화 규칙** 세트입니다. 이메일에 항상 특정 요소(예: 구독 취소 링크 또는 제목 줄)가 포함되어 있는지 확인하거나 그룹을 의도한 타겟(구독 취소자, 경쟁 업체 또는 비충성 고객)에서 제외하는 필터링 규칙이 있는지 확인할 수 있습니다.

유형화를 메시지 또는 메시지 템플릿과 연결하면 유형화에 포함된 유형화 규칙을 실행하여 메시지를 준비하는 동안 메시지의 유효성을 확인합니다.

![](assets/delivery-settings-1.png)


### 압력 매개변수 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="게재 가중치"
>abstract="게재 가중치를 사용하면 압력 관리 프레임워크 내에서 우선 순위가 가장 높은 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선 순위가 있습니다."

이 섹션에서 압력 매개 변수를 사용하여 **임계값**. 일정 기간 동안 하나의 프로필에 보낼 수 있는 최대 메시지 수입니다. 이 임계값에 도달하면, 고려된 기간이 끝날 때까지 더 이상 게재할 수 없습니다. 이 프로세스를 사용하면 메시지가 설정된 임계값을 초과하는 경우 게재 시 프로필을 자동으로 제외하여 과도한 요청을 방지할 수 있습니다.

임계값은 상수 또는 변수일 수 있습니다. 즉, 특정 기간 동안 임계값은 프로필마다 또는 심지어 동일한 프로필에 대해서도 다를 수 있습니다.

에서 **가중치 유형** 필드, 다음 세 가지 옵션을 사용할 수 있습니다.

* **영구**
* **수신자에 따라 다릅니다.**
* **각 규칙에 정의됨**

를 사용하십시오 **게재 중량** 필드를 사용하여 배달 우선순위를 정의합니다. 각 게재에는 우선 순위 수준을 나타내는 가중치가 있습니다. 기본적으로 게재 가중치는 5로 설정됩니다. 압력 규칙을 사용하여 게재에 적용할 게재 가중치를 정의할 수 있습니다.가중치는 수신자에 맞는 공식을 통해 설정하거나 계산할 수 있습니다. 예를 들어 수신자 관심사에 따라 게재 가중치를 정의할 수 있습니다.


를 사용하십시오 **게재 모드** 대상 평가 모드를 선택하는 필드입니다. 다음 세 가지 모드를 사용할 수 있습니다.

* **대상 예상 및 메시지 개인화**
* **잠정 대상의 예상 및 승인**
* **대상 평가**

피로도 관리는 **캠페인 최적화** 추가 기능. 압력 규칙 및 의 피로 관리를 구성하는 방법에 대해 자세히 알아보십시오 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ko){target="_blank"}.

### 수용작업량 설정 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="수신자의 중요도"
>abstract="수신자의 중요성은 용량 유형화 규칙을 초과할 때 유지되는 수신자를 결정하는 데 사용되는 공식입니다."

이 섹션에서는 Adobe Campaign v8 콘솔에 정의된 용량 규칙을 선택할 수 있습니다. 이 규칙은 이메일 채널과 연결됩니다.

다음 **수신자의 중요성** 필드는 용량 유형화 규칙을 초과할 때 유지되는 수신자를 결정하는 데 사용되는 공식입니다.

일관성 및 용량 규칙 및 구성 방법에 대해 자세히 알아보기 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## 대상자 {#audience}

이 섹션에서 **대상 매핑** 그 중에서 Target 매핑은 Adobe Campaign v8 콘솔에서 정의됩니다.

에서 타겟 매핑에 대해 자세히 알아보십시오 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## 게재 {#delivery}

게재 매개 변수는 게재에 적용되는 기술 설정입니다.

* **라우팅**: 통합 전자 메일 라우팅 외부 계정은 기본적으로 제공됩니다. 애플리케이션이 전자 메일을 보낼 수 있는 기술 매개 변수가 포함되어 있습니다.

* **SMTP 배달 테스트**: 이 옵션은 SMTP를 통한 전송을 테스트하는 데 사용됩니다. 게재는 SMTP 서버에 대한 연결까지 처리되지만 전송되지 않습니다: 게재를 받는 모든 사람에 대해 Campaign은 SMTP 공급자 서버에 연결하고 SMTP RCPT TO 명령을 실행하고 SMTP DATA 명령 전에 연결을 닫습니다.

* **이메일 BCC**: 이 옵션은 메시지 타겟에 숨은 참조 이메일 주소를 추가하면 BCC를 통해 외부 시스템에 이메일을 저장하는 데 사용됩니다. 의 이메일 BCC에 대해 자세히 알아보십시오 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### 다시 시도 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="최대 재시도 수"
>abstract="일시적인 오류로 인해 메시지가 실패하면 게재 기간 동안 다시 시도됩니다."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

의 다시 시도 관리에 대해 자세히 알아보십시오 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 승인 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="승인 모드"
>abstract="게재의 각 단계는 다양한 프로세스를 완벽하게 모니터링하고 제어하기 위해 승인을 받을 수 있습니다."

게재를 준비하는 동안 경고가 생성되면 게재를 구성하여 여전히 실행해야 하는지 여부를 정의할 수 있습니다. 기본적으로 사용자는 분석 단계가 끝날 때 메시지 전송을 확인해야 합니다. 이것은 **수동** 유효성 검사.

해당 필드에서 다른 승인 모드를 선택할 수 있습니다. 사용 가능한 모드는 다음과 같습니다.

* **수동**: 분석 단계가 끝날 때 사용자는 게재를 확인하여 전송을 시작해야 합니다.

* **반자동**: 분석 단계에서 경고 메시지가 생성되지 않으면 전송이 자동으로 시작됩니다.

* **자동**: 전송은 결과와 관계없이 분석 단계가 끝날 때 자동으로 시작됩니다.


## 유효성 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="게재 기간"
>abstract="게재 기간 필드를 사용하면 글로벌 게재 다시 시도의 제한을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 보낸 다음, 오류만 반환하는 메시지의 경우 유효성 제한에 도달할 때까지 정기적으로 구성 가능한 다시 시도가 수행됩니다."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="리소스 유효성 검사 제한"
>abstract="유효성 제한 필드는 주로 미러 페이지와 이미지에 대해 업로드된 리소스에 사용됩니다. 이 페이지의 리소스는 제한된 시간 동안 유효합니다."


다음 **배달 기간** 필드를 사용하면 글로벌 게재 다시 시도 제한을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 보낸 다음, 오류만 반환하는 메시지의 경우 유효성 제한에 도달할 때까지 정기적으로 구성 가능한 다시 시도가 수행됩니다.

날짜를 지정하도록 선택할 수도 있습니다. 이렇게 하려면 을(를) 선택합니다. **유효성 날짜 명시적으로 설정**. 이 경우 게재 및 유효성 제한 날짜도 시간을 지정할 수 있도록 해줍니다. 현재 시간은 기본적으로 사용되지만 입력 필드에서 직접 수정할 수 있습니다.

**자원 유효 한도** 는 주로 미러 페이지 및 이미지에 대해 업로드된 리소스에 사용됩니다. 이 페이지의 리소스는 제한된 시간 동안 유효합니다(디스크 공간을 절약하기 위함).

![](assets/delivery-settings-2.png)


에서 게재 유효 기간에 대해 자세히 알아보십시오 [Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 미러 페이지 관리 {#mirror}

미러 페이지는 웹 브라우저를 통해 온라인으로 액세스할 수 있는 HTML 페이지입니다. 콘텐츠는 이메일과 동일합니다. 기본적으로 링크가 메일 콘텐츠에 삽입되면 미러 페이지가 생성됩니다.

기본 모드 외에 다음 옵션도 사용할 수 있습니다.

* **[!UICONTROL 미러 페이지 강제 생성]**: 게재에 미러 페이지에 대한 링크가 삽입되지 않더라도 미러 페이지가 생성됩니다.
* **[!UICONTROL 미러 페이지를 생성하지 않음]**: 링크가 게재에 있어도 미러 페이지가 생성되지 않습니다.
* **[!UICONTROL 메시지 식별자만 사용하여 액세스할 수 있는 미러 페이지를 생성합니다]**: 이 옵션을 사용하면 게재 로그 창에서 개인화 정보를 사용하여 미러 페이지의 콘텐츠에 액세스할 수 있습니다. 이렇게 하려면 게재 종료 후 **[!UICONTROL 배달]** 탭을 선택하고 미러 페이지를 보려는 수신자 줄을 선택합니다. 을(를) 클릭합니다. **[!UICONTROL 이 메시지의 미러 페이지 표시...]** 링크를 클릭합니다.


### 추적 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="유효 기간"
>abstract="이 옵션은 URL에서 추적이 활성화되는 기간을 정의합니다."

추적 매개 변수는 관련 섹션에 정의됩니다. 가능한 옵션은 다음과 같습니다.

**유효성 제한 추적**: 이 옵션을 사용하여 URL에서 추적이 활성화되는 기간을 변경할 수 있습니다.

**만료된 URL에 대한 대체 URL**: 폴백 웹 페이지의 URL을 입력하려면 이 옵션을 사용합니다. 추적이 만료되면 표시됩니다.

## 테스트 설정 {#test-setttings}

이 섹션에서 제외 매개 변수를 설정할 수 있습니다. 사용 가능한 옵션은 다음과 같습니다.

* **더블 유지** 여러 타겟팅 기준을 충족하는 수신자에게 여러 게재를 승인할 수 있도록 해줍니다.

* **차단 목록에 추가된 주소 유지** 구독 취소(옵트아웃) 후와 같이, 더 이상 게재의 타겟이 되지 않는 프로필을 타겟에서 계속 지정할 수 있습니다.

* **격리된 주소 유지** 응답하지 않는 주소가 있는 모든 프로필을 타겟에서 보호할 수 있습니다.

증명 이름을 사용자 지정할 수도 있습니다.

를 사용하십시오 **증명 게재 코드 유지** 를 증명에 연결하는 방법은 게재에 대해 정의된 코드와 동일한 배달 코드를 나타냅니다.

기본적으로 증명의 제목에는 &#39;PROOF #&#39;이라는 접두사가 붙습니다. 여기서 #은 증명의 번호입니다. 이 접두사는 **레이블 접두사** 필드.