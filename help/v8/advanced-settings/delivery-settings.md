---
audience: end-user
title: 게재 설정
description: Campaign 웹에서 게재 설정에 대해 자세히 알아보기
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="제한 공개"
source-git-commit: 96aec85933a47c1289549ba0696874a5f82e7fd5
workflow-type: tm+mt
source-wordcount: '2316'
ht-degree: 58%

---


# 이메일 게재 설정 {#email-del-settings}

이메일 게재 설정은 다음과 같습니다. **기술 게재 매개 변수** 이메일 템플릿에 정의되어 있습니다. 각 게재에 대해 오버로드될 수 있습니다.

이러한 설정은 다음에서 사용할 수 있습니다. **설정** 버튼 이메일 게재 또는 이메일 게재 템플릿을 편집할 때 사용할 수 있습니다.

## 이메일 게재 설정 {#email-delivery-settings}

>[!CAUTION]
>
>이러한 설정은 정보 목적으로만 설명됩니다. 그 중 일부는 구성 및 권한에 따라 다릅니다. 이 버전의 제품에서는 수정할 수 없습니다.

## 유형화 설정 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="유형화"
>abstract="유형화 규칙을 통해 마케터는 모든 게재에 걸쳐 비즈니스 사례를 표준화할 수 있습니다. 유형화는 게재 전송에 대해 제어, 필터링 및 우선 순위 지정을 수행할 수 있는 유형화 규칙 모음입니다. 유형화 규칙 내의 기준과 일치하는 프로필은 준비 단계에 게재 대상자에서 제외됩니다. 유형화 및 유형화 규칙은 Campaign 클라이언트 콘솔에서 만들어집니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="게재에 대한 유형화 설정"
>abstract="유형화 규칙을 통해 마케터는 모든 게재에 걸쳐 비즈니스 사례를 표준화할 수 있습니다. 유형화는 게재 전송에 대해 제어, 필터링 및 우선 순위 지정을 수행할 수 있는 유형화 규칙 모음입니다. 유형화 규칙 내의 기준과 일치하는 프로필은 준비 단계에 게재 대상자에서 제외됩니다. 유형화 및 유형화 규칙은 Campaign 클라이언트 콘솔에서 만들어집니다."


유형화는 다음 집합입니다. **유형화 규칙** 여러 필터링 규칙을 한 번에 쉽게 게재에 적용하기 위해 준비 단계 중에 실행됩니다. 이를 통해 마케터는 게재 전송을 제어, 필터링 및 우선 순위를 지정할 수 있으므로 모든 게재에서 비즈니스 사례를 표준화할 수 있습니다.

유형화를 메시지 또는 메시지 템플릿과 연결하면 해당 유형화에 포함된 유형화 규칙이 실행되어 메시지를 준비하는 동안 게재 유효성을 검사합니다. 그러면 유형화 규칙 내의 기준과 일치하는 프로필은 게재 대상자에서 제외됩니다.

유형화를 사용하면 이메일에 항상 특정 요소(예: 구독 취소 링크 또는 제목 줄)가 포함되어 있는지 확인하거나 그룹을 의도한 타겟(구독 취소자, 경쟁 업체 또는 비충성 고객)에서 제외하는 필터링 규칙이 있는지 확인할 수 있습니다.

![](assets/delivery-settings-typology.png)

>[!NOTE]
>
>유형화 및 유형화 규칙은 Campaign 클라이언트 콘솔에서 만들어집니다. 압력 규칙 및 의 피로도 관리 구성 방법에 대해 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=ko){target="_blank"}.

### 압력 매개변수 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="게재에 대한 압력 매개변수"
>abstract="게재 가중치를 통해 피로도 관리 프레임워크 내에서 최우선 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선 순위가 높습니다."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="게재 가중치"
>abstract="게재 가중치를 통해 압력 관리 프레임워크 내에서 최우선 게재를 식별할 수 있습니다. 가중치가 가장 높은 메시지는 우선 순위가 높습니다."

이 섹션에서 압력 매개 변수를 사용하여 **임계값** 지정된 기간 동안 하나의 프로필에 보낼 수 있는 최대 메시지 수인 피로도 관리 규칙을 설정합니다.

