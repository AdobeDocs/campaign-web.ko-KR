---
audience: end-user
title: 게재 설정 구성
description: Campaign 웹에서 게재 설정을 구성하는 방법 알아보기
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 5835d45ea2a383eed7d280fdd263548ea2e8530d
workflow-type: tm+mt
source-wordcount: '3159'
ht-degree: 41%

---


# 게재 설정 구성 {#del-settings}

배달 설정은 배달 템플릿에 정의된 **기술 배달 매개 변수**&#x200B;입니다. 각 게재에 대해 오버로드될 수 있습니다. 이러한 설정은 게재 또는 게재 템플릿을 편집할 때 사용할 수 있는 **설정** 단추에서 사용할 수 있습니다.

>[!CAUTION]
>
>이러한 설정은 정보 목적으로만 설명됩니다. 그 중 일부는 구성 및 권한에 따라 다릅니다. 이 버전의 제품에서는 수정할 수 없습니다.

## 유형화 설정 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="유형화"
>abstract="유형화를 통해 모든 게재에서 비즈니스 사례를 표준화할 수 있습니다. 유형화는 게재 전송에 대해 제어, 필터링 및 우선순위 지정을 수행할 수 있는 유형화 규칙 모음입니다. 유형화 규칙 내의 기준과 일치하는 프로필은 준비 단계에 게재 대상자에서 제외됩니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="게재에 대한 유형화 설정"
>abstract="유형화 규칙을 통해 모든 게재에서 비즈니스 사례를 표준화할 수 있습니다. 유형화는 게재 전송에 대해 제어, 필터링 및 우선순위 지정을 수행할 수 있는 유형화 규칙 모음입니다. 유형화 규칙 내의 기준과 일치하는 프로필은 준비 단계에 게재 대상자에서 제외됩니다."

유형화는 한 번에 여러 필터링 규칙을 쉽게 게재에 적용하기 위해 준비 단계 동안 실행되는 **유형화 규칙** 집합입니다. 이를 통해 마케터는 게재 전송을 제어, 필터링 및 우선 순위를 지정할 수 있으므로 모든 게재에서 비즈니스 사례를 표준화할 수 있습니다. [유형화 및 유형화 규칙을 만드는 방법을 알아봅니다](../administration/typologies.md)

![](assets/delivery-settings-typology.png){zoomable="yes"}

### 압력 매개변수 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="게재에 대한 압력 매개변수"
>abstract="게재 가중치를 통해 피로도 관리 프레임워크 내에서 최우선 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선순위가 높습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="게재 가중치"
>abstract="게재 가중치를 통해 압력 관리 프레임워크 내에서 최우선 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선순위가 높습니다."

이 섹션에서 압력 매개 변수를 사용하면 피로도 관리 규칙을 설정할 **임계값**&#x200B;을(를) 정의할 수 있습니다. 피로도 관리 규칙은 지정된 기간 동안 한 프로필에 보낼 수 있는 최대 메시지 수입니다.

이 임계값에 도달하면 고려된 기간이 끝날 때까지 더 이상 게재할 수 없습니다. 이 프로세스를 사용하면 메시지가 설정된 임계값을 초과하는 경우 게재 시 프로필을 자동으로 제외하여 과도한 요청을 방지할 수 있습니다.

임계값은 상수 또는 변수일 수 있습니다. 즉, 특정 기간 동안 임계값은 프로필마다 또는 심지어 동일한 프로필에 대해서도 다를 수 있습니다.

**[!UICONTROL 가중치 유형]** 필드에서 다음 세 가지 옵션을 사용할 수 있습니다.

* **[!UICONTROL 일정]**
* **[!UICONTROL 수신자에 따라 다름]**
* **[!UICONTROL 각 규칙에 정의됨]**

**[!UICONTROL 게재 가중치]** 필드를 사용하여 게재 우선 순위를 정의합니다. 각 게재에는 우선 순위 수준을 나타내는 가중치가 있습니다. 기본적으로 게재 가중치는 5로 설정되어 있습니다. 압력 규칙을 사용하면 적용되는 게재의 가중치를 정의할 수 있습니다. 가중치는 수신자에 맞게 공식을 통해 설정하거나 계산할 수 있습니다. 예를 들어 수신자의 관심사에 따라 게재 가중치를 정의할 수 있습니다.

