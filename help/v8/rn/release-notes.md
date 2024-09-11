---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 020cd1608887023dd4ff434c58cc98e3c1f93adf
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 59%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 9월 업데이트 {#9-2024}

<table>
<thead>
<tr>
<th><strong>Adobe Campaign 웹의 AI Assistant - Content Accelerator</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>메시지를 만들고 맞춤화했으면 Adobe Campaign Web의 AI Assistant for Content Acceleration을 사용하여 한 차원 높은 수준으로 메시지를 이동하십시오. 이 강력한 도구를 사용하면 매력적인 텍스트, 주요 제목 및 시각적으로 매력적인 이미지를 생성하여 콘텐츠의 영향을 최적화할 수 있습니다.</p>
<p>기능을 직접 탐색하고 기능을 완전히 이해할 수 있도록 설계된 <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">라이브 기능 미리 보기</a>를 통해 실습 경험에 몰입하세요.</a>.</p>
<p>자세한 내용은 <a href="../email/generative-gs.md">세부 설명서</a>를 참조하세요.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
</td>
</tr>
</tbody>
</table>

## 8월 릴리스 정보 {#24-8-release}

**릴리스 일자**: 2024년 9월 3일

8월 릴리스부터 다음과 같은 기능 및 개선 사항을 이용할 수 있습니다.

* **값 배포** - 개인화를 위해 필드 목록에 액세스할 때 이제 각 필드에 대한 값이 어떻게 배포되어 있는지 확인할 수 있습니다. 전용 팝업 창에 각 값의 수와 백분율이 표시됩니다. [자세히 알아보기](../query/build-query.md#distribution-values-query)

* **SMTP 매개 변수** - 이제 전자 메일 게재 설정에서 SMTP 설정을 사용할 수 있습니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#smtp)

* **전역 변수** - 이제 전역 변수를 정의하여 게재의 값을 정의할 수 있습니다. [자세히 알아보기](../advanced-settings/delivery-settings.md#variables-delivery)

### 제한 공개된 새로운 기능 {#acs-24-8}

>[!AVAILABILITY]
>
>다음 기능은 제한 공개(LA)로 제공됩니다. **Adobe Campaign Standard에서 Adobe Campaign v8로** 마이그레이션하는 고객으로 제한되며 다른 환경에는 배포할 수 없습니다.
>
>다음 문서 페이지를 참조하세요. [Campaign v8로 Campaign Standard 전환](../rn/acs-migration.md) 및 [Campaign Standard 사용자를 위한 기능](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **다이렉트 메일에 대한 브랜딩** - 기술 관리자는 이제 브랜드의 정체성에 영향을 미치는 매개변수를 중앙 집중화하기 위해 하나 이상의 브랜드를 정의할 수 있습니다. 여기에는 브랜드 로고, 랜딩 페이지의 액세스 URL의 도메인 또는 메시지 추적 설정이 포함됩니다. 이제 이러한 브랜드를 만들어 메시지 또는 랜딩 페이지에 연결할 수 있습니다. 이 구성은 템플릿에서 관리됩니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **랜딩 페이지를 포함하는 구독** - 이제 랜딩 페이지를 서비스에 연결하고 사용자가 유효성을 검사할 때 확인 메시지를 보낼 수 있습니다. [자세히 알아보기](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **시각적 조각** - 이제 시각적 콘텐츠 조각을 보관할 수 있습니다. [자세히 알아보기](../content/create-fragment.md#archive)

* **랜딩 페이지의 CAPTCHA** - 이제 CAPTCHA를 추가하여 봇으로 인한 스팸 및 남용을 방지할 수 있습니다. 이는 고객과의 상호 작용이 필요하지 않고 사이트와의 상호 작용을 기반으로 하기 때문에 고객을 방해하지 않습니다. [자세히 알아보기](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
