---
title: 프로필 시작
description: Campaign 웹에서 프로필을 모니터링하고 관리하는 방법을 알아봅니다.
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 26%

---

# 프로필 시작 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="프로필 자세히 살펴보기"
>abstract="새로운 프로필을 만들고, 강력한 보고서와 도구를 통해 모니터링합니다. 프로필 속성, 상호 작용 및 로그에 액세스합니다. 필터링 옵션을 사용하여 프로필 목록을 찾아보고 프로필을 편집 및 업데이트합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=ko" text="릴리스 정보 참조"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="프로필 자세히 살펴보기"
>abstract="새로운 프로필을 만들고, 강력한 보고서와 도구를 통해 모니터링합니다. 프로필 속성, 상호 작용 및 로그에 액세스합니다. 필터링 옵션을 사용하여 프로필 목록을 찾아보고 프로필을 편집 및 업데이트합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=ko" text="릴리스 정보 참조"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="프로필"
>abstract="프로필은 Adobe Campaign에서 보낸 메시지를 수신하도록 대상으로 지정된 개인입니다. 권한에 따라 이 목록에서 프로필의 세부 정보를 볼 수 있습니다. 필터링 옵션을 사용하여 이 목록을 찾아볼 수 있습니다. 일부 프로필 속성을 편집하고 업데이트할 수 있습니다."

## 프로필이란? {#what}

A **프로필**&#x200B;클라이언트 콘솔에서 &quot;수신자&quot;라고도 하는 는 Campaign 데이터베이스에 저장된 개인을 나타내며 의 주요 구성 요소 역할을 합니다. [대상자 만들기](create-audience.md) 게재 및 [개인화 추가](../personalization/personalize.md) 데이터를 콘텐츠에 추가합니다. Adobe Campaign을 사용하면 Campaign 웹 사용자 인터페이스를 통해 새 항목 만들기에서 모든 프로필의 속성 및 서비스 구독에 대한 포괄적인 보기에 액세스하는 등 프로필을 원활하게 관리할 수 있습니다.

또한 **[!UICONTROL 테스트 프로필]**&#x200B;클라이언트 콘솔에서 &quot;시드 프로필&quot;로 식별된 를 사용하면 주어진 게재의 타겟팅 기준과 일치하지 않는 추가 수신자를 타겟팅할 수 있습니다. 이러한 프로필에는 가상 연락처 정보 또는 발신자가 제어하는 연락처 정보가 포함되어 있습니다. 수신자 데이터베이스의 부정 사용을 감지하거나 이메일이 받은 편지함에 도착하는지 확인하기 위해 메시지 대상자에 추가할 수 있습니다. [테스트 프로필 작업 방법 알아보기](test-profiles.md)

프로필과 테스트 프로필 모두 의도한 대상자에게 도달하기 전에 게재를 테스트하는 데 사용할 수 있습니다. 이를 통해 메시지 콘텐츠 및 개인화를 미리 보고, 테스트 및 유효성 검사를 위한 증명을 보내고, 다양한 플랫폼 및 디바이스에서 이메일 렌더링을 평가하고, 랜딩 페이지를 테스트할 수 있습니다. [게재 미리 보기 및 테스트 방법 알아보기](../preview-test/preview-test.md)

## 프로필 목록 액세스 {#access}

프로필은 Adobe Campaign 웹에서 액세스하고 편집할 수 있습니다. **[!UICONTROL 고객 관리]** > **프로필** 왼쪽 탐색 레일의 항목. 다음에서 액세스할 수도 있습니다. **[!UICONTROL 탐색기]** 보기, 에서 **[!UICONTROL 프로필 및 타겟]** > **[!UICONTROL 수신자]** 노드. 여기에서 폴더 또는 하위 폴더를 탐색, 생성 및 관리하고 관련 권한을 확인할 수 있습니다. [폴더 만들기 방법 알아보기](../get-started/permissions.md#folders)

>[!NOTE]
>
>사용 권한에 따라 데이터베이스에 저장된 프로필의 전체 목록에 액세스하지 못할 수도 있습니다. [권한에 대해 자세히 알아보기](../get-started/permissions.md).

다음을 필터링할 수 있습니다. **[!UICONTROL 프로필]** 다음에서 사용할 수 있는 검색 필드 또는 필터를 사용하여 나열: **필터 표시** 단추를 클릭합니다. 결과를 특정 항목으로 제한할 수 있습니다 [폴더](../get-started/permissions.md#folders) 드롭다운 목록을 사용하거나 [쿼리 모델러](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable=&quot;yes&quot;}

프로필의 세부 정보에 액세스하려면 목록에서 해당 이름을 클릭합니다. 프로필에 대한 세부 보기가 열리고 해당 속성과 가입한 서비스를 살펴볼 수 있습니다. [프로필의 세부 정보를 탐색하는 방법 알아보기](create-profile.md)

프로파일을 삭제하려면 다음 목록에서 해당 옵션을 선택합니다 **[!UICONTROL 추가 작업]** 메뉴 아래의 제품에서 사용할 수 있습니다.
