---
title: 스키마 작업
description: 스키마 작업 방법을 알아봅니다.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 18%

---

# 스키마 작업 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="스키마"
>abstract="**[!DNL Adobe Campaign]**&#x200B;의 경우 XML 기반 스키마를 사용하여 애플리케이션 내 데이터의 물리적, 논리적 구조를 정의합니다. 이 화면에서는 기존 스키마를 모두 볼 수 있으며 목록에서 스키마 이름을 선택하여 스키마의 세부 정보에 액세스할 수 있습니다. 편집 가능한 스키마만 표시하는 등 목록을 구체화하는 데 도움이 되는 필터를 사용할 수 있습니다."

## 스키마 정보 {#about}

**[!DNL Adobe Campaign]**&#x200B;의 경우 XML 기반 스키마를 사용하여 애플리케이션 내 데이터의 물리적, 논리적 구조를 정의합니다. 스키마는 다음을 정의하는 데이터베이스 테이블에 연결된 XML 문서입니다.

* 테이블 이름, 필드 및 관계를 포함한 SQL 테이블 구조입니다.
* 요소, 특성, 계층, 형식, 기본값 및 레이블을 포함하는 XML 데이터 구조입니다.

스키마는 다음 작업에서 중요한 역할을 합니다.

* 응용 프로그램 데이터를 데이터베이스 테이블에 매핑합니다.
* 데이터 개체 간의 관계를 정의합니다.
* 각 필드의 구조 및 속성 지정.

Adobe Campaign의 각 엔티티에는 전용 스키마가 있어 데이터 일관성과 조직을 유지할 수 있습니다.

스키마에 대한 자세한 내용은 [Campaign 콘솔 설명서](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}를 참조하세요.

## 웹 사용자 인터페이스의 스키마에 액세스 {#access}

**[!UICONTROL 관리]** > **[!UICONTROL 스키마]** 메뉴에서 스키마에 액세스할 수 있습니다.

![사용 가능한 스키마와 필터를 보여 주는 스키마 목록 화면](assets/schemas-list.png)

이 화면에서 기존의 모든 스키마를 볼 수 있습니다. 편집 가능한 스키마만 표시하는 등 목록을 구체화하는 데 도움이 되는 필터를 사용할 수 있습니다.

스키마를 열려면 스키마 이름을 선택합니다. 자세한 스키마 보기가 표시됩니다.

![스키마 속성 및 콘텐츠를 표시하는 스키마 세부 정보 화면](assets/schema-details.png)

### 스키마 개요 {#overview}

**[!UICONTROL 개요]** 탭에서는 스키마에 대한 일반 보기를 제공합니다.

* **[!UICONTROL 속성]** 섹션에는 스키마 이름, 네임스페이스 및 관련 테이블 이름과 같은 주요 정보가 표시됩니다.

* **[!UICONTROL 스키마 정의]** 섹션에는 데이터 조정에 사용되는 기본 키와 다른 테이블과의 링크를 포함하여 스키마 정의에 대한 세부 정보가 표시됩니다.

  스키마를 구성하는 다양한 필드 및 링크를 보려면 **[!UICONTROL 스키마 미리 보기]** 단추를 클릭하십시오. 이를 통해 스키마의 전체 구조를 확인할 수 있습니다. 스키마가 사용자 지정 필드로 확장된 경우 모든 해당 확장을 시각화할 수 있습니다.

* **[!UICONTROL 콘텐츠]** 섹션에는 스키마의 XML 콘텐츠가 표시되어 소스와 생성된 구문 간에 전환할 수 있습니다.

### 스키마 데이터 {#data}

**[!UICONTROL 데이터]** 탭에서 스키마 데이터에 대한 정보를 제공합니다.

![데이터 구조 및 특성을 표시하는 스키마 데이터 탭](assets/schemas-data.png)

## 사용자 정의 필드 편집 {#fields}

사용자 지정 필드는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가된 추가 속성입니다. 조직의 요구 사항에 맞게 새 속성을 포함하여 스키마를 사용자 지정할 수 있습니다.

사용자 지정 필드는 Campaign 웹 인터페이스의 프로필 세부 사항과 같은 다양한 화면에 표시할 수 있습니다. 표시되는 필드와 인터페이스에 표시되는 방식을 제어할 수 있습니다. 이렇게 하려면 **[!UICONTROL 스키마]** 메뉴에서 **[!UICONTROL 화면 편집]** 단추를 클릭하십시오.

![편집 가능한 특성을 표시하는 사용자 지정 필드 화면](assets/schemas-custom.png)

**[!UICONTROL 미리 보기]**&#x200B;를 클릭하여 샘플 화면에 사용자 지정 필드를 표시합니다.

스키마에서 사용자 정의 필드를 편집하는 방법에 대한 자세한 내용은 [사용자 정의 필드 구성](../administration/custom-fields.md) 섹션을 참조하십시오.