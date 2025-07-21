---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 98%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [2024](release-notes-24.md) 및 [2025](release-notes-25.md)에 나열되어 있습니다.

## 2025년 7월 업데이트 {#25-7-updates}

>[!AVAILABILITY]
>
>이번 업데이트의 혜택을 받으려면 서버를 최소 8.8.1로 업그레이드해야 합니다. 클라이언트 콘솔 [릴리스 정보](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}를 참조하십시오.

이전에는 제한적으로만 제공되던 다음과 같은 기능이 이제 모든 환경에서 사용할 수 있습니다(일반 가용성).

* **다국어 게재 생성** - 이제 Adobe Campaign Web 사용자 인터페이스에서 다양한 언어로 여러 이메일 게재를 전송할 수 있습니다. 다국어 게재 기능을 사용하면 게재의 기본 언어는 물론, 게재를 전송할 수 있는 다양한 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다. [자세히 보기](../email/edit-content.md#multilingual-delivery)

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}
-->

* **게재 경고** - 게재 경고 기능은 사용자 그룹이 게재 실행에 대한 정보가 포함된 알림을 자동으로 수신할 수 있는 경고 관리 시스템입니다. [자세히 보기](../msg/delivery-alerting.md)

* **랜딩 페이지 개선 사항** - 다음과 같은 랜딩 페이지 개선 사항이 적용되었습니다.

   * 이제 서비스를 구성할 때 기본 구독/구독 취소 랜딩 페이지를 참조할 수 있습니다. 이메일을 설계할 때 해당 랜딩 페이지에 대한 링크를 정의하면 랜딩 페이지 양식을 제출하는 사용자는 자동으로 이 서비스에 구독하거나 구독 취소됩니다. [자세히 보기](../audience/manage-services.md#create-service)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 익명의 방문자가 랜딩 페이지에 액세스할 수 있습니다. 이 옵션을 선택 취소하면 식별된 사용자만 양식에 액세스하여 제출할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 랜딩 페이지 구성의 새로운 옵션을 사용하면 랜딩 페이지가 제출될 때 추가 내부 데이터를 저장할 수 있습니다. [자세히 보기](../landing-pages/create-lp.md#create-landing-page)
   * 새로운 옵션을 사용하면 여러 서비스에 랜딩 페이지를 사용할 수 있으므로 동적으로 변경할 수 있습니다. 이메일에 링크를 추가할 때 동적 랜딩 페이지를 선택하면 모든 서비스를 선택할 수 있습니다. 특정 서비스가 연결된 랜딩 페이지를 선택하면 해당 서비스가 자동으로 사용됩니다(다른 서비스를 선택할 수 없음). [자세히 보기](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 이제 랜딩 페이지에서 조건부 콘텐츠가 지원됩니다. [자세히 보기](../landing-pages/lp-content.md)
   * 랜딩 페이지를 서비스에 연결하고, 사용자가 해당 랜딩 페이지를 검증할 때 확인 메시지를 보낼 수 있습니다. [자세히 알아보기](../landing-pages/lp-content.md#lp-message)
   * 봇으로 인한 스팸과 남용으로부터 랜딩 페이지를 보호하기 위해 Captcha를 추가할 수 있습니다. 이는 고객과의 상호 작용이 필요하지 않고 사이트와의 상호 작용을 기반으로 하기 때문에 고객을 방해하지 않습니다. [자세히 알아보기](../landing-pages/create-lp.md#captcha)

이전에는 제한적으로 제공되던 다음과 같은 기능을 이제 **온디맨드**&#x200B;로 사용할 수 있습니다.

* **동적 보고**: 이제 마케팅 활동의 영향을 측정하기 위해 완전히 사용자 정의 가능한 실시간 보고서를 제공하는 동적 보고 기능을 이용할 수 있습니다. 이 기능은 프로필 데이터에 대한 액세스를 추가하여 열기 및 클릭과 같은 기능적 이메일 캠페인 데이터 외에도 성별, 도시, 연령과 같은 프로필 차원별로 인구통계학적 분석을 지원합니다. 다국어 이메일 게재 및 트랜잭션 메시지에 대한 동적 보고 기능도 제공됩니다. [자세히 보기](../reporting/dynamic-reporting/get-started-reporting.md)

* **중앙 집중식 브랜딩** - 기술 관리자는 이제 브랜드의 아이덴티티에 영향을 미치는 매개변수를 중앙 집중화하기 위해 하나 이상의 브랜드를 정의할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. SMS 및 다이렉트 메일을 포함한 모든 채널에 대해 브랜딩 옵션을 사용할 수 있습니다. [자세히 보기](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >이 기능은 새 구현에만 사용할 수 있습니다.

위에 나열된 기능 외에도 이번 릴리스에는 클라이언트 콘솔에서 사용할 수 있는 다음과 같은 기능 세트가 함께 제공됩니다.

* [새 SMS 전송 커넥터](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html). (FDA 환경)
* [나머지 API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html)&#x200B;(주문형, FDA 환경)

클라이언트 콘솔 [릴리스 정보](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}를 참조하십시오.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->