---
title: Campaign v8 Web 사용자 인터페이스 이전 릴리스 정보
description: 2025 Campaign Web 사용자 인터페이스 릴리스
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 875e60defa2d96a6d7b3663516b757f3cc8cd154
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 100%

---

# 2025 릴리스 정보 {#2025-release}

이 페이지에는 **2025년 릴리스**&#x200B;를 통해 이용할 수 있는 모든 변경 사항과 개선 사항이 나열되어 있습니다. 최신 릴리스 정보는 [이 페이지](release-notes.md)에서 확인할 수 있습니다.

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
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko" target="_blank">release notes</a>.
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
<p>이 기능은 온디맨드로만 사용할 수 있습니다. 액세스 권한을 받으려면 Adobe 담당자에게 문의하십시오. 서버를 최소 8.8.1로 업그레이드해야 합니다. 클라이언트 콘솔 <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko" target="_blank">릴리스 정보</a>를 참조하십시오.
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
<p>이 기능은 새로운 구현에 대해서만 온디맨드로 제공됩니다. 액세스 권한을 받으려면 Adobe 담당자에게 문의하십시오. 서버를 최소 8.8.1로 업그레이드해야 합니다. 클라이언트 콘솔 <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko" target="_blank">릴리스 정보</a>를 참조하십시오.
<p>자세한 내용은 <a href="../administration/branding/branding-gs.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

위에 나열된 기능 외에도 이번 릴리스에는 클라이언트 콘솔에서 사용할 수 있는 다음과 같은 기능 세트가 함께 제공됩니다.

* [새로운 SMS 전송 커넥터](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=ko) (FDA 환경)
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ko) (온디맨드, FDA 환경)

클라이언트 콘솔 [릴리스 정보](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko){target="_blank"}를 참조하십시오.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=ko){target="_blank"}

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

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=ko) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ko) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ko){target="_blank"}.

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

## 2025년 6월 릴리스 {#25-6-release}

### 개선 사항 {#25-6-improvements}

* 이제 콜센터와 사용자 정의 채널 모두에 대한 게재 요약 보고서를 사용할 수 있습니다. [자세히 알아보기](../reporting/direct-mail.md)

* SMS 게재를 구성할 때 이제 특정 SMS 매개변수에 액세스할 수 있습니다. 이는 클라이언트 콘솔에서 사용할 수 있는 매개변수와 동일합니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#sms-tab)

