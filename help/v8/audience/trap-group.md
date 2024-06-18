---
audience: end-user
title: 트랩 그룹 사용
hide: true
hidefromtoc: true
description: Campaign 웹 사용자 인터페이스에서 게재에 트랩 그룹을 사용하는 방법을 알아봅니다
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# 사용 **[!UICONTROL 트랩 그룹]** {#trap-group}

A **[!UICONTROL 트랩 그룹]** 정의된 대상 기준과 일치하지 않는 수신자를 타겟팅하는 데 사용됩니다. 이렇게 하면 게재 범위를 벗어난 수신자는 다른 대상 수신자와 마찬가지로 게재를 받을 수 있습니다.
A **[!UICONTROL 트랩 그룹]** 은(는) 의 그룹입니다. **[!UICONTROL 시드 주소]**.

## 사용 이유 **[!UICONTROL 트랩 그룹]**

다음을 사용할 수 있습니다. **[!UICONTROL 트랩 그룹]** :

1. **증명** : 의 각 멤버 **[!UICONTROL 트랩 그룹]** 은 마치 대상의 일부인 것처럼 게재를 받습니다.


1. **메일링 목록을 보호하려면** : 대상자가 받게 될 내용을 각각 수신함 **[!UICONTROL 시드 주소]** / **[!UICONTROL 트랩 그룹]** 타사에서 메일링 목록을 사용하는 경우 이 표시됩니다.

## 정보 **[!UICONTROL 트랩 그룹]**

시드 주소는 다음 게재 통계에 대한 보고서에서 자동으로 제외됩니다. **클릭수**, **열림**, **구독 취소**. 보고서는 실제 대상자에 대해서만 표시됩니다.

이메일 게재의 경우 이메일 주소만 필요합니다. **[!UICONTROL 트랩 그룹]**, 다른 필드의 개인화는 Campaign에 의해 임의로 채워집니다.

## 를 설정하는 방법 **[!UICONTROL 트랩 그룹]** 게재 중

을(를) 설정하려면 **[!UICONTROL 트랩 그룹]**&#x200B;로 이동합니다. **[!UICONTROL 대상자]** 게재 설정. 2가지 옵션이 있습니다.
- [테스트 프로필 선택](#select-test-profile)
- [조건 만들기](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 테스트 프로필 선택 {#select-test-profiles}

&quot;테스트 프로필 선택&quot;을 선택하면 다음과 같이 초대되는 창이 표시됩니다. **[!UICONTROL 테스트 프로필 추가]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

버튼을 클릭하면 추가할 수 있는 시드 주소에 액세스할 수 있습니다. **[!UICONTROL 트랩 그룹]**. 사용할 항목을 선택합니다.
새 시드 주소를 만들 수 있습니다. [자세히 알아보기](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

트랩 주소를 확인하면 아래에 올바른 번호가 있는지 확인하십시오. **[!UICONTROL 트랩 그룹]**.

![](assets/trap-check.png){zoomable="yes"}

### 조건 만들기 {#create-condition}

포함 **[!UICONTROL 조건 만들기]** 을(를) 선택하면 쿼리를 사용자 지정하여 사용할 시드 주소를 정의할 수 있는 새 창이 열립니다.

![](assets/trap-create-condition.png){zoomable="yes"}

쿼리가 아래에 표시됩니다. **[!UICONTROL 트랩 그룹]**.

![](assets/trap-custom.png){zoomable="yes"}

## 새로 만드는 방법 **[!UICONTROL 시드 주소]** {#create-seed}

새 을(를) 만들 수 있습니다 **[!UICONTROL 시드 주소]** 위치: **[!UICONTROL 탐색기]** > **[!UICONTROL 리소스]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 초기 멤버]**

![](assets/trap-create.png){zoomable="yes"}

시드 멤버에 대한 모든 세부 정보를 대상 프로필인 것처럼 완료할 수 있습니다.

![](assets/trap-create-contact.png){zoomable="yes"}