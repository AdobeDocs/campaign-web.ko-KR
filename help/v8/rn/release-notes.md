---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 100%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

이전 릴리스를 통해 이용할 수 있는 변경 사항 및 개선 사항은 [2024](release-notes-24.md) 및 [2025](release-notes-25.md) 페이지에 나열되어 있습니다.

## 2025년 10월 업데이트 {#25-9-updates}

_2025년 10월 9일_

<table>
<thead>
<tr>
<th><strong>트랜잭션 메시지, 푸시 알림 및 SMS를 위한 다국어 기능 (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web 사용자 인터페이스에서 여러 언어로 여러 트랜잭션 메시지, 푸시 알림 및 SMS 메시지를 보낼 수 있습니다. 다국어 게재 기능을 사용하면 게재의 기본 언어는 물론, 게재를 전송할 수 있는 다양한 언어를 선택할 수 있습니다. 선택한 언어로 게재 내용을 미리 볼 수도 있습니다.</p>
<p>참고: 이 기능은 조직 집합에만 사용할 수 있으며(제한된 가용성), 향후 릴리스를 통해 전역적으로 출시될 예정입니다.</p>
<p>자세한 내용은 <a href="../msg/multilingual.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>트랜잭션 메시지의 프로필 보강 (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이 기능을 사용하면 Adobe Campaign 데이터베이스 필드를 메시지 콘텐츠에 연결하여 트랜잭션 메시지를 개인화할 수 있습니다. 대상 매핑, 데이터 보강 열 및 조정 키를 선택하여 성능 임계값을 유지하면서 정확한 실시간 개인화를 보장할 수 있습니다.</p>
<p>참고: 이 기능은 조직 집합에만 사용할 수 있으며(제한된 가용성), 향후 릴리스를 통해 전역적으로 출시될 예정입니다. 이 기능은 현재 이메일에서만 사용할 수 있습니다.</p>
<p>자세한 내용은 <a href="../transactional-messaging/profile-enrichment.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>


## 2025년 9월 릴리스 {#25-9-release}

_2025년 9월 23일_

9월 릴리스부터 다음과 같은 기능을 사용할 수 있습니다.

<table>
<thead>
<tr>
<th><strong>API 게재를 위한 사용자 정의 채널</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Adobe Campaign Web UI에서 직접 사용자 정의 API 채널을 기반으로 게재를 조율하고 실행할 수 있습니다. 이들 게재는 독립적으로 실행하거나 워크플로의 일부로 실행할 수도 있습니다. 사용자 정의 API 채널의 구성은 콘솔에서 수행됩니다.</p>
<p>자세한 내용은 <a href="../call-center/gs-custom-channel.md">세부 설명서</a>를 참조하십시오.</p>
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
<p>캠페인 관리자는 이제 Campaign Web 사용자 인터페이스에서 외부 시스템과의 새로운 연결을 설정할 수 있습니다. 기존 외부 계정을 보고, 업데이트하고, 관리할 수도 있습니다.</p>
<p>자세한 내용은 <a href="../administration/create-external-account.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>이메일 콘텐츠 잠금</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign에서 이메일 템플릿의 콘텐츠를 잠글 수 있습니다. 템플릿 전체를 잠그거나 특정 구조 및 구성 요소를 잠그는 것이 가능합니다. 이를 통해 의도하지 않은 편집 또는 삭제를 방지할 수 있으므로 템플릿의 사용자 정의 기능을 더욱 강력하게 제어하고 이메일 캠페인의 효율성과 안정성을 향상시킬 수 있습니다.</p>
<p>자세한 내용은 <a href="../content/content-locking.md">세부 설명서</a>를 참조하십시오.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### 개선 사항 {#25-9-improvements}

* 이메일 디자이너의 조건부 콘텐츠 기능을 사용하여 조건을 설정할 때 새로운 연산자 세트가 추가되었습니다.
* 이제 **대상자 빌드** 워크플로 활동에서 필터링 차원을 사용할 수 있습니다. 이를 확인하거나 변경하려면 타기팅 차원 옆에 있는 아이콘을 클릭하십시오. [자세히 알아보기](../workflows/activities/build-audience.md#build-audience-configuration)
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

