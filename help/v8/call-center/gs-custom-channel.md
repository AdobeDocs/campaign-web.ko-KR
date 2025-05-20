---
audience: end-user
title: 사용자 지정 외부 채널 시작
description: Adobe Campaign 웹을 사용하여 사용자 지정 외부 채널 게재를 만들고 보내는 방법을 알아봅니다
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# 사용자 지정 외부 채널 시작 {#gs-custom-channel}

Adobe Campaign Web UI에서 직접 서드파티와 통합된 사용자 지정 외부 채널을 기반으로 게재를 통합 및 실행할 수 있습니다. 사용자 지정 외부 채널 만들기는 클라이언트 콘솔에서 수행됩니다.

워크플로우에서 또는 독립 실행형 게재로 사용자 지정 채널 외부 게재를 구성하고, 대상자를 정의하고, 필요한 모든 연락처 및 개인화 데이터를 사용하여 사용자 지정 가능한 내보내기 파일을 생성할 수 있습니다.

>[!NOTE]
>
>사용자 지정 채널 외부 게재에 대해 웹 UI에서 보고를 사용할 수 없습니다. 보고서에 액세스하려면 클라이언트 콘솔로 이동해야 합니다.

아래 단계에서는 독립 실행형(일회성) 게재 절차를 자세히 설명합니다. 대부분의 단계는 콜 센터 게재와 유사합니다. 자세한 내용은 이 [페이지](../call-center/create-call-center.md)를 참조하세요.

새 독립형 사용자 지정 외부 게재를 만들고 전송하려면 다음 기본 단계를 수행합니다.

1. 사용자 지정 외부 채널을 만듭니다. [자세한 내용](#create-channel)
1. 게재를 만듭니다. [자세한 내용](#create-delivery)
1. 대상자를 정의합니다. [자세히 보기](#select-audience)
1. 콘텐츠 편집, [자세히 보기](#edit-content)
1. 게재를 미리 보고 보냅니다. [자세히 보기](#preview-send)

## 사용자 지정 외부 채널 만들기{#create-channel}

먼저 사용자 지정 외부 채널을 구성해야 합니다. 클라이언트 콘솔에서 수행하는 주요 단계는 다음과 같습니다.

1. 사용 가능한 채널 목록에 새 채널을 추가하도록 스키마를 구성합니다.
1. 새 라우팅 외부 계정을 만듭니다.
1. 새 채널과 연결된 새 게재 템플릿을 만듭니다.

자세한 내용은 [클라이언트 콘솔 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html)를 참조하세요.

## 게재 만들기{#create-delivery}

다음 단계에 따라 게재를 만들고 속성을 구성합니다.

1. **[!UICONTROL 게재]** 메뉴를 선택하고 **[!UICONTROL 게재 만들기]** 단추를 클릭합니다.

1. 원하는 사용자 지정 외부 채널을 선택하고 연결된 템플릿을 선택한 다음 **[!UICONTROL 게재 만들기]**&#x200B;를 클릭하여 확인합니다.

   ![사용자 지정 게재 만들기를 보여 주는 스크린샷](assets/cus-create.png){zoomable="yes"}


1. **[!UICONTROL 속성]**&#x200B;에서 게재할 **[!UICONTROL 레이블]**&#x200B;을(를) 입력하십시오.

   ![사용자 지정 게재에 대한 속성 구성을 보여 주는 스크린샷](assets/cus-properties.png){zoomable="yes"}

게재 만들기에 대한 자세한 내용은 콜센터 [설명서](../call-center/create-call-center.md#create-delivery)를 참조하세요.

## 대상자 정의{#select-audience}

이제 추출 파일의 타겟이 될 대상자를 정의해야 합니다.

1. 게재 페이지의 **[!UICONTROL 대상]** 섹션에서 **[!UICONTROL 대상 선택]**&#x200B;을 클릭합니다.

1. 기존 대상자를 선택하거나 직접 대상자를 만듭니다.

   ![사용자 지정 게재에 대한 대상 선택을 보여 주는 스크린샷](assets/cc-audience2.png){zoomable="yes"}

대상자 정의에 대한 자세한 내용은 콜센터 [설명서](../call-center/create-call-center.md#select-audience)를 참조하세요.

## 콘텐츠 편집{#edit-content}

이제 사용자 지정 채널 전달에서 생성될 추출 파일의 컨텐츠를 편집해 보겠습니다.

1. 게재 페이지에서 **[!UICONTROL 콘텐츠 편집]** 단추를 클릭합니다.

1. **[!UICONTROL 파일 이름]**&#x200B;을 지정하고 **[!UICONTROL 파일 형식]**&#x200B;을 선택한 다음 추출 파일에 필요한 만큼 열을 추가하십시오.

   ![추출 파일에 대한 특성 구성 옵션을 보여 주는 스크린샷입니다.](assets/cc-content-attributes.png)

콘텐츠 편집에 대한 자세한 내용은 콜센터 [설명서](../call-center/create-call-center.md#edit-content)를 참조하세요.

## 게재 미리 보기 및 보내기{#preview-send}

게재 콘텐츠가 준비되면 테스트 프로필을 사용하여 미리 보고 증명을 보낼 수 있습니다. 그런 다음 게재를 전송하여 추출 파일을 생성할 수 있습니다.

1. 게재 콘텐츠 페이지에서 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하고 테스트 프로필을 선택합니다.

   ![게재 콘텐츠 페이지의 콘텐츠 시뮬레이션 옵션을 보여 주는 스크린샷](assets/cus-simulate.png){zoomable="yes"}

1. 게재 페이지에서 **[!UICONTROL 검토 및 보내기]**&#x200B;를 클릭하고 **[!UICONTROL 준비]**&#x200B;를 클릭합니다. 그런 다음 확인합니다.

   ![준비 옵션 및 로그 메뉴를 보여 주는 스크린샷](assets/cus-prepare.png){zoomable="yes"}

1. **[!UICONTROL 보내기]**&#x200B;를 클릭하여 최종 전송 프로세스를 진행한 다음 확인합니다.

미리 보기 및 전송에 대한 자세한 내용은 콜센터 [설명서](../call-center/create-call-center.md#preview-send)를 참조하세요.
