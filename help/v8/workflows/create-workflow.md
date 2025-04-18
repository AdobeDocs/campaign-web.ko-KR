---
audience: end-user
title: Adobe Campaign Web을 사용하여 워크플로 만들기
description: Adobe Campaign 웹으로 워크플로우를 만드는 방법을 알아봅니다
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 18%

---

# 워크플로 만들기 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="캠페인의 워크플로 목록"
>abstract="**워크플로** 탭에는 현재 캠페인에 연결된 워크플로가 모두 나열됩니다. 편집하려면 워크플로 이름을 클릭합니다. **워크플로 만들기** 버튼을 사용하여 이 캠페인에 새 워크플로를 추가합니다."

독립 실행형 워크플로우 또는 캠페인 내에서 워크플로우를 만들 수 있습니다. 첫 번째 단계는 템플릿을 선택하고 일반 속성을 정의하는 것입니다. 그런 다음 필요에 따라 추가 설정을 구성합니다.

이렇게 하려면 다음 단계를 수행합니다.

1. **독립 실행형 워크플로**&#x200B;를 만들려면 **워크플로** 메뉴로 이동하십시오. **캠페인 워크플로**&#x200B;를 만들려면 **캠페인** 메뉴로 이동한 다음 새 워크플로를 만들 캠페인을 여십시오.

1. 화면 오른쪽 상단의 **[!UICONTROL 워크플로 만들기]** 단추를 클릭합니다.

   ![화면 오른쪽 상단에 워크플로 만들기 단추를 표시하는 스크린샷입니다.](assets/workflow-create.png){zoomable="yes"}

