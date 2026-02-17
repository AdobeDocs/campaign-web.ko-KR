---
title: 스키마 정보
description: 스키마 작업 방법을 알아봅니다.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# 스키마 정보 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="스키마"
>abstract="Adobe Campaign은 XML 기반 스키마를 사용하여 애플리케이션 내의 데이터의 물리적 및 논리적 구조를 정의합니다. 이 화면에서는 웹 사용자 인터페이스에서 기존 스키마를 모두 보고, 스키마 세부 정보에 액세스하고, 사용자 정의 양식을 구성하고, 스키마를 직접 만들거나 확장할 수 있습니다."

**[!DNL Adobe Campaign]**&#x200B;의 경우 XML 기반 스키마를 사용하여 애플리케이션 내 데이터의 물리적, 논리적 구조를 정의합니다. 스키마는 다음을 정의하는 데이터베이스 테이블에 연결된 XML 문서입니다.

* 테이블 이름, 필드 및 관계를 포함한 SQL 테이블 구조입니다.
* 요소, 특성, 계층, 형식, 기본값 및 레이블을 포함하는 XML 데이터 구조입니다.

스키마는 다음 작업에서 중요한 역할을 합니다.

* 응용 프로그램 데이터를 데이터베이스 테이블에 매핑합니다.
* 데이터 개체 간의 관계를 정의합니다.
* 각 필드의 구조 및 속성 지정.

Adobe Campaign의 각 엔티티에는 전용 스키마가 있어 데이터 일관성과 조직을 유지할 수 있습니다.

스키마 인터페이스를 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* [스키마 액세스 및 사용자 지정](schemas-browse-access.md) - 사용 가능한 스키마를 보고 세부 정보를 탐색하며 화면 표시를 사용자 지정합니다.
* [목록 열 구성](schemas-list-columns.md) - 목록 보기에 기본적으로 표시되는 열을 구성합니다.
* [사용자 정의 필드 편집](schemas-custom-fields.md) - 세부 정보 화면에 표시할 사용자 정의 필드를 구성하고 섹션으로 구성합니다.
* [컬렉션 목록 추가](schemas-collection-lists.md) - 프로필 화면에 관련 데이터를 표시할 컬렉션 목록을 추가합니다.
* [스키마 만들기 및 관리](schemas-create-publish.md#create-schemas) - 새 스키마를 만들고 기존 스키마를 확장합니다.
* [스키마 게시 및 동기화](schemas-create-publish.md#publish) - 스키마 변경 내용을 데이터베이스 구조와 동기화합니다.
* [사용자 정의 양식으로 작업](schemas-custom-forms.md) - 데이터 입력 양식을 사용하여 사용자 정의 스키마에서 레코드를 만들고, 편집하고, 관리합니다.

>[!NOTE]
>
>스키마를 관리하려면 관리자 권한이 있어야 합니다.

스키마에 대한 자세한 내용은 [Campaign 콘솔 설명서](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}를 참조하세요.
