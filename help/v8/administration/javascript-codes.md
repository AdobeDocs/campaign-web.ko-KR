---
title: JavaScript 코드 작업
description: JavaScript 코드를 사용하여 작업하는 방법을 알아봅니다.
exl-id: 4f3b7fce-0373-4db1-8239-64b1bda0f14c
source-git-commit: 3bedb4562c5858cd6057fd8a17064ccac8303c39
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# JavaScript 코드 작업 {#javascript-codes}

<!-- JavaScript codes -->

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_list"
>title="JavaScript 코드"
>abstract="JavaScript 코드"

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_create"
>title="JavaScript 코드 만들기"
>abstract="JavaScript 코드 만들기"

## JavaScript 코드 정보 {#about}

JavaScript 코드를 사용하면 라이브러리와 유사하게 워크플로 전체에서 활용할 수 있는 재사용 가능한 기능을 만들 수 있습니다. 이러한 함수는 왼쪽 탐색 창의 **[!UICONTROL 관리]** > **[!UICONTROL JavaScript 코드]** 메뉴에 저장됩니다.

![](assets/javascript-list.png)

JavaScript 코드 목록에서 다음을 수행할 수 있습니다.

* **코드 복제 또는 삭제**: 줄임표 단추를 클릭하고 원하는 작업을 선택합니다.
* **코드 수정**: 속성을 열려면 코드 이름을 클릭합니다. 변경 작업을 수행한 다음 저장합니다.
* **새 JavaScript 코드 만들기**: **[!UICONTROL JavaScript 코드 만들기]** 단추를 클릭합니다.

>[!NOTE]
>
>JavaScript 콘솔과 웹 사용자 인터페이스 간에 Adobe Campaign 코드 메뉴 위치가 다르지만 목록은 동일하며 거울처럼 작동합니다.

## JavaScript 코드 만들기 {#create}

JavaScript 코드를 만들려면 다음 단계를 수행하십시오.

1. **[!UICONTROL JavaScript 코드]** 메뉴로 이동한 다음 **[!UICONTROL JavaScript 코드 만들기]** 단추를 클릭합니다.

1. 코드의 속성을 정의합니다.

   * **[!UICONTROL 네임스페이스]**: 사용자 지정 리소스와 관련된 네임스페이스를 지정합니다. 기본적으로 네임스페이스는 &quot;cus&quot;이지만 구현에 따라 달라질 수 있습니다.
   * **[!UICONTROL 이름]**: 코드를 참조하는 데 사용할 고유 식별자입니다.
   * **[!UICONTROL 레이블]**: JavaScript 코드 목록에 표시할 설명 레이블입니다.

   ![](assets/javascript-create.png)

   >[!NOTE]
   >
   >**[!UICONTROL 네임스페이스]** 및 **[!UICONTROL 이름]** 필드를 만든 후에는 수정할 수 없습니다. 변경하려면 코드를 복제하고 필요에 따라 업데이트합니다.
   >
   >Campaign 콘솔에서 JavaScript 코드 이름은 이 두 필드의 연결로 표시됩니다.

1. **[!UICONTROL 코드 만들기]** 단추를 클릭하여 JavaScript 코드를 정의합니다. 왼쪽 창에는 조건 및 날짜 서식과 관련된 미리 정의된 함수를 사용할 수 있는 두 개의 메뉴가 있습니다.

   ![](assets/javascript-code.png)

1. 코드를 저장하려면 **[!UICONTROL 확인]**&#x200B;을 클릭하세요.

1. JavaScript 코드가 준비되면 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.  이제 JavaScript 코드를 여러 워크플로우에서 사용할 수 있습니다.

## 워크플로우에서 JavaScript 코드 사용 {#workflow}

### JavaScript 코드 라이브러리 로드 {#library}

워크플로우에서 JavaScript 코드를 참조하여 반복적인 작업에 대한 코드를 다시 작성하지 않을 수 있습니다. 이러한 코드를 사용하려면 먼저 워크플로우의 초기화 스크립트에서 해당 라이브러리를 로드해야 합니다. 이를 통해 워크플로우에서 사용할 함수를 포함하는 모든 라이브러리를 한 번 로드할 수 있습니다.

라이브러리를 로드하려면 다음 단계를 수행합니다.

1. 워크플로우를 열고 **[!UICONTROL 설정]** 단추를 클릭합니다.
1. **[!UICONTROL 초기화 스크립트]** 섹션으로 이동한 다음 **[!UICONTROL 코드 만들기]**&#x200B;를 클릭합니다.

   ![](assets/javascript-initialization.png)

1. 코드를 로드할 때 아래 구문을 사용하십시오.

   ```
   loadLibrary("/<namespace>/<name>")
   ```

   * `<namespace>`을(를) JavaScript 코드를 만드는 동안 지정된 네임스페이스로 바꾸십시오.
   * `<name>`을(를) JavaScript 코드 이름으로 바꾸십시오.

1. **[!UICONTROL 확인]**&#x200B;을 클릭하고 설정을 저장합니다.

### 워크플로우의 참조 함수 {#reference}

JavaScript 라이브러리가 로드되면 워크플로우 내에서 직접 JavaScript 코드에 정의된 함수를 참조할 수 있습니다. 일반적으로 **[!UICONTROL JavaScript 코드]** 활동을 사용합니다.

![](assets/javascript-function.png)
