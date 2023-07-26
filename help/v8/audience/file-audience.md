---
audience: end-user
title: 파일에서 수신자 타겟팅
description: 외부 파일에서 수신자를 사용하여 이메일 대상자를 빌드하는 방법 알아보기
badge: label="Alpha"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 66%

---

# 파일에서 이메일 대상자 로드 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="파일 선택"
>abstract="업로드할 로컬 파일을 선택합니다. 지원되는 형식은 TXT 및 CSV입니다. 파일 형식을 아래 링크된 샘플 파일에 일치시킵니다."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="열 정의"
>abstract="로컬 파일에서 삽입할 열 형식을 확인합니다."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="서식 지정 매개변수"
>abstract="파일에 대한 서식 지정 매개변수를 확인합니다."

외부 파일에서 연락처를 업로드할 수 있습니다. 프로필이 데이터베이스에 추가되지 않지만 입력 파일의 모든 필드를 사용할 수 있습니다. [개인화](../personalization/gs-personalization.md). 지원되는 파일 형식은 텍스트(TXT) 및 쉼표로 구분된 값(CSV)입니다. 

>[!CAUTION]
>
>* 이 기능은 에만 사용할 수 있습니다. **독립형 이메일 게재**. 워크플로우나 SMS 또는 푸시 게재에서는 사용할 수 없습니다.
>
>* 외부 파일에서 대상 모집단을 로드하면 [컨트롤 그룹](control-group.md)을 사용할 수 없습니다.


이메일 인터페이스에서 직접 로컬 파일의 프로필을 타겟팅하려면 다음 단계를 수행합니다.

1. 기존 이메일 게재를 열거나 [새 이메일 게재 만들기](../email/create-email.md).
1. **대상자** 섹션의 이메일 게재 생성 창에서 **대상자 선택** 버튼을 클릭하고 **파일에서 선택** 옵션을 선택합니다.

   ![](assets/select-from-file.png)

1. 업로드할 로컬 파일을 선택합니다. 형식은 와 일치해야 합니다. [샘플 파일](#sample-file).
1. 화면 중앙 섹션에서 데이터가 매핑되는 방식을 미리 보고 확인합니다.
1. **주소 필드** 드롭다운에서 이메일 주소가 포함된 열을 선택합니다. 입력 파일에 이러한 정보가 있는 경우 차단 목록 열을 선택할 수도 있습니다.
1. 열 설정과 사용 가능한 옵션에서 데이터 서식을 지정하는 방법을 조정합니다.
1. 설정이 적절하면 **확인**&#x200B;을 클릭합니다.

메시지 콘텐츠를 만들고 개인화할 때 의 입력 파일에서 필드를 선택할 수 있습니다. [개인화 편집기](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## 샘플 파일 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="샘플 파일"
>abstract="지원되는 파일 형식은 txt, csv입니다. 첫 번째 라인을 열 머리글로 사용합니다."

지원되는 형식은 TXT 및 CSV입니다. 첫 번째 줄은 열 머리글입니다.

파일 형식을 아래의 샘플 파일과 일치시키십시오.

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
