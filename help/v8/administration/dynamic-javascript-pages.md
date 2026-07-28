---
title: 동적 JavaScript 페이지 작업
description: 동적 JavaScript 페이지를 사용하여 작업하는 방법을 알아봅니다.
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2df9759bb21eae0630bcbe9130a1a20b165e8cca
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 26%

---

# 동적 JavaScript 페이지 작업 {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="동적 JavaScript 페이지"
>abstract="동적 JavaScript 페이지(JSSP)를 사용하면 사용자 정의 API, 내보내기 또는 웹 애플리케이션 논리와 같은 URL을 통해 액세스할 때 동적 콘텐츠를 생성하는 서버 측 페이지를 구축할 수 있습니다. 이 목록에서 동적 JavaScript 페이지를 만들거나, 수정하거나, 복제하거나, 삭제할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="동적 JavaScript 페이지 만들기"
>abstract="동적 JavaScript 페이지에 대한 네임스페이스, 이름 및 레이블을 정의한 후, JavaScript 코드를 사용하여 콘텐츠를 작성합니다. 네임스페이스와 이름이 만들어진 후에는 수정할 수 없습니다."

## 동적 JavaScript 페이지 기본 정보 {#about}

동적 JavaScript 페이지(JSSP)를 사용하면 사용자 정의 API, 내보내기 또는 웹 애플리케이션 논리와 같은 URL을 통해 액세스할 때 동적 콘텐츠를 생성하는 서버 측 페이지를 구축할 수 있습니다. 이러한 페이지는 왼쪽 탐색 창의 **[!UICONTROL 관리]** > **[!UICONTROL 동적 JavaScript 페이지]** 메뉴에 저장됩니다.

![사용 가능한 옵션을 표시하는 동적 JavaScript 페이지 목록 인터페이스](assets/dynamic-javascript-pages.png)

동적 JavaScript 페이지 목록에서 다음 작업을 수행할 수 있습니다.

* **페이지 복제 또는 삭제**: 줄임표 단추를 클릭하고 원하는 작업을 선택합니다.
* **페이지 수정**: 페이지 이름을 클릭하여 속성을 열고 변경한 다음 저장합니다.
* **새 동적 JavaScript 페이지 만들기**: **[!UICONTROL 동적 JavaScript 페이지 만들기]** 단추를 클릭합니다.

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## 동적 JavaScript 페이지 만들기 {#create}

동적 JavaScript 페이지를 만들려면 다음 단계를 수행하십시오.

1. **[!UICONTROL 동적 JavaScript 페이지]** 메뉴로 이동한 다음 **[!UICONTROL 동적 JavaScript 페이지 만들기]** 단추를 클릭합니다.

1. 페이지의 속성을 정의합니다.

   * **[!UICONTROL 네임스페이스]**: 사용자 지정 리소스와 관련된 네임스페이스를 지정합니다. 기본적으로 네임스페이스는 &quot;cus&quot;이지만, 구현에 따라 달라질 수 있습니다.
   * **[!UICONTROL 이름]**: 페이지를 참조하는 데 사용한 고유 식별자입니다.
   * **[!UICONTROL 레이블]**: 동적 JavaScript 페이지 목록에 표시되는 설명 레이블입니다.

   ![네임스페이스, 이름 및 레이블 필드를 표시하는 동적 JavaScript 페이지 생성 인터페이스](assets/dynamic-javascript-pages2.png)

   >[!NOTE]
   >
   >**[!UICONTROL 네임스페이스]** 및 **[!UICONTROL 이름]** 필드를 만든 후에는 수정할 수 없습니다. 변경하려면 페이지를 복제하고 필요에 따라 업데이트합니다.

1. **[!UICONTROL 코드 만들기]** 단추를 클릭하여 페이지 콘텐츠를 정의한 다음 `<%@ page %>` 지시문과 핵심 라이브러리를 로드하기 위한 `NL.require()` 호출을 사용하여 JSSP 코드를 작성합니다.

   ![동적 JavaScript 페이지 코드 편집기](assets/dynamic-javascript-pages4.png)

1. 코드를 저장하려면 **[!UICONTROL 확인]**&#x200B;을 클릭하세요.

1. 동적 JavaScript 페이지가 준비되면 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. 이제 `https://<your-instance>/<namespace>/<name>` 형식의 네임스페이스와 이름으로 작성된 URL에서 페이지에 액세스할 수 있습니다. 예를 들어 `cus` 네임스페이스의 이름이 `recipientAPI.jssp`인 페이지는 `https://<your-instance>/cus/recipientAPI.jssp`에서 액세스할 수 있습니다.

재사용 가능한 JavaScript 함수에 대한 자세한 내용은 [JavaScript 코드 작업](javascript-codes.md)을 참조하세요.
