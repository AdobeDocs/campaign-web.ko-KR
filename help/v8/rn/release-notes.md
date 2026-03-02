---
title: Campaign v8 Web 사용자 인터페이스 릴리스 정보
description: 최신 Campaign Web 사용자 인터페이스 릴리스에 포함된 새로운 기능 살펴보기
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f77c4998c3db462c3caaece98a65be1226ab7c69
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 42%

---

# 릴리스 정보 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="릴리스 정보"
>abstract="Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 Campaign 릴리스 정보는 최신 기능, 개선 사항 및 수정 사항을 포함하여 한 달에 여러 번 업데이트됩니다. 정기적으로 확인하는 것이 좋습니다."

Adobe Campaign Web 사용자 인터페이스 릴리스는 기능 배포에 대한 보다 확장 가능한 단계별 접근 방식을 고려하는 연속 게재 모델에서 작동합니다. 따라서 이들 릴리스 정보는 월별로 여러 차례 업데이트됩니다. 이들 릴리스 정보를 정기적으로 확인하십시오.

## 2026년 3월 업데이트 {#26-3-release}

<table>
<thead>
<tr>
<th><strong>사용자 지정 Firefly 모델 및 타사 이미지 생성 모델 통합</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>승인된 타사 이미지 모델과 함께 표준 및 사용자 지정 Firefly 모델을 매끄럽게 통합하여 이미지 생성 시 더 큰 유연성, 제어 및 브랜드 정렬을 제공합니다.</p>
<p>요구 사항에 맞는 모델을 선택하십시오.</p>
<ul><li> 추가 설정 없이 즉각적인 이미지를 생성할 수 있도록 <strong>Adobe 모델</strong>(Firefly Image Model 4 제공)</li><li> 특수 기능을 위한 <strong>파트너 모델</strong>(Gemini 2.5 Flash 지원)</li><li>브랜드 정체성, 스타일 및 시각적 지침에 따라 정확하게 일치하는 온브랜드 생성을 위한 <strong>사용자 지정 모델</strong>(사용자 고유의 자산에 대해 교육된 브랜드별 모델).</li></ul>
<p>자세한 내용은 <a href="../content/generative-models.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

## 2026년 2월 릴리스 {#26-2-release}

_2026년 2월 17일_

### 새로운 기능 {#26-2-features}

<!--table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>캠페인 인벤토리의 타임라인 보기</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 캠페인 인벤토리에 시간 경과에 따른 캠페인을 시각화하고 관리할 수 있는 타임라인 보기가 포함됩니다. 목록 및 타임라인 간을 전환하고 주, 월 또는 일별로 탐색하며, 오늘 버튼을 사용하여 현재 날짜로 이동하며, 목록 보기와 동일한 필터 및 검색을 사용하여 오른쪽 패널에서 캠페인 세부 사항(상태, 워크플로, 게재)을 열 수 있습니다.</p>
<p>자세한 내용은 <a href="../campaigns/manage-campaigns.md#timeline">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>스키마 작성(LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>이제 Campaign 웹 사용자 인터페이스에서 직접 스키마를 만들고 관리할 수 있습니다. 이 기능을 사용하면 새 테이블을 만들고, 기존 스키마를 확장하며, 사용자 정의 양식을 만들 수 있습니다. 클라이언트 콘솔에 액세스하지 않고도 특정 비즈니스 요구 사항을 지원하도록 사용자 정의 데이터 구조를 정의할 수 있습니다.</p>
<p>참고: 이 기능은 조직 집합에만 사용할 수 있으며(제한된 가용성), 향후 릴리스를 통해 전역적으로 출시될 예정입니다.</p>
<p>자세한 내용은 <a href="../administration/schemas.md">세부 설명서</a>를 참조하세요.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)-->