**[!UICONTROL 배달 모드]** 필드를 사용하여 대상 평가 모드를 선택하십시오.

다음 세 가지 모드를 사용할 수 있습니다.

* **[!UICONTROL 대상 예상 및 메시지 개인화]**
* **[!UICONTROL 잠정 대상 예상 및 승인]**
* **[!UICONTROL 대상 평가]**

>[!NOTE]
>
>피로도 관리 및 압력 규칙은 Campaign 클라이언트 콘솔에 구성됩니다. 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ko){target="_blank"}를 참조하세요.

### 수용작업량 설정 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="게재에 대한 수용작업량 설정"
>abstract="메시지를 게재하기 전에 수용작업량 규칙을 사용하여 조직이 게재, 게재로 인해 생성될 수 있는 인바운드 메시지와 구독자에게 문의할 수 있는 통화 수를 처리할 수 있는지 확인합니다. 수용작업량 규칙은 Adobe Campaign v8 콘솔에 정의되어 있습니다. 이 화면에서 채널과 연계된 규칙을 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="수신자 중요도"
>abstract="수신자 중요도는 용량 유형화 규칙 초과 시 유지되는 프로필을 결정하는 데 사용되는 공식입니다."

이 섹션에서는 Adobe Campaign v8 콘솔에 정의된 용량 규칙을 선택할 수 있습니다. 이 규칙은 채널과 연결되어 있습니다.

**[!UICONTROL 수신자의 중요도]** 필드는 용량 유형화 규칙을 초과할 때 어떤 프로필이 유지되는지 확인하는 데 사용되는 수식입니다.

>[!NOTE]
>
>유형화 규칙은 Campaign 클라이언트 콘솔에 구성됩니다. 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=ko){target="_blank"}를 참조하세요.

## 대상자 설정 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="게재에 대한 대상자 설정"
>abstract="사용 가능한 **대상 매핑** 중 원하는 옵션을 선택합니다. 대상 매핑은 Adobe Campaign v8 콘솔에서 정의됩니다. 게재에 대한 제외 매개변수를 설정할 수도 있습니다."

이 섹션에서는 사용 가능한 **대상 매핑** 중 원하는 옵션을 선택할 수 있습니다. 대상 매핑은 Adobe Campaign v8 콘솔에서 정의됩니다. 대상 매핑은 작업에서 처리하는 데이터 유형입니다. 대상 모집단(수신자, 계약 수혜자, 운영자, 구독자 등)을 정의할 수 있습니다. [대상 매핑에 대해 자세히 알아보기](../audience/targeting-dimensions.md).

**[!UICONTROL 제외]** 필드에서 더 이상 연락을 원치 않거나 격리된 프로필을 제외하도록 선택할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=ko){target="_blank"}

## 게재 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="게재에 대한 전역 설정"
>abstract="게재 매개변수는 게재에 적용되는 기술 설정입니다. 게재 및 일반 모드를 변경하고, 이메일 BCC를 활성화하고, 예약된 일괄 처리를 사용하여 전송하고, 전송된 이메일 메시지의 형식을 선택할 수도 있습니다. 이 옵션은 숙련된 사용자로만 제한됩니다."

**[!UICONTROL 게재]** 매개 변수는 게재에 적용되는 기술 설정입니다.

![](assets/delivery-settings-delivery.png){zoomable="yes"}

기본적으로 통합된 **[!UICONTROL 라우팅]** 외부 계정이 제공됩니다. 여기에는 애플리케이션이 게재를 보낼 수 있는 기술 매개 변수가 포함되어 있습니다.

아래에 **[!UICONTROL 전송]** 설정을 정의할 수 있습니다.

* **[!UICONTROL 게재 우선 순위]**: 우선 순위 수준을 보통, 높음 또는 낮음으로 설정하여 게재의 전송 순서를 변경하려면 이 옵션을 사용합니다.