이 임계값에 도달하면 고려된 기간이 끝날 때까지 더 이상 게재할 수 없습니다. 이 프로세스를 사용하면 메시지가 설정된 임계값을 초과하는 경우 게재 시 프로필을 자동으로 제외하여 과도한 요청을 방지할 수 있습니다.

임계값은 상수 또는 변수일 수 있습니다. 즉, 특정 기간 동안 임계값은 프로필마다 또는 심지어 동일한 프로필에 대해서도 다를 수 있습니다.

**[!UICONTROL 가중치 유형]** 필드에서 다음 세 가지 옵션을 사용할 수 있습니다.

* **[!UICONTROL 일정]**
* **[!UICONTROL 수신자에 따라 다름]**
* **[!UICONTROL 각 규칙에 정의됨]**

**[!UICONTROL 게재 가중치]** 필드를 사용하여 게재 우선 순위를 정의합니다. 각 게재에는 우선 순위 수준을 나타내는 가중치가 있습니다. 기본적으로 게재 가중치는 5로 설정되어 있습니다. 압력 규칙을 사용하면 적용되는 게재의 가중치를 정의할 수 있습니다. 가중치는 수신자에 맞게 공식을 통해 설정하거나 계산할 수 있습니다. 예를 들어 수신자의 관심사에 따라 게재 가중치를 정의할 수 있습니다.

대상 평가 모드를 선택하려면 **[!UICONTROL 게재 모드]**&#x200B;를 사용합니다. 다음 세 가지 모드를 사용할 수 있습니다.

* **[!UICONTROL 대상 예상 및 메시지 개인화]**
* **[!UICONTROL 잠정 대상 예상 및 승인]**
* **[!UICONTROL 대상 평가]**

>[!NOTE]
>
>피로도 관리는 Campaign 클라이언트 콘솔에서 구성됩니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### 수용작업량 설정 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="게재에 대한 수용작업량 설정"
>abstract="메시지를 게재하기 전에 수용작업량 규칙을 사용하여 조직이 게재, 게재로 인해 생성될 수 있는 인바운드 메시지와 구독자에게 문의할 수 있는 통화 수를 처리할 수 있는지 확인합니다. 수용작업량 규칙은 Adobe Campaign v8 콘솔에 정의되어 있습니다. 이 화면에서 이메일 채널과 연계된 규칙을 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="수신자 중요도"
>abstract="수신자 중요도는 용량 유형화 규칙 초과 시 유지되는 수신자를 결정하는 데 사용되는 공식입니다."


이 섹션에서는 Adobe Campaign v8 콘솔에 정의된 용량 규칙을 선택할 수 있습니다. 이 규칙은 이메일 채널과 연결되어 있습니다.

다음 **[!UICONTROL 수신자의 중요도]** 필드는 용량 유형화 규칙을 초과할 때 어떤 수신자를 유지할지 결정하는 데 사용되는 수식입니다.

>[!NOTE]
>
>유형화 규칙은 Campaign 클라이언트 콘솔에 구성됩니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.

## 대상자 설정 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="게재에 대한 대상자 설정"
>abstract="사용 가능한 **대상 매핑** 중 원하는 옵션을 선택합니다. 대상 매핑은 Adobe Campaign v8 콘솔에서 정의됩니다. 게재에 대한 제외 매개변수를 설정할 수도 있습니다. "

이 섹션에서는 사용 가능한 **대상 매핑** 중 원하는 옵션을 선택할 수 있습니다. 대상 매핑은 Adobe Campaign v8 콘솔에서 정의됩니다. 대상 매핑은 작업에서 처리하는 데이터 유형입니다. 대상 모집단(수신자, 계약 수혜자, 운영자, 구독자 등)을 정의할 수 있습니다.

다음에서 대상 매핑에 대해 자세히 알아보기: [이 섹션](../audience/targeting-dimensions.md).

다음에서 **[!UICONTROL 제외]** 필드에서는 더 이상 연락을 원치 않거나 격리된 수신자를 제외하도록 선택할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## 게재 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="게재에 대한 게재 설정"
>abstract="게재 매개변수는 게재에 적용되는 기술 설정입니다. 게재를 위한 BCC를 활성화하고 게재 및 일반 모드를 변경할 수 있습니다. 이 옵션은 숙련된 사용자로만 제한됩니다."

**[!UICONTROL 게재]** 매개 변수는 게재에 적용되는 기술 설정입니다.

