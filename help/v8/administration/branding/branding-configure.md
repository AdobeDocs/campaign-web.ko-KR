---
title: 브랜딩
description: 브랜드 구성 방법 살펴보기
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 29%

---

# 브랜드 구성 {#branding-configure}

>[!IMPORTANT]
>
>최종 사용자가 브랜드를 만들거나 수정할 수 없습니다. 이러한 작업은 Adobe Campaign 기술 관리자가 수행해야 합니다. 요청이 있으면 Adobe 고객 지원 센터에 문의하십시오.

Adobe Campaign V8의 브랜드는 **[!UICONTROL 관리 > 플랫폼 > 브랜딩]** 메뉴에서 찾을 수 있습니다.

**[!UICONTROL 브랜드]**&#x200B;는 다음과 같은 특성에 의해 정의됩니다.

* 브랜드를 정의하고 개인화하는 **[!UICONTROL 아이덴티티]**&#x200B;입니다. 이 섹션에는 다음 필드가 포함되어 있습니다.

   * 인터페이스에 표시되는 **[!UICONTROL 레이블]**
   * **[!UICONTROL ID]**
   * **[!UICONTROL 브랜드 이름]**
   * 브랜드의 **[!UICONTROL 웹 사이트 URL]** 및 **[!UICONTROL 웹 사이트 레이블]**
   * **[!UICONTROL 브랜드 로고]**

  ![](assets/branding_1.png)

* 캠페인 수신자에게 표시되는 내용을 개인화하는 **[!UICONTROL 보낸 전자 메일의 헤더 매개 변수]**. 이 섹션에는 다음 필드가 포함되어 있습니다.

   * 브랜드 이메일 주소가 있는 **[!UICONTROL 발신자(이메일 주소)]**.
   * 브랜드 이름이 있는 **[!UICONTROL 발신자(이름)]**.
   * 고객이 회신할 수 있는 이메일 주소가 있는 **[!UICONTROL 회신 대상(이메일 주소)]**.
   * 브랜드 이름이 있는 **[!UICONTROL 회신 대상(이름)]**.
   * 오류가 발생한 경우 사용할 이메일 주소가 있는 **[!UICONTROL 오류(이메일 주소)]**.

  >[!IMPORTANT]
  >
  >이메일의 헤더 매개 변수를 업데이트한 후 템플릿에서 만든 이메일에서 발신자의 이름 및 이메일 주소가 변경되지 않은 경우, 템플릿의 고급 설정을 확인하십시오.

  ![](assets/branding_2.png)

* **[!UICONTROL 브랜드 구성]**&#x200B;은(는) 랜딩 페이지 액세스를 위한 추적에도 사용되는 서버를 정의합니다. 이 섹션에는 다음 필드가 포함되어 있습니다.

   * **[!UICONTROL Brand 하위 도메인]**&#x200B;은(는) Adobe에서 위임이 요청된 이 브랜드와 관련된 지정된 하위 도메인 URL을 참조합니다.

  추적, 미러 및 애플리케이션 서버에 대한 구성은 라우팅과 연관된 별도의 외부 계정에 저장됩니다. 이러한 설정은 프로비저닝 중에 적용되므로 수정해서는 안 됩니다. URL을 표시하려면 외부 계정에서 **[!UICONTROL 브랜딩 접두사]** 탭에 액세스하십시오.

  ![](assets/branding_3.png)

* **[!UICONTROL URL 구성 추적]** 메뉴를 사용하면 Adobe Analytics 및 Google Analytics과 같은 Web Analytics 도구와의 통합을 위한 추가 매개 변수를 정의하여 URL 추적을 개선할 수 있습니다.

  **[!UICONTROL 추가 URL 매개 변수]** 메뉴를 사용하여 적용 가능성 조건과 함께 추가 매개 변수를 키-값 쌍으로 만드십시오. 각 매개 변수 이름은 고유해야 하며 비어 있지 않아야 하고, 각 매개 변수 값은 비어 있지 않아야 합니다. 적용 가능성 조건은 비어 있을 수 있지만 이러한 값 중 JST 태그를 포함할 수 있는 값은 없습니다.

  이러한 매개 변수는 **[!UICONTROL 도메인 이름 목록]**&#x200B;에 지정된 모든 도메인 이름과 일치하는 추적된 URL에 적용되며, 여기에는 정규 표현식이 포함될 수 있습니다.

  **예:** 해당 도메인에 대해 추가 매개 변수 `https://www.example.com` 및 `https://www.example.com/?age=21&deliveryName=DM101`이(가) 구성되면 `age=21`과(와) 같은 추적된 URL은 `deliveryName=DM101`이(가) 됩니다.

## 트랜잭션 메시지를 위한 브랜딩 구성 {#branding-transactional-config}

>[!IMPORTANT]
>
>이 섹션은 트랜잭션 메시지(메시지 센터)에만 적용됩니다.
>
>트랜잭션 기능은 Campaign 웹 UI에서 사용할 수 있지만 아래 단계는 Campaign v8 클라이언트 콘솔(컨트롤 인스턴스)에서 수행해야 합니다.

브랜딩과 함께 트랜잭션 메시지(메시지 센터)를 사용하는 경우 추가 구성이 필요합니다.

### 실시간 인스턴스에 대한 추적 공식

브랜딩이 실시간(RT) 제어 인스턴스에서 활성화되면 특정 추적 옵션이 추적 공식을 관리하는 데 사용됩니다. 이러한 수식은 각 RT 실행 인스턴스에서 개별적으로 구성되지 않고 RT 제어 인스턴스에서 중앙에서 구성됩니다.

다음 옵션은 RT 게재에서 사용하는 추적 공식을 정의합니다.

* **`NmsTracking_RT_ClickFormula`**: RT 인스턴스에서 클릭 추적에 사용되는 수식을 지정합니다.

* **`NmsTracking_RT_OpenFormula`**: RT 인스턴스에서 열린 추적에 사용되는 수식을 지정합니다.

구현에서 트랜잭션 메시지에 대한 사용자 지정 추적 수식이 필요한 경우 아래 옵션을 사용하십시오.

* **`Branding_RT_ListXtkOptions_toPublish`**: 사용자 지정 수식의 XTK 옵션 이름을 여기에 나열합니다(쉼표로 구분). 이렇게 하면 RT 게재가 사용자 지정 추적 공식을 적용할 수 있습니다.