* 이제 자주 사용하는 폴더가 탐색기 페이지의 왼쪽 패널 상단에 표시되어 간편하게 액세스할 수 있습니다. [자세히 알아보기](../get-started/work-with-folders.md#favorite-folders)

* 이제 규칙 빌더가 드래그 앤 드롭을 지원하여 쿼리 구성 요소를 더 효율적으로 재정렬할 수 있습니다. [자세히 알아보기](../query/build-query.md#drag-and-drop)

* 규칙 빌더의 “인간 조건”이 개선되었습니다. 화면 하단에 표시되는 규칙의 작성된 일반 언어 버전은 다음과 같습니다.

   * 속성이 이제 강조 표시되고 연관된 스키마가 표시됩니다.
   * 이들 요소를 클릭하면 더 자세한 정보를 볼 수 있습니다.
   * 이제 해당 버튼을 사용하여 인간 조건을 복사할 수 있습니다.

* 이제 “기술 워크플로” 및 “자동으로 생성된 오브젝트” 폴더에 대한 액세스가 제한되어 이들 폴더를 볼 수 없습니다. [자세히 알아보기](../get-started/work-with-folders.md#about-folders)

## 2025년 5월 릴리스 {#25-5-release}

다음 기능은 5월 릴리스 이후 모든 사용자가 사용할 수 있습니다.

<table>
<thead>
<tr>
<th><strong>브랜드 정렬 점수 (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>브랜드 정렬 점수 기능은 이메일 디자이너에서 직접 명확한 피드백을 제공하여 내 콘텐츠가 브랜드의 톤, 스타일 및 가이드라인에 부합하는지 확인하는 데 도움을 줍니다. 이 기능은 Beta 버전으로 사용할 수 있습니다.</p>
<p>자세한 내용은 <a href="../content/brands-score.md">세부 설명서</a>를 참조하십시오.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>외부 게재를 위한 사용자 정의 채널</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web UI에서 직접 사용자 정의 외부 채널을 기반으로 게재를 조율하고 실행할 수 있습니다. 이들 게재는 독립적으로 실행하거나 워크플로의 일부로 실행할 수도 있습니다. 서드파티와 통합된 사용자 정의 외부 채널의 생성은 콘솔에서 수행됩니다.</p>
<p>참고: 사용자 정의 채널의 경우 Web UI에서 보고 기능을 사용할 수 없습니다. 보고서에 액세스하려면 클라이언트 콘솔로 이동해야 합니다.</p>
<p>자세한 내용은 <a href="../call-center/gs-custom-channel.md">세부 설명서</a>를 참조하십시오.</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#25-5-improvements}

유형화 규칙 생성 화면이 업데이트되어 규칙 유형을 더 쉽게 선택할 수 있게 되었습니다.

## 2025년 4월 릴리스 {#25-4-release}

**릴리스 일자**: 2025년 4월 29일

### 새로운 기능 {#25-4-features}

다음 기능은 4월 릴리스 이후 모든 사용자가 사용할 수 있습니다.

<table>
<thead>
<tr>
<th><strong>콜센터 채널</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign Web 사용자 인터페이스에서 콜센터 채널을 사용할 수 있습니다. 이 채널은 콜센터를 통해 처리되는 커뮤니케이션 또는 상호 작용을 관리하고 추적하는 데 사용되는 커뮤니케이션 방식을 의미합니다. 일반적으로 상담원이 고객이나 잠재 고객에게 전화를 거는 경우에 사용됩니다.</p>
<p>참고: 콜센터 채널의 경우 Web UI에서 보고 기능을 사용할 수 없습니다. 보고서에 액세스하려면 클라이언트 콘솔로 이동해야 합니다.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>자세한 내용은 <a href="../call-center/gs-call-center.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>새로운 규칙 빌더</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 개선된 사용자 인터페이스에서 복잡한 조건을 정의하는 데 도움이 되는 새로운 규칙 작성기를 사용할 수 있습니다. 필요에 따라 이전 규칙 빌더에서 새로운 규칙 빌더로 전환할 수 있습니다.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>자세한 내용은 <a href="../query/query-modeler-overview.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>외부 계정 작성</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>캠페인 관리자는 이제 Campaign Web 사용자 인터페이스에서 외부 시스템과의 새로운 연결을 설정할 수 있습니다.
기존 외부 계정을 보고, 업데이트하고, 관리할 수도 있습니다.</p>
<p>자세한 내용은 <a href="../administration/external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

### 개선 사항 {#25-4-improvements}

**일반 인터페이스 개선**

* 이제 사용자 인터페이스에서 스키마 속성에 대한 필드 설명, 즐겨찾기에 추가 및 값 분포 옵션을 더 쉽게 확인할 수 있습니다. 자세한 내용은 [세부 설명서](../get-started/attributes.md)를 참조하십시오.
* 이제 인터페이스에서 날짜와 시간이 Experience League 환경 설정에서 설정된 기본 언어에 따라 표시됩니다. 이 개선 사항은 몇몇 언어에만 적용됩니다. 지원되는 언어의 전체 목록을 보려면 [세부 설명서](https://experienceleague.adobe.com/ko/docs/core-services/interface/features/browser-language){target=_blank}를 참조하십시오.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**이메일 편집기**: 이제 Campaign Web UI의 접근성을 높이기 위해 이메일 디자이너에서 두 개의 새로운 필드를 사용할 수 있습니다. 이 필드는 이메일 콘텐츠의 `title` 요소와 `html` 요소의 언어 속성에 해당합니다. 이러한 설정은 이메일 본문 섹션에서 프리헤더 필드 외에도 정의할 수 있습니다. 자세한 내용은 [세부 설명서](../email/metadata.md)를 참조하십시오.

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**스키마**

* 이제 Campaign Web 사용자 인터페이스에서 목록의 임시 스키마를 편집할 수 있습니다. 자세한 내용은 [세부 설명서](../audience/manage-audience.md)를 참조하십시오.
* 이제 샘플 화면에서 스키마의 사용자 정의 필드를 미리 볼 수 있습니다. 자세한 내용은 [세부 설명서](../administration/custom-fields.md#add)를 참조하십시오.
* 이제 끌어다 놓기로 목록에서 사용자 정의 필드를 이동할 수 있습니다. 자세한 내용은 [세부 설명서](../administration/custom-fields.md#add)를 참조하십시오.


### 제한적으로 사용 가능한 새로운 기능 {#25-4-features-la}

>[!AVAILABILITY]
>
>다음 기능은 제한 공개(LA)로 제공됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8로** 마이그레이션하는 고객으로 제한되며 다른 환경에는 배포할 수 없습니다. 해당 고객은 Campaign 서버를 v8.7.4로 업그레이드해야 합니다.
>
>[Campaign Standard에서 Campaign v8로의 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ko) 설명서 페이지를 참조하십시오.

* **다국어 게재 생성** - 이제 Adobe Campaign Web 사용자 인터페이스에서 다양한 언어로 여러 이메일 게재를 전송할 수 있습니다. 다국어 게재 기능을 사용하면 게재의 기본 언어는 물론, 게재를 전송할 수 있는 다양한 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다. 자세한 내용은 [세부 설명서](../email/edit-content.md)를 참조하십시오.

* **다국어를 위한 동적 보고** - 이제 다국어 이메일 게재에 대해 동적 보고가 가능합니다. 자세한 내용은 [세부 설명서](../reporting/global-reports.md)를 참조하십시오.

* **SMS REST API 지원(LA)** - 이제 SMS 채널에서 트랜잭션 메시지 REST API를 사용할 수 있습니다. 페이로드에 이메일과 휴대폰이 모두 있는 경우 “wishedChannel” 필드를 사용하여 채널을 지정할 수 있습니다. 제공되지 않으면 wishedChannel에서 SMS를 명시적으로 요청하지 않는 한 기본적으로 이메일이 사용됩니다. 자세한 내용은 [세부 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ko){target=_blank}를 참조하십시오.

## 2025년 2월 릴리스 {#25-2-release}

**릴리스 일자**: 2025년 2월 18일

2월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

### 기능 {#25-2-features}

<table>
<thead>
<tr>
<th><strong>비즈니스 규칙(유형화 규칙) 만들기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 유형화 및 유형화 규칙을 만들 수 있습니다. 유형화를 통해 게재 전송을 제어, 필터링 및 모니터링할 수 있습니다. 유형화는 게재에 항상 필수 구성 요소(예: 구독 취소 링크 또는 제목 줄) 또는 그룹(예: 구독 취소자, 경쟁 업체 또는 충성도가 낮은 고객)을 대상자에서 제외하기 위한 필터링 규칙이 포함되어 있는지 확인하는 데 사용됩니다.</p>
<img src="assets/do-not-localize/typology.gif">
<p>자세한 내용은 <a href="../administration/typologies.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>대상 매핑</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign Web 사용자 인터페이스에서 대상 매핑을 만들 수 있습니다. 대상 매핑은 다양한 게재 채널(이메일, SMS, 푸시 알림)이 스키마의 데이터 필드에 연결되는 방식을 정의합니다. 대상 매핑을 통해 프로필, 약정 수혜자, 운영자, 구독자, 잠재 고객 등 타기팅되는 대상자를 정의할 수 있습니다.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>자세한 내용은 <a href="../administration/target-mappings.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>스키마 세부 정보</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 목록에서 스키마 이름을 선택하여 스키마의 세부 정보에 액세스할 수 있습니다. 이제 스키마 세부 정보에 표시되는 <b>사용자 정의 필드 편집</b> 버튼을 사용하여 사용자 정의 필드 편집 기능에 액세스할 수 있습니다.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>자세한 내용은 <a href="../administration/schemas.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

## 2025년 1월 릴리스 {#25-1-release}

**릴리스 일자**: 2025년 2월 5일

1월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

### 기능 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>시각적 조각 만들기 및 사용하기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>시각적 조각은 여러 이메일 게재 또는 콘텐츠 템플릿에서 재사용할 수 있는 사전 정의된 시각적 블록입니다. 이 기능은 이제 서버 빌드 8.6.4 이상을 실행하는 모든 고객이 사용할 수 있습니다.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>자세한 내용은 <a href="../content/use-visual-fragments.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>서드파티 시스템을 사용하여 게재 전송</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign 웹 인터페이스에서 외부 게재와 외부 게재 템플릿을 정의할 수 있습니다. 이 모드에서는 메시지가 출력 파일에 컴파일되어 외부 공급자와 공유할 수 있습니다. 기본적으로 외부 게재 모드는 다이렉트 메일(DM) 채널에 사용됩니다.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>자세한 내용은 <a href="../msg/send-external-deliveries.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>열거 관리</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스를 통해 직접 열거를 만들 수 있습니다. 열거는 필드를 채우기 위해 시스템이 제안하는 값의 목록입니다. 열거를 사용하여 이러한 필드의 값을 표준화하고, 쿼리 내에서 데이터 입력이나 사용을 돕습니다.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>자세한 내용은 <a href="../administration/enumerations.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>사용자 정의 옵션 만들기</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 기술 옵션에 액세스하여 요구 사항에 맞는 사용자 정의 옵션을 직접 만들 수 있습니다. 이 기능은 특히 중간 데이터를 저장하기 위해 JavaScript 코드 워크플로 활동을 수행할 때 유용합니다.</p>
<img src="assets/do-not-localize/options.gif">
<p>자세한 내용은 <a href="../administration/options.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>JavaScript 코드 정의 및 호출</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 JavaScript 코드를 만들 수 있습니다. 이를 통해 라이브러리처럼 여러 워크플로에서 활용할 수 있는 재사용 가능한 함수를 만들 수 있습니다.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>자세한 내용은 <a href="../administration/javascript-codes.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>AI 어시스턴트를 사용하여 랜딩 페이지 생성</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 AI 어시스턴트를 랜딩 페이지 게재에 사용할 수 있으며 이를 통해 텍스트, 이미지 또는 전체 페이지 레이아웃을 생성할 수 있습니다.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>AI 어시스턴트에 대한 자세한 내용은 <a href="../email/generative-lp.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


### 개선 사항 {#25-1-improvements}

* 인터페이스에서 사용자 정의 필드의 표시 사용자 정의:

   * 이제 인터페이스에서 표시할 추가 사용자 정의 필드를 선택할 수 있습니다.
   * 이제 다른 필드의 입력에 따라 목록 값을 제한하는 것과 같이 링크 유형 사용자 정의 필드를 표시하기 위한 규칙을 설정할 수 있습니다.
   * 이제 인터페이스에서 필드를 보다 유연하게 배열할 수 있습니다. 필드를 단일 열에 걸쳐 배치하거나 더 나은 구성을 위해 하위 섹션으로 그룹화할 수 있습니다.
   * 이제 특정 필드를 읽기 전용으로 설정할 수 있습니다.

* 최근 항목 및 즐겨찾기 필터: 자주 사용되는 속성을 빠르게 재사용하기 위해 이제 이를 즐겨찾기에 추가할 수 있습니다. 이렇게 하면 향후 작업에 간편하게 액세스할 수 있습니다. 즐겨찾기 외에도 가장 최근에 선택한 속성을 조회하고 사용할 수 있습니다.

* 외부 계정: 외부 계정을 새로 만들 때 새로운 **[!UICONTROL 라우팅]** 유형을 사용할 수 있습니다. 이렇게 하면 외부 게재에 사용할 특정 외부 계정을 구성할 수 있습니다. [자세히 알아보기](../administration/external-account.md#routing)