통합 이메일 **[!UICONTROL 라우팅]** 기본적으로 외부 계정이 제공됩니다. 애플리케이션이 이메일을 전송할 수 있는 기술 매개변수가 포함되어 있습니다.

다음을 정의할 수 있습니다 **[!UICONTROL 전송 중]** 설정:

* **[!UICONTROL SMTP 게재 테스트]**: 이 옵션은 SMTP를 통한 전송을 테스트하는 데 사용됩니다. 게재는 SMTP 서버에 연결될 때까지 처리되지만 전송되지는 않습니다. 게재의 모든 수신자에 대해 Campaign은 SMTP 공급자 서버에 연결하고 SMTP RCPT TO 명령을 실행한 다음 SMTP DATA 명령 전에 연결을 종료합니다.

* **[!UICONTROL 이메일 BCC]**: 이 옵션은 메시지 대상에 BCC 이메일 주소를 추가하여 BCC를 통해 외부 시스템에 이메일을 저장하는 데 사용됩니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

* **[!UICONTROL 여러 웨이브를 사용하여 보내기]**: 웨이브를 사용하여 전송되는 볼륨을 점진적으로 늘릴 수 있습니다. 이렇게 하면 메시지가 스팸으로 표시되거나 하루에 메시지 수를 제한하려는 경우를 방지할 수 있습니다. 웨이브를 사용하여 동시에 대량의 메시지를 전송하는 대신 게재를 여러 배치로 나눌 수 있습니다. [자세히 알아보기](send-using-waves.md)

또한 보낸 이메일 메시지의 형식을 변경할 수 있습니다.

* **[!UICONTROL 수신자 환경 설정 사용]** (기본 모드)

  메시지 형식은 수신자 프로필에 저장된 데이터에 따라 정의됩니다. 수신자가 특정 형식으로 메시지를 수신하려는 경우에 보내는 형식입니다. 필드를 입력하지 않으면 다중 파트 대체 메시지가 전송됩니다(아래 참조).

* **[!UICONTROL 수신자 메일 클라이언트가 가장 적절한 형식을 선택하도록 허용]**

  메시지에는 텍스트 및 HTML 두 가지 형식이 모두 포함되어 있습니다. 수신에 표시되는 형식은 수신자의 메일 소프트웨어(다중 파트 대체)의 구성에 따라 다릅니다.

  >[!IMPORTANT]
  >
  >이 옵션에는 문서의 두 버전이 모두 포함됩니다. 따라서 메시지 크기가 더 크기 때문에 게재 속도에 영향을 줍니다.

* **[!UICONTROL 모든 메시지를 텍스트 형식으로 보내기]**

  메시지는 텍스트 형식으로 전송됩니다. HTML 형식은 전송되지 않지만 수신자가 메시지를 클릭할 때만 미러 페이지에 사용됩니다.

## 웹 분석 {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="게재에 대한 웹 분석 설정"
>abstract="웹 분석 계정을 선택합니다. 이 계정은 Campaign 클라이언트 콘솔에서 구성됩니다. 사용 중인 분석 도구와 공유되는 태그를 정의할 수도 있습니다."

이 섹션에서 웹 분석 계정을 선택할 수 있습니다. 이 계정은 Campaign 클라이언트 콘솔에 구성됩니다.

사용 중인 분석 도구와 공유되는 태그를 정의할 수도 있습니다.

>[!NOTE]
>
>웹 분석 기능은 Campaign 클라이언트 콘솔에서 구성됩니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## 재시도 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="최대 재시도 수"
>abstract="일시적인 오류로 인해 메시지 전송이 실패하면 게재 기간이 종료될 때까지 재시도를 수행합니다."

<!--Currently not visible in UI > ??-->

소프트 또는 무시됨 오류로 인해 일시적으로 게재되지 않은 메시지는 자동 재시도의 적용을 받습니다. 기본적으로 5번의 다시 시도가 배달 첫 날에 예약되며 하루 중 24시간 동안 최소 1시간 간격으로 분산됩니다.

에서 다시 시도 관리에 대해 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 승인 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="게재 승인 모드"
>abstract="승인 모드를 선택합니다. 게재 준비 중에 경고가 생성되면 게재를 계속 실행해야 하는지 여부를 정의하도록 구성할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="게재 승인 모드"
>abstract="이 템플릿을 기반으로 게재에 대한 승인 모드를 선택합니다. 게재 준비 중에 경고가 생성되면 게재를 계속 실행해야 하는지 여부를 정의하도록 구성할 수 있습니다."

