---
title: 외부 계정 관리
description: 외부 계정을 구성하는 방법 알아보기
exl-id: 52b4ec99-4f55-4e0b-8a54-b25058d97b02
source-git-commit: 1a5f49cfdf56a21faedcef3029b62b88ebd81c8d
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 17%

---

# 외부 계정 만들기 {#create-external-account}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="외부 계정 작성"
>abstract="캠페인 관리자는 이제 Campaign Web 사용자 인터페이스에서 외부 시스템과의 새로운 연결을 설정할 수 있습니다. 기존 외부 계정을 보고, 업데이트하고, 관리할 수도 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="릴리스 정보 참조"

새 외부 계정을 만들려면 아래에 설명된 단계를 수행합니다. 특정 구성 설정은 만들고 있는 외부 계정 유형에 따라 다릅니다.

1. 왼쪽 창 메뉴에서 **[!UICONTROL 관리]**&#x200B;의 **[!UICONTROL 외부 계정]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL 외부 계정 만들기]**&#x200B;를 클릭합니다.

   ![웹 사용자 인터페이스에서 외부 계정을 만드는 옵션을 보여 주는 스크린샷입니다.](assets/external_account_create_1.png)

1. **[!UICONTROL 레이블]**&#x200B;을(를) 입력하고 외부 계정 **[!UICONTROL 유형]**&#x200B;을(를) 선택하십시오.

   * [캠페인 특정 유형](external-account.md)
   * [Adobe 솔루션 통합](integration-external-account.md)
   * [데이터 전송](transfer-external-account.md)
   * [외부 데이터베이스](external-account-database.md)

   ![레이블을 입력하고 외부 계정 유형을 선택하는 필드를 보여 주는 스크린샷입니다.](assets/external_account_create_2.png)

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

1. 필요한 경우 **[!UICONTROL 추가 옵션]** 드롭다운에서 **[!UICONTROL 내부 이름]** 또는 **[!UICONTROL 폴더]** 경로를 변경합니다.

   ![내부 이름 및 폴더 경로 구성에 대한 추가 옵션을 보여 주는 스크린샷입니다.](assets/external_account_create_3.png)

1. 이 외부 계정에서 관리하는 데이터를 자동으로 내보내려면 **[!UICONTROL 자동으로 패키지로 내보내기]** 옵션을 사용하도록 설정하십시오. <!--Exported where??-->

   ![패키지에서 자동 내보내기를 사용하도록 설정하는 옵션을 보여 주는 스크린샷입니다.](assets/external_account_create_exported.png)

1. **[!UICONTROL 세부 정보]** 섹션에서 선택한 외부 계정 유형에 따라 자격 증명을 지정하여 계정에 대한 액세스를 구성합니다. [자세히 알아보기](#bounce)

1. 구성이 올바른지 확인하려면 **[!UICONTROL 연결 테스트]**&#x200B;를 클릭하십시오.

1. **[!UICONTROL 자세히..]** 메뉴에서 외부 계정을 복제하거나 삭제하십시오.

   ![외부 계정을 복제하거나 삭제할 수 있는 옵션이 있는 기타 메뉴를 보여 주는 스크린샷입니다.](assets/external_account_create_4.png)

1. 구성이 완료되면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