* **[!UICONTROL 메시지 일괄 처리 수량]**: 이 옵션을 사용하여 동일한 XML 게재 패키지 내에서 그룹화된 메시지 수를 정의합니다. 매개 변수를 0으로 설정하면 메시지가 자동으로 그룹화됩니다. 패키지 크기는 패키지로 최소 8개에서 최대 256개의 메시지로 계산 `<delivery size>/1024`에 의해 정의됩니다.

  >[!IMPORTANT]
  >
  >기존 게재를 복제하여 게재를 만들 때 이 매개 변수는 재설정됩니다.

* **[!UICONTROL SMTP 배달 테스트]**(전자 메일 채널): 이 옵션은 SMTP를 통한 전송을 테스트하는 데 사용됩니다. 전자 메일은 SMTP 서버 연결까지 처리되지만 전송되지 않습니다. 전자 메일의 모든 수신자에 대해 Campaign은 SMTP 공급자 서버에 연결하고 SMTP RCPT TO 명령을 실행하고 SMTP DATA 명령 전에 연결을 닫습니다.

* **[!UICONTROL 전자 메일 BCC]**(전자 메일 채널): 이 옵션은 메시지 대상에 BCC 전자 메일 주소를 추가하여 BCC를 통해 외부 시스템에 전자 메일을 저장하는 데 사용됩니다. 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html?lang=ko){target="_blank"}를 참조하세요.

**[!UICONTROL 웨이브 정의]** 섹션에서 **[!UICONTROL 여러 웨이브를 사용하여 보내기]** 옵션을 선택하여 웨이브를 사용하여 보낸 볼륨을 점진적으로 늘립니다. 이렇게 하면 메시지가 스팸으로 표시되거나 하루에 메시지 수를 제한하려는 경우를 방지할 수 있습니다. 웨이브를 사용하여 동시에 대량의 메시지를 전송하는 대신 게재를 여러 배치로 나눌 수 있습니다. [자세히 알아보기](send-using-waves.md)

전자 메일의 경우 아래에 자세히 설명된 대로 보낸 메시지의 **[!UICONTROL 메일 형식]**&#x200B;을 변경할 수도 있습니다.

* **[!UICONTROL 받는 사람 환경 설정 사용]**(기본 모드): 전자 메일 형식은 받는 사람 프로필에 저장된 데이터에 따라 정의됩니다. 수신자가 특정 형식으로 이메일을 수신하려는 경우 이는 전송된 형식입니다. 필드를 입력하지 않으면 다중 파트 대체 이메일이 전송됩니다(아래 참조).

* **[!UICONTROL 받는 사람 메일 클라이언트가 가장 적절한 형식을 선택할 수 있도록 합니다]**: 전자 메일에는 텍스트 및 HTML의 두 형식 모두가 포함됩니다. 수신에 표시되는 형식은 수신자의 메일 소프트웨어(다중 파트 대체)의 구성에 따라 다릅니다.

  >[!IMPORTANT]
  >
  >이 옵션에는 문서의 두 버전이 모두 포함됩니다. 따라서 이메일 크기가 더 크기 때문에 게재 속도에 영향을 줍니다.

* **[!UICONTROL 모든 메시지를 텍스트 형식으로 보내기]**: 전자 메일이 텍스트 형식으로 전송됩니다. HTML 형식은 전송되지 않지만 수신자가 이메일을 클릭할 때만 미러 페이지에 사용됩니다.

## 웹 분석 {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="게재에 대한 웹 분석 설정"
>abstract="웹 분석 계정을 선택합니다. 이 계정은 Campaign 클라이언트 콘솔에서 구성됩니다. 사용 중인 분석 도구와 공유되는 태그를 정의할 수도 있습니다."

이 섹션에서 웹 분석 계정을 선택할 수 있습니다. 이 계정은 Campaign 클라이언트 콘솔에 구성됩니다.

사용 중인 분석 도구와 공유되는 태그를 정의할 수도 있습니다.

>[!NOTE]
>
>웹 분석 기능은 Campaign 클라이언트 콘솔에서 구성됩니다. 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=ko#external-account-ac){target="_blank"}를 참조하세요.

## 재시도 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="최대 재시도 수"
>abstract="일시적인 오류로 인해 메시지 전송이 실패하면 게재 기간이 종료될 때까지 재시도를 수행합니다."

<!--Currently not visible in UI > ??-->

