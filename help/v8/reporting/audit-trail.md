---
product: campaign
title: 감사 추적
description: Campaign 감사 추적을 사용하여 인스턴스를 모니터링하는 방법 알아보기
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 감사 추적 {#audit-trail}

Adobe Campaign 웹 사용자 인터페이스에서 **[!UICONTROL 감사 추적]** 기능은 사용자가 인스턴스 내의 중요한 엔터티(일반적으로 인스턴스의 원활한 작업에 상당한 영향을 주는 엔터티)에 대한 모든 수정 사항을 완전히 볼 수 있도록 합니다.

>[!IMPORTANT]
>
>* Adobe Campaign Web User Interface는 사용자 권한, 템플릿, 개인화 또는 캠페인 내에서 수행된 변경 사항을 감사하지 않습니다.
>* 인스턴스의 관리자만 감사 추적을 관리할 수 있습니다.

**[!UICONTROL 감사 추적]** 기능은 Adobe Campaign 인스턴스 내에서 발생하는 작업 및 이벤트에 대한 자세한 로그를 실시간으로 지속적으로 기록합니다. 편리한 방법을 사용하여 데이터의 연대순 레코드에 액세스하고, 워크플로 상태, 이를 수정할 최신 개인 또는 인스턴스 내에서 사용자가 수행한 활동과 같은 쿼리를 해결합니다.

+++ 감사 추적 사용 가능한 엔터티에 대해 자세히 알아보기

* **Source 스키마 감사 추적**&#x200B;을 통해 Campaign v8 클라이언트 콘솔에서 수행한 활동 및 스키마에 대한 최근 수정 사항을 모니터링할 수 있습니다.

  스키마에 대한 자세한 내용은 [Campaign v8 설명서](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/developer/shemas-forms/schemas)를 참조하세요.

* **워크플로우 감사 추적**&#x200B;을 통해 다음과 같은 현재 상태를 포함하여 워크플로우에 대한 활동 및 최근 변경 사항을 추적할 수 있습니다.

   * 시작
   * 일시 정지
   * 정지
   * 다시 시작
   * 정리 - 작업 삭제 내역과 같음
   * 시뮬레이션 - 시뮬레이션 모드에서 시작 작업과 같음
   * 절전 모드 해제: 지금 보류 중인 작업 실행 작업과 같음
   * 무조건 정지

  워크플로우에 대한 자세한 내용은 이 [페이지](../workflows/gs-workflows.md)를 참조하세요.

* **옵션 감사 추적**&#x200B;을 통해 Campaign v8에서 수행한 활동 및 최근 옵션 수정 사항을 모니터링할 수 있습니다.

  옵션에 대한 자세한 내용은 이 [페이지](https://experienceleague.adobe.com/ko/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options)를 참조하세요.

* **게재 감사 추적**&#x200B;을 통해 활동 및 게재에 대한 마지막 수정 사항을 확인할 수 있습니다.

  게재에 대한 자세한 내용은 이 [페이지](../msg/gs-deliveries.md)를 참조하세요.

* **외부 계정**&#x200B;을(를) 사용하면 기술 워크플로우 또는 캠페인 워크플로우와 같은 기술 프로세스에서 사용하는 Campaign v8의 외부 계정에 대한 수정 사항을 확인할 수 있습니다.

  외부 계정에 대한 자세한 내용은 이 [페이지](../administration/external-account.md)를 참조하세요.

* **게재 매핑**&#x200B;을(를) 사용하면 Campaign v8에서 게재 매핑에 대한 활동 및 최근 수정 사항을 모니터링할 수 있습니다.

  게재 매핑에 대한 자세한 내용은 이 [페이지](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/audience/add-profiles/target-mappings)를 참조하세요.

* **웹 응용 프로그램**&#x200B;을(를) 사용하면 입력 및 선택 필드가 있는 페이지를 만드는 데 사용되는 Campaign v8에서 웹 폼에 대한 수정 사항과 데이터베이스의 데이터를 포함할 수 있는 수정 사항을 확인할 수 있습니다.

  웹 응용 프로그램에 대한 자세한 내용은 이 [페이지](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/content/webapps)를 참조하세요.

* **오퍼**&#x200B;를 사용하면 활동 및 오퍼에 대한 마지막 수정 사항을 확인할 수 있습니다.

  오퍼에 대한 자세한 내용은 이 [페이지](../msg/offers.md)를 참조하세요.

* **연산자**&#x200B;을(를) 사용하면 Campaign v8에서 연산자에 대한 활동 및 최근 수정 사항을 모니터링할 수 있습니다.

  연산자에 대한 자세한 내용은 이 [페이지](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators)를 참조하세요.

+++

## 감사 추적 액세스 {#accessing-audit-trail}

인스턴스의 **[!UICONTROL 감사 추적]**&#x200B;에 액세스하려면:

1. **[!UICONTROL 관리]** 메뉴에서 **[!UICONTROL 감사 추적]**&#x200B;을 선택합니다.

   ![감사 추적 옵션이 선택된 관리 메뉴를 보여 주는 스크린샷](assets/audit-trail-1.png)

1. 엔터티 목록과 함께 **[!UICONTROL 감사 추적]** 창이 열립니다. Adobe Campaign 웹 사용자 인터페이스는 워크플로우, 옵션, 게재 및 스키마에 대한 만들기, 편집 및 삭제 작업을 감사합니다.

   마지막 수정 사항에 대해 자세히 알아보려면 엔티티 중 하나를 선택합니다.

1. **[!UICONTROL 감사 엔터티]** 창은 다음과 같이 선택한 엔터티에 대한 자세한 정보를 제공합니다.

   * **[!UICONTROL 유형]**: 워크플로, 옵션, 게재 또는 스키마.
   * **[!UICONTROL 엔터티]**: 활동의 내부 이름입니다.
   * **[!UICONTROL 수정한 사람]**: 이 엔터티를 마지막으로 수정한 사람의 사용자 이름입니다.
   * **[!UICONTROL Action]**: 이 엔터티에서 마지막으로 수행한 작업이 생성됨, 수정됨 또는 삭제됨입니다.
   * **[!UICONTROL 수정 날짜]**: 이 엔터티에서 마지막으로 수행한 작업의 날짜입니다.

   코드 블록은 엔티티에서 정확히 변경된 사항에 대한 자세한 정보를 제공합니다.

   ![수정 사항에 대한 자세한 정보가 포함된 감사 엔터티 창을 표시하는 스크린샷](assets/audit-trail-2.png)