1. 워크플로 **속성** 대화 상자에서 워크플로를 만드는 데 사용할 템플릿을 선택합니다(기본 제공 템플릿을 사용할 수도 있음). [워크플로 템플릿에 대해 자세히 알아보기](#workflow-templates).

1. 워크플로우의 레이블을 입력합니다. 또한 화면의 **[!UICONTROL 추가 옵션]** 섹션의 전용 필드에 워크플로우에 설명을 추가하십시오.

1. **[!UICONTROL 추가 옵션]** 섹션을 확장하여 워크플로우에 대한 추가 설정을 구성합니다. [이 페이지](workflow-settings.md#properties)에서 워크플로 속성을 구성하는 방법을 알아보세요.

   ![워크플로 설정을 구성하기 위한 추가 옵션 섹션을 보여 주는 스크린샷입니다.](assets/workflow-additional-options.png){zoomable="yes"}

1. **[!UICONTROL 워크플로 만들기]** 단추를 클릭하여 워크플로 만들기를 확인합니다.

이제 워크플로우가 만들어지고 워크플로우 목록에서 사용할 수 있습니다. 해당 시각적 캔버스에 액세스하여 수행할 작업을 추가, 구성 및 오케스트레이션할 수 있습니다. [워크플로우 활동을 오케스트레이션하는 방법을 알아봅니다](orchestrate-activities.md).

## 워크플로 템플릿 작업 {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="워크플로 템플릿"
>abstract="워크플로 템플릿에는 새 워크플로를 만드는 데 재사용할 수 있는 사전 구성된 설정 및 활동이 포함되어 있습니다."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="워크플로 속성"
>abstract="워크플로 템플릿에는 새 워크플로를 만드는 데 재사용할 수 있는 사전 구성된 설정 및 활동이 포함되어 있습니다. 이 화면에서는 워크플로 템플릿의 레이블을 입력하고 내부 이름, 폴더 및 실행 폴더, 시간대, 감독자 그룹 등의 설정을 구성합니다."

워크플로 템플릿에는 새 워크플로를 만드는 데 재사용할 수 있는 사전 구성된 설정 및 활동이 포함되어 있습니다. 워크플로우를 만들 때 워크플로우 속성에서 워크플로우의 템플릿을 선택합니다. 기본적으로 빈 템플릿이 제공됩니다.

기존 워크플로우에서 템플릿을 만들거나 새 템플릿을 처음부터 만들 수 있습니다. 두 방법 모두 아래에 자세히 설명되어 있습니다.

>[!BEGINTABS]

>[!TAB 기존 워크플로우에서 템플릿 만들기]

기존 워크플로우에서 워크플로우 템플릿을 만들려면 다음 단계를 수행합니다.

1. **워크플로** 메뉴를 열고 템플릿으로 저장할 워크플로를 찾아봅니다.
1. 워크플로 이름의 오른쪽에 있는 세 점을 클릭하고 **템플릿으로 복사**&#x200B;를 선택합니다.

   ![워크플로 메뉴의 템플릿으로 복사 옵션을 보여 주는 스크린샷입니다.](assets/wf-copy-as-template.png){zoomable="yes"}

1. 팝업 창에서 템플릿 만들기를 확인합니다.
1. 워크플로 템플릿 캔버스에서 필요에 따라 활동을 선택, 추가 및 구성합니다.
1. **설정** 단추에서 설정으로 이동하여 워크플로 템플릿의 이름을 변경하고 설명을 입력하십시오.
1. 템플릿의 **폴더** 및 **실행 폴더**&#x200B;를 선택하십시오. 폴더는 워크플로 템플릿이 저장되는 위치입니다. 실행 폴더는 이 템플릿을 기반으로 만든 워크플로우가 저장되는 폴더입니다.

   ![워크플로 템플릿의 폴더 및 실행 폴더 설정을 보여 주는 스크린샷입니다.](assets/wf-settings-template.png){zoomable="yes"}

   다른 속성은 워크플로와 공통됩니다. [이 페이지](workflow-settings.md#properties)에서 자세히 알아보십시오.

1. 변경 내용을 저장합니다.

이제 템플릿 목록에서 워크플로 템플릿을 사용할 수 있습니다. 이 템플릿을 기반으로 워크플로우를 만들 수 있습니다. 이 워크플로우는 템플릿에 정의된 설정 및 활동으로 사전 구성됩니다.

>[!TAB 처음부터 템플릿을 만듭니다]

워크플로 템플릿을 처음부터 만들려면 다음 단계를 수행하십시오.

1. **워크플로** 메뉴를 열고 **템플릿** 탭으로 이동합니다. 사용 가능한 워크플로우 템플릿 목록을 볼 수 있습니다.
1. 화면 오른쪽 상단의 **[!UICONTROL 템플릿 만들기]** 단추를 클릭합니다.
1. 레이블을 입력하고 추가 옵션을 열어 워크플로 템플릿에 대한 설명을 입력합니다.
1. 템플릿의 폴더 및 실행 폴더를 선택합니다. 폴더는 워크플로 템플릿이 저장되는 위치입니다. 실행 폴더는 이 템플릿을 기반으로 만든 워크플로우가 저장되는 폴더입니다.

   ![폴더 및 실행 폴더 설정을 사용하여 새 워크플로 템플릿을 만드는 것을 보여 주는 스크린샷입니다.](assets/new-wf-template.png){zoomable="yes"}

   다른 속성은 워크플로와 공통됩니다. [이 페이지](workflow-settings.md#properties)에서 자세히 알아보십시오.

1. **만들기** 단추를 클릭하여 설정을 확인합니다.
1. 워크플로 템플릿 캔버스에서 필요에 따라 활동을 추가하고 구성합니다.

   ![활동 추가 및 구성을 위한 워크플로 템플릿 캔버스를 보여주는 스크린샷입니다.](assets/wf-template-activities.png){zoomable="yes"}

1. 변경 내용을 저장합니다.

이제 템플릿 목록에서 워크플로 템플릿을 사용할 수 있습니다. 이 템플릿을 기반으로 워크플로우를 만들 수 있습니다. 이 워크플로우는 템플릿에 정의된 설정 및 활동으로 사전 구성됩니다.

>[!ENDTABS]