소프트 또는 무시됨 오류로 인해 일시적으로 게재되지 않은 메시지는 자동 재시도의 적용을 받습니다. 기본적으로 5번의 다시 시도가 배달 첫 날에 예약되며 하루 중 24시간 동안 최소 1시간 간격으로 분산됩니다.

## 승인 (이메일 채널) {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="게재 승인 모드"
>abstract="승인 모드를 선택합니다. 게재 준비 중에 경고가 생성되면 게재를 계속 실행해야 하는지 여부를 정의하도록 구성할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="게재 승인 모드"
>abstract="이 템플릿을 기반으로 게재에 대한 승인 모드를 선택합니다. 게재 준비 중에 경고가 생성되면 게재를 계속 실행해야 하는지 여부를 정의하도록 구성할 수 있습니다."

이메일 게재를 준비하는 동안 경고가 생성되면 게재를 구성하여 계속 실행할지 여부를 정의할 수 있습니다. 기본적으로 사용자는 분석 단계가 끝날 때 이메일 전송을 확인해야 합니다. **수동** 유효성 검사입니다.

적절한 필드에서 다른 승인 모드를 선택할 수 있습니다. 사용 가능한 모드는 다음과 같습니다.

* **[!UICONTROL 수동]**: 분석 단계가 끝나면 사용자는 전송을 시작하기 위해 게재를 확인해야 합니다.
* **[!UICONTROL 반자동]**: 분석 단계에서 경고 메시지가 생성되지 않으면 자동으로 전송이 시작됩니다.
* **[!UICONTROL 자동]**: 결과와 관계없이 분석 단계가 끝나면 자동으로 전송이 시작됩니다.

## 유효성 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="설정 유효성"
>abstract="**게재 기간** 필드를 통해 글로벌 게재 재시도에 대한 제한 값을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 전송하고 나서 메시지가 오류만 반환하는 경우 유효성 검사 제한에 도달할 때까지 구성 가능한 일반 재시도를 수행합니다.<br>**리소스 유효성 검사 제한** 필드는 미러 페이지나 이미지와 같이 업로드된 리소스에 사용됩니다. 제한에 도달하면 리소스를 더 이상 사용할 수 없습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="리소스 유효성 검사 제한"
>abstract="**리소스 유효성 검사 제한** 필드는 미러 페이지나 이미지와 같이 업로드된 리소스에 사용됩니다. 이러한 리소스는 제한된 시간 동안만 유효합니다. 한도에 도달하면 리소스를 더 이상 사용할 수 없습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="게재 기간"
>abstract="**게재 기간** 필드를 통해 글로벌 게재 재시도에 대한 제한 값을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 전송하고 나서 메시지가 오류만 반환하는 경우 유효성 검사 제한에 도달할 때까지 구성 가능한 일반 재시도를 수행합니다."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### 유효 기간 {#validity-period}

**[!UICONTROL 게재 기간]** 필드를 통해 글로벌 게재 재시도에 대한 제한 값을 입력할 수 있습니다. 즉, Adobe Campaign은 시작 날짜부터 메시지를 전송하고 나서 메시지가 오류만 반환하는 경우 유효성 검사 제한에 도달할 때까지 구성 가능한 일반 재시도를 수행합니다.

날짜를 지정할 수도 있습니다. 이렇게 하려면 **[!UICONTROL 명시적으로 유효일자 설정]**&#x200B;을 선택하십시오. 이 경우 게재 및 유효성 검사 제한 날짜를 통해 시간을 지정할 수도 있습니다. 기본적으로 현재 시간이 사용되지만 입력 필드에서 직접 수정할 수 있습니다.

**[!UICONTROL 리소스 유효성 검사 제한]**&#x200B;은(는) 주로 미러 페이지와 이미지에 대해 업로드된 리소스에 사용됩니다. 이 페이지의 리소스는 제한된 시간 동안 유효합니다(디스크 공간을 절약하기 위함). 이 제한이 지나면 이러한 리소스를 더 이상 사용할 수 없습니다.

![](assets/delivery-settings-validity.png){zoomable="yes"}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

[Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=ko#validity-period){target="_blank"}에서 게재 유효 기간에 대해 자세히 알아보세요.

### 미러 페이지 관리(이메일 채널) {#mirror}

미러 페이지는 웹 브라우저를 통해 온라인으로 액세스할 수 있는 HTML 페이지입니다. 콘텐츠는 이메일과 동일합니다. 링크가 이메일의 콘텐츠에 삽입되면 기본적으로 미러 페이지가 생성됩니다.

기본 모드 이외에 다음 옵션도 사용할 수 있습니다.

* **[!UICONTROL 미러 페이지 강제 생성]**: 이메일에 미러 페이지 링크가 삽입되지 않은 경우에도 이 모드를 사용하여 미러 페이지를 생성하십시오.
* **[!UICONTROL 미러 페이지를 생성하지 않음]**: 링크가 이메일에 있더라도 미러 페이지를 생성하지 않도록 하려면 이 모드를 사용하십시오.
* **[!UICONTROL 메시지 식별자만 사용하여 액세스할 수 있는 미러 페이지를 생성합니다.]**: 미러 페이지 링크가 이메일 콘텐츠에 없는 경우 이 옵션을 사용하여 게재 로그 창에서 클라이언트 콘솔에서 미러 페이지의 콘텐츠에 액세스할 수 있도록 설정하십시오.

### 추적 {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="유효 기간"
>abstract="유효 기간은 메시지 URL에서 추적이 활성화되는 기간을 설정합니다."

**[!UICONTROL 추적]** 매개 변수가 관련 섹션에 정의되어 있습니다. 가능한 옵션은 다음과 같습니다.

* **[!UICONTROL 추적 유효성 제한]**: 이 옵션을 사용하여 URL에서 추적이 활성화되는 기간을 변경할 수 있습니다.
* **[!UICONTROL 만료된 URL에 대한 대체 URL]**: 이 옵션을 사용하여 대체 웹 페이지에 대한 URL을 입력하십시오. 추적이 만료되면 표시됩니다.

## 교정쇄 설정 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="게재에 대한 교정쇄 설정 정의"
>abstract="제외 매개변수를 선택하고 교정쇄의 레이블을 사용자 정의합니다."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

이 섹션에서는 제외 매개변수를 설정할 수 있습니다. 사용 가능한 옵션은 다음과 같습니다.

* **[!UICONTROL 중복 항목 유지]**&#x200B;를 사용하면 여러 타깃팅 기준을 충족하는 프로필에 여러 게재를 승인할 수 있습니다.
* **[!UICONTROL 차단 목록에 추가된 주소 보관]** 옵션을 사용하면 구독 취소(옵트아웃) 후와 같이 게재에서 더 이상 대상으로 지정되지 않는 프로필을 대상에서 유지할 수 있습니다.
* **[!UICONTROL 격리된 주소 보관]** 옵션을 사용하면 주소가 응답하지 않는 프로필을 대상에서 유지할 수 있습니다.

다음과 같이 증명 레이블을 사용자 지정할 수도 있습니다.

* **[!UICONTROL 증명에 대한 게재 코드 보관]**&#x200B;을 사용하여 관련된 게재에 대해 정의된 것과 동일한 게재 코드를 증명에 연결합니다.
* 기본적으로 증명 제목에는 &#39;PROOF #&#39;가 붙습니다. 여기서 #은 증명 번호입니다. 이 접두사는 **[!UICONTROL 레이블 접두사]** 필드에서 변경할 수 있습니다.

## SMS 설정(SMS 채널) {#sms-tab}

>[!CONTEXTUALHELP]
>id="acw_sms_delivery_settings"
>title="SMS 게재 설정"
>abstract="SMS 게재 매개 변수는 SMS 게재에 적용되는 기술 설정입니다. 발신자 주소, 서비스 매개변수, 전송 모드 등을 정의할 수 있습니다. 이 옵션은 숙련된 사용자로만 제한됩니다."

SMS 게재 매개 변수는 SMS 게재에 적용되는 기술 설정입니다. 발신자 주소, 서비스 매개변수, 전송 모드 등을 정의할 수 있습니다. 이 옵션은 숙련된 사용자로만 제한됩니다.

<!--

* **[!UICONTROL Sender address]**

  The field is limited to 21 characters by the SMPP specification, but some providers may allow longer values. Note also that very strict restrictions may be applied in some countries (length, content, allowed characters, …), so you may need to double-check that the content you place here is legal. Be especially careful when using personalized fields.


  This optional field allows you to override the sender address (oADC). Its content is placed in the *source_addr* field of the SUBMIT_SM PDU.

  Although the SMPP specification limits this field to 21 characters, some providers may support longer values. Be aware that certain countries impose strict regulations on sender addresses (regarding length, content, allowed characters, etc.), so always verify that your input complies with local requirements. Use extra caution when working with personalized fields.

  If this field is left empty, the value of the Source number field defined in the external account will be used instead. If both values are empty, the *source_addr* field will be left empty.

-->

* **[!UICONTROL 서비스 유형]**:

  이 매개 변수는 그대로 공급자에게 전달됩니다.

* **[!UICONTROL 서비스 또는 프로그램 ID]**

  >[!NOTE]
  >
  >이 필드는 사용하지 마십시오. 클라이언트 콘솔에서 사용할 수 있는 선택적 SMPP 매개 변수는 훨씬 더 유연한 구현을 제공합니다.
  >
  >이 필드는 선택적 SMPP 매개 변수와 동시에 사용할 수 없습니다.

  일치하는 외부 계정 설정과 결합하여 각 MT에 하나의 선택적 매개 변수를 보낼 수 있습니다. 이 필드는 TLV의 값 부분을 정의합니다.

* **[!UICONTROL 전송 모드]**

  이 필드는 전송할 SMS 유형(일반 메시지인지 플래시 메시지인지 여부 및 모바일 장치에 저장해야 하는지 또는 SIM 카드에 저장해야 하는지 여부)을 정의합니다. 이 설정은 SUBMIT_SM PDU의 dest_addr_subunit 선택 필드에서 전송됩니다.

   * **Flash**&#x200B;이(가) 값을 1로 설정합니다. 화면에 즉시 나타나며 저장되지 않는 Flash SMS를 보냅니다.
   * **보통**&#x200B;은 값을 0으로 설정합니다. 표준 SMS를 보냅니다.
   * **모바일에 저장됨**&#x200B;에서 값을 2로 설정합니다. SMS를 내부 메모리에 저장하도록 장치에 지시합니다.
   * **터미널에 저장됨**&#x200B;이(가) 값을 3으로 설정합니다. SMS를 SIM 카드에 저장하도록 장치에 지시합니다.

* **[!UICONTROL 우선 순위, 통신 유형]**

  확장 SMPP 커넥터에서는 이러한 필드를 무시합니다.

* **[!UICONTROL 메시지당 최대 SMS 수]**

  이 설정은 메시지 페이로드 옵션이 비활성화되어 있을 경우에만 적용됩니다(자세한 내용은 외부 계정 설정 참조). 메시지에 이 값보다 많은 SMS가 필요한 경우 오류가 트리거됩니다.

  SMS 프로토콜을 통해 메시지를 최대 255개의 부분으로 분할할 수 있지만 일부 모바일 장치는 10개 이상의 부분으로 메시지를 다시 어셈블하기 어려울 수 있습니다(제한은 장치 모델에 따라 다름). 안정성을 위해서는 메시지를 5부분 이하로 제한하는 것이 가장 좋습니다.

  Adobe Campaign에서 개인화된 메시지가 작동하는 방식으로 인해 메시지 크기가 달라질 수 있습니다. 긴 메시지 수가 많으면 전송 비용이 증가할 수 있으므로 적절한 한도를 사용하면 비용 관리에 도움이 됩니다.

  이 값을 0으로 설정하면 제한이 비활성화됩니다.

## 이메일 게재를 위한 SMTP 설정 {#smtp}

>[!CONTEXTUALHELP]
>id="acw_email_settings_smtp"
>title="SMTP 매개변수"
>abstract="이메일 게재에 추가 SMTP 매개변수를 추가할 수 있습니다."

전자 메일 게재에 추가 SMTP 매개 변수를 추가할 수 있습니다. 게재 설정의 SMTP 탭에서 수행할 수 있습니다.

![](assets/smtp_tab.png){zoomable="yes"}

### 문자 인코딩 {#character-encoding}

**[!UICONTROL 문자 인코딩]** 섹션에서 특정 인코딩을 설정할 수 있습니다. 기본 인코딩은 대부분의 문자에 작동하는 UTF-8입니다. 그러나 일부 이메일 공급자가 UTF-8 표준 인코딩을 지원하지 않는 경우 특수 문자를 올바르게 표시하지 않을 수 있습니다.

예를 들어, 일본어 문자가 포함된 이메일을 보내려면 해당 문자를 구체적으로 지원하는 인코딩을 사용하는 것이 좋습니다. 그러면 일본에 있는 대상자가 모든 문자를 올바르게 볼 수 있습니다.

이렇게 하려면 **[!UICONTROL 메시지에 사용된 인코딩 강제 적용]** 토글을 활성화하고 특수 문자를 지원하는 목록에서 올바른 인코딩을 선택합니다.

![](assets/smtp_encoding.png){zoomable="yes"}

### 바운스 이메일 {#bounce-emails}

게재 설정의 **[!UICONTROL SMTP]** 탭을 사용하면 바운스 메일 관리도 구성할 수 있습니다.

* **[!UICONTROL 오류 수신 주소]**: **[!UICONTROL 플랫폼에 대해 정의된 기본 오류 주소를 사용]** 전환을 활성화하면 반송된 전자 메일이 플랫폼의 기본 오류 상자에서 수신됩니다. 활성화하지 않으면 게재에 대한 특정 오류 주소를 정의할 수 있습니다.

* **[!UICONTROL 바운스 주소]**: 처리되지 않은 반송된 전자 메일이 전달되는 다른 주소를 정의할 수도 있습니다. 이 주소를 사용하면 애플리케이션에서 이메일을 자동으로 검증할 수 없을 때 반송 원인을 조사할 수 있습니다.

이 두 필드는 [이 섹션](../personalization/gs-personalization.md)에 설명된 대로 개인화할 수 있습니다.

![](assets/smtp_bounce.png){zoomable="yes"}

### 추가 SMTP 헤더 {#smtp-headers}

게재 설정의 SMTP 탭에서 전자 메일 게재에 **[!UICONTROL SMTP 헤더]**&#x200B;를 추가할 수 있습니다.

이 창에 입력한 스크립트는 줄당 name:value 형식으로 한 개의 헤더를 참조해야 합니다.

필요한 경우 값이 자동으로 인코딩됩니다.

![](assets/smtp_headers.png){zoomable="yes"}


>[!IMPORTANT]
>
>추가 SMTP 헤더 삽입을 위한 스크립트 추가는 고급 사용자를 위해 예약되어 있습니다. 이 스크립트의 구문은 다음과 같은 이 콘텐츠 형식의 요구 사항을 준수해야 합니다: 사용하지 않은 공간, 빈 줄 등이 없음.

## 변수 추가 {#variables-delivery}

>[!CONTEXTUALHELP]
>id="acw_delivery_settings_variable"
>title="변수"
>abstract="게재에 변수를 추가할 수 있으며, 이는 추적 및 개인화에 유용할 수 있습니다. 이러한 변수는 게재 콘텐츠와 워크플로 모두에서 액세스할 수 있습니다."

게재에 변수를 추가할 수 있으며, 이는 추적 및 개인화에 유용할 수 있습니다. 이러한 변수는 게재 콘텐츠와 워크플로우 모두에서 액세스할 수 있습니다. 저장된 변수는 게재 내의 모든 메시지에서 일정하게 유지되는 값을 설정하는 데 사용됩니다. 게재 템플릿에서도 구성할 수 있습니다.

변수를 추가하려면 아래와 같이 **[!UICONTROL 변수]** 탭으로 이동하십시오.

![](assets/variables-tab.png){zoomable="yes"}

변수의 세부 정보를 입력하려면 **[!UICONTROL 변수 추가]** 단추를 클릭하십시오. **[!UICONTROL 값이 식의 결과임]** 확인란을 활성화하여 값을 직접 추가하거나 식을 사용할 수 있습니다. **[!UICONTROL 확인]**&#x200B;을 클릭하여 변경 내용을 저장합니다.

![](assets/variables-add.png){zoomable="yes"}

[개인화에 변수 사용](../personalization/personalize.md#variables-personalization) 및 [다이내믹 컨텐츠에 변수 사용](../personalization/conditions.md#variables-conditional)에 대해 자세히 알아보세요.