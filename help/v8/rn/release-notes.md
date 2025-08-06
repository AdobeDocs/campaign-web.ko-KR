---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [2024](release-notes-24.md) 및 [2025](release-notes-25.md) 페이지에 나열되어 있습니다.

## 2025년 7월 릴리스 {#25-7-release}

### 새로운 기능 {#25-7-features}

7월 릴리스부터 다음과 같은 기능을 사용할 수 있습니다.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>이메일 디자이너에서 사용자 정의 CSS 지원</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이메일을 디자인할 때 이제 이메일 디자이너 내에서 직접 사용자 정의 CSS를 추가할 수 있습니다. 이 기능을 사용하면 고급 및 특정 스타일을 적용하여 콘텐츠의 유연성을 높이고 외관을 제어할 수 있습니다.</p>
<p>자세한 내용은 <a href="../email/custom-css.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>브랜드</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 커뮤니케이션 전반에 걸쳐 시각적, 언어적 정체성을 명확하게 정의하기 위해 자체 브랜드를 만들고 사용자 정의할 수 있습니다. 브랜드 정렬 점수를 사용하면 콘텐츠가 브랜드의 톤, 스타일, 가이드라인을 얼마나 잘 반영하는지에 대한 실시간 피드백을 받을 수 있으므로 보내는 모든 메시지에서 일관되게 브랜드에 맞는 내용을 전달하는 데 도움이 됩니다.
</p>
<p>자세한 내용은 <a href="../content/brands.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>게재 알림</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>게재 알림 기능은 사용자 그룹이 게재 실행에 대한 정보가 포함된 알림을 자동으로 수신할 수 있는 알림 관리 시스템입니다.</p>
<p>자세한 내용은 <a href="../msg/delivery-alerting.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>동적 보고</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 마케팅 활동의 영향을 측정하기 위해 완전히 사용자 정의 가능한 실시간 보고서를 제공하는 동적 보고 기능을 이용할 수 있습니다. 이 기능은 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 기능적 이메일 캠페인 데이터 외에도 성별, 도시, 연령과 같은 프로필 차원별로 인구통계 분석을 지원합니다. 다국어 이메일 게재 및 트랜잭션 메시지에 대한 동적 보고 기능도 제공됩니다.</p>
<p>이 기능은 온디맨드로만 사용할 수 있습니다. 액세스 권한을 받으려면 Adobe 담당자에게 문의하십시오. 서버를 최소 8.8.1로 업그레이드해야 합니다. 클라이언트 콘솔 <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">릴리스 정보</a>를 참조하십시오.
<p>자세한 내용은 <a href="../reporting/dynamic-reporting/get-started-reporting.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>중앙 집중식 브랜딩</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 기술 관리자는 브랜드의 정체성에 영향을 미치는 매개변수를 중앙 집중식으로 정의할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. SMS 및 다이렉트 메일을 포함한 모든 채널에 대해 브랜딩 옵션을 사용할 수 있습니다.</p>
<p>이 기능은 새로운 구현에 대해서만 온디맨드로 제공됩니다. 액세스 권한을 받으려면 Adobe 담당자에게 문의하십시오. 서버를 최소 8.8.1로 업그레이드해야 합니다. 클라이언트 콘솔 <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">릴리스 정보</a>를 참조하십시오.
<p>자세한 내용은 <a href="../administration/branding/branding-gs.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

위에 나열된 기능 외에도 이번 릴리스에는 클라이언트 콘솔에서 사용할 수 있는 다음과 같은 기능 세트가 함께 제공됩니다.

* [새로운 SMS 전송 커넥터](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA 환경)
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (온디맨드, FDA 환경)

클라이언트 콘솔 [릴리스 정보](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}를 참조하십시오.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

-->

### 개선 사항 {#25-7-improvements}

* 이제 규칙 빌더에서 각 조건 및 그룹에 대한 대상 모집단을 직접 계산할 수 있습니다. 결과 번호를 클릭하면 자세한 기록 목록을 볼 수 있습니다. [자세히 알아보기](../query/build-query.md#validate-query)

* 이제 규칙 빌더에서 미리 정의된 필터를 직접 편집하거나 삭제할 수 있습니다. [자세히 알아보기](../get-started/predefined-filters.md#manage-predefined-filter)

* 이제 SMS 게재를 구성할 때 **SMS** 섹션에서 **선택적 SMPP 매개변수(TLV)**&#x200B;에 액세스할 수 있습니다. 이 매개변수는 클라이언트 콘솔에서의 매개변수와 동일합니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#sms-tab)

* 이제 iOS 콘텐츠 에디션 화면의 **고급 설정** 섹션에서 제공되는 새로운 **콘텐츠 사용 가능** 옵션을 사용하여 iOS에서 백그라운드 알림을 활성화할 수 있습니다. 이렇게 하면 `aps` 페이로드에 `content-available:1` 플래그가 추가됩니다. [이 페이지](../push/content-push.md)에서 자세히 알아보십시오. [이 페이지](../push/rich-push-ios.md)도 참조하십시오.

* 이제 다음과 같은 랜딩 페이지 개선 사항을 이용할 수 있습니다.

   * 이제 서비스를 구성할 때 기본 구독/구독 취소 랜딩 페이지를 참조할 수 있습니다. 이메일을 설계할 때 해당 랜딩 페이지에 대한 링크를 정의하면 랜딩 페이지 양식을 제출하는 사용자는 자동으로 이 서비스에 구독하거나 구독 취소됩니다. [자세히 보기](../audience/manage-services.md#create-service)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 익명의 방문자가 랜딩 페이지에 액세스할 수 있습니다. 이 옵션을 선택 취소하면 식별된 사용자만 양식에 액세스하여 제출할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 랜딩 페이지가 제출될 때 추가 내부 데이터를 저장할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 새로운 옵션을 사용하면 여러 서비스에 랜딩 페이지를 사용할 수 있으므로 동적으로 변경할 수 있습니다. 이메일에 링크를 추가할 때 동적 랜딩 페이지를 선택하면 모든 서비스를 선택할 수 있습니다. 특정 서비스가 연결된 랜딩 페이지를 선택하면 해당 서비스가 자동으로 사용됩니다(다른 서비스를 선택할 수 없음). [자세히 보기](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 이제 랜딩 페이지에서 조건부 콘텐츠가 지원됩니다. [자세히 보기](../landing-pages/lp-content.md)
   * 랜딩 페이지를 서비스에 연결하고, 사용자가 해당 랜딩 페이지를 검증할 때 확인 메시지를 보낼 수 있습니다. [자세히 알아보기](../landing-pages/lp-content.md#lp-message)
   * 봇으로 인한 스팸과 남용으로부터 랜딩 페이지를 보호하기 위해 Captcha를 추가할 수 있습니다. 이는 고객과의 상호 작용이 필요하지 않고 사이트와의 상호 작용을 기반으로 하기 때문에 고객을 방해하지 않습니다. [자세히 알아보기](../landing-pages/create-lp.md#captcha)
