---
audience: end-user
title: 브랜드 관리
description: 브랜드 지침을 만들고 관리하는 방법 알아보기
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 3%

---

# 브랜드 만들기 및 관리 {#brands}

브랜드 지침은 브랜드의 시각적 및 언어적 정체성을 정의하는 포괄적인 규칙 및 표준 세트입니다. 모든 마케팅 및 커뮤니케이션 채널에서 일관된 브랜드 표현을 보장하기 위한 참조 역할을 합니다.

[!DNL Adobe Campaign Web]에서 사용자는 수동으로 브랜드 정보를 입력 및 구성하거나 자동 데이터 추출을 위해 브랜드 지침 문서를 업로드할 수 있습니다.

## 브랜드 액세스 {#generative-access}

**[!UICONTROL 에서]**&#x200B;브랜드[!DNL Adobe Campaign Web] 메뉴에 액세스하려면 사용자에게 **[!UICONTROL 관리자(관리자)]** 및 **[!UICONTROL 브랜드 키트]** 제품 프로필을 할당하여 브랜드를 만들고 관리해야 합니다. 읽기 전용 액세스를 위해 사용자는 [!UICONTROL AI Assistant] 제품 프로필이 필요합니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ 브랜드 관련 권한을 할당하는 방법을 알아봅니다.

1. [Admin Console](https://adminconsole.adobe.com/enterprise) 홈 페이지에서 Campaign 제품에 액세스하십시오.

   ![Campaign 제품 액세스를 표시하는 Admin Console 홈 페이지](assets/brands_admin_1.png)

1. 사용자에게 부여할 권한 수준에 따라 **[!DNL Product profile]**&#x200B;을(를) 선택합니다.

   ![Admin Console에서 제품 프로필 선택](assets/brands_admin_2.png)

1. 선택한 제품 프로필을 할당하려면 **[!DNL Add users]**&#x200B;을(를) 클릭하십시오.

   ![Admin Console에서 사용자 추가 옵션](assets/brands_admin_3.png)

1. 사용자 이름, 사용자 그룹 또는 이메일 주소를 입력합니다.

1. 변경 내용을 적용하려면 **저장**&#x200B;을 클릭하세요.

이 역할에 이미 할당된 사용자의 권한은 자동으로 업데이트됩니다.

+++

## 브랜드 만들기 {#create-brand-kit}

브랜드 지침을 만들고 관리하려면 아래 단계를 따르십시오.

사용자는 세부 정보를 수동으로 입력하거나 브랜드 가이드라인 문서를 업로드하여 정보를 자동으로 추출할 수 있습니다.

1. **[!UICONTROL 브랜드]** 메뉴에서 **[!UICONTROL 브랜드 만들기]**&#x200B;를 클릭합니다.

   ![브랜드 만들기 옵션이 있는 브랜드 메뉴](assets/brands-1.png)

1. 브랜드의 **[!UICONTROL 이름]**&#x200B;을(를) 입력하십시오.

1. 파일을 드래그 앤 드롭하거나 선택하여 브랜드 지침을 업로드하고 자동으로 관련 브랜드 정보를 추출합니다. **[!UICONTROL 브랜드 만들기]**&#x200B;를 클릭합니다.

   이제 정보 추출 프로세스가 시작됩니다. 완료하는 데 몇 분 정도 걸릴 수 있습니다.

   ![브랜드 지침 추출을 위한 파일 업로드](assets/brands-2.png)

1. 이제 콘텐츠 및 시각적 만들기 표준이 자동으로 채워집니다. 다양한 탭을 탐색하여 필요에 따라 정보를 조정합니다. [자세히 알아보기](#personalize)

1. 각 섹션 또는 범주의 고급 메뉴에서 참조를 추가하여 관련 브랜드 정보를 자동으로 추출할 수 있습니다.

   기존 콘텐츠를 제거하려면 **[!UICONTROL 섹션 지우기]** 또는 **[!UICONTROL 범주 지우기]** 옵션을 사용하십시오.

   ![](assets/brands-15.png)

1. 구성하고 나면 **[!UICONTROL 저장]**&#x200B;을 클릭한 다음 **[!UICONTROL 게시]**&#x200B;을 클릭하여 브랜드 지침을 AI Assistant에서 사용할 수 있도록 만드십시오.

1. 게시된 브랜드를 수정하려면 **[!UICONTROL 브랜드 편집]**&#x200B;을 클릭하세요.

   >[!NOTE]
   >
   >이렇게 하면 편집 모드에 임시 복사본이 만들어지고 게시 후 라이브 버전이 대체됩니다.

   ![브랜드 메뉴에서 브랜드 옵션 편집](assets/brands-8.png)

1. **[!UICONTROL 브랜드]** 대시보드에서 ![](assets/do-not-localize/Smock_More_18_N.svg) 아이콘을 클릭하여 고급 메뉴를 열어 다음 작업을 수행합니다.

   * 브랜드 보기
   * 편집
   * 기본 브랜드로 표시
   * 복제
   * 게시
   * 게시 취소
   * 삭제

   ![브랜드 대시보드의 고급 메뉴 옵션](assets/brands-6.png)

이제 AI Assistant 메뉴의 **[!UICONTROL 브랜드]** 드롭다운에서 브랜드 지침에 액세스할 수 있습니다. 이를 통해 AI Assistant는 사용자 사양에 맞게 콘텐츠 및 에셋을 생성할 수 있습니다. [AI Assistant에 대해 자세히 알아보기](../content/generative-gs.md)

브랜드 지침을 사용하여 콘텐츠 품질과 브랜드 정렬을 평가할 수도 있습니다. [콘텐츠 품질 유효성 검사에 대해 자세히 알아보기](brands-score.md#validate-quality)

![브랜드 드롭다운이 있는 AI 도우미 메뉴](assets/brands_6.png)

### 기본 브랜드 설정 {#default-brand}

캠페인 생성 중 콘텐츠를 생성하고 정렬 점수를 계산할 때 자동으로 적용할 기본 브랜드를 지정할 수 있습니다.

기본 브랜드를 설정하려면 **[!UICONTROL 브랜드]** 대시보드로 이동하십시오. ![](assets/do-not-localize/Smock_More_18_N.svg) 아이콘을 클릭하여 고급 메뉴를 열고 **[!UICONTROL 기본 브랜드로 표시]**&#x200B;를 선택합니다.

![브랜드 대시보드의 고급 메뉴 옵션](assets/brands-6.png)