게재 준비 중에 경고가 생성되면 게재를 계속 실행해야 하는지 여부를 정의하도록 구성할 수 있습니다. 사용자는 기본적으로 분석 단계가 끝나면 메시지 전송을 확인해야 합니다. 이를 **수동** 유효성 검사라고 합니다.

적절한 필드에서 다른 승인 모드를 선택할 수 있습니다. 사용 가능한 모드는 다음과 같습니다.

* ****[!UICONTROL 수동]****: 분석 단계가 끝나면 사용자는 전송을 시작하기 위해 게재를 확인해야 합니다.

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

**[!UICONTROL 리소스 유효성 검사 제한]** 주로 미러 페이지와 이미지에 대해 업로드된 리소스에 사용됩니다. 이 페이지의 리소스는 제한된 시간 동안 유효합니다(디스크 공간을 절약하기 위함). 이 제한이 지나면 이러한 리소스를 더 이상 사용할 수 없습니다.

![](assets/delivery-settings-validity.png)

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

에서 게재 유효 기간에 대해 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 미러 페이지 관리 {#mirror}

미러 페이지는 웹 브라우저를 통해 온라인으로 액세스할 수 있는 HTML 페이지입니다. 콘텐츠는 이메일과 동일합니다. 기본적으로 링크가 메일의 콘텐츠에 삽입된 경우 미러 페이지가 생성됩니다.

기본 모드 이외에 다음 옵션도 사용할 수 있습니다.

* **[!UICONTROL 미러 페이지 강제 생성]**: 게재에 미러 페이지 링크가 삽입되지 않은 경우에도 이 모드를 사용하여 미러 페이지를 생성합니다.
* **[!UICONTROL 미러 페이지 생성 안 함]**: 링크가 게재에 있더라도 미러 페이지가 생성되지 않도록 하려면 이 모드를 사용하십시오.
* **[!UICONTROL 메시지 식별자만 사용하여 액세스할 수 있는 미러 페이지 생성]**: 이메일 콘텐츠에 미러 페이지 링크가 없는 경우 이 옵션을 사용하여 게재 로그 창에서 클라이언트 콘솔에서 미러 페이지의 콘텐츠에 액세스할 수 있도록 합니다.


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

**[!UICONTROL 추적]** 매개 변수는 관련 섹션에 정의되어 있습니다. 가능한 옵션은 다음과 같습니다.

**[!UICONTROL 추적 유효성 검사 제한]**: 이 옵션을 사용하여 URL에서 추적이 활성화되는 기간을 변경합니다.

**[!UICONTROL 만료된 URL의 대체 URL]**: 이 옵션을 사용하여 대체 웹 페이지의 URL을 입력합니다. 추적이 만료되면 표시됩니다.

## 증명 설정 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="게재에 대한 증명 설정 정의"
>abstract="제외 매개변수를 선택하고 증명의 레이블을 사용자 정의합니다."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

이 섹션에서는 제외 매개변수를 설정할 수 있습니다. 사용 가능한 옵션은 다음과 같습니다.

* ****[!UICONTROL 중복 요소 보관]**** 여러 타겟팅 기준을 충족하는 수신자에게 여러 게재를 승인할 수 있습니다.

* **[!UICONTROL 차단 목록에 추가된 주소 보관]** 옵션을 사용하면 구독 취소(옵트아웃) 후와 같이 게재에서 더 이상 대상으로 지정되지 않는 프로필을 대상에서 유지할 수 있습니다.

* **[!UICONTROL 격리된 주소 보관]** 옵션을 사용하면 주소가 응답하지 않는 프로필을 대상에서 유지할 수 있습니다.

다음과 같이 증명 레이블을 사용자 지정할 수도 있습니다.

* 사용 **[!UICONTROL 증명을 위해 게재 코드 보관]** 증명에 연결하는 데 관련된 게재에 대해 정의된 것과 동일한 게재 코드를 연결합니다.

* 기본적으로 증명 제목에는 &#39;PROOF #&#39;가 붙습니다. 여기서 #은 증명 번호입니다. 이 접두사는 **[!UICONTROL 레이블 접두사]** 필드에서 변경할 수 있습니다.