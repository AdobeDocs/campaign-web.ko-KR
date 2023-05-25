---
audience: end-user
title: 파일에서 수신자 Target
description: 외부 파일의 수신자를 사용하여 이메일 대상자를 작성하는 방법을 알아봅니다
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 20%

---

# 파일에서 수신자 로드 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="파일 선택"
>abstract="업로드할 로컬 파일을 선택합니다. 지원되는 형식은 TXT 및 CSV입니다. 아래 링크된 샘플 파일과 파일 형식을 맞춥니다."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="열 정의"
>abstract="로컬 파일에서 삽입할 열의 형식을 확인합니다."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="서식 지정 매개변수"
>abstract="파일의 형식 매개 변수를 확인합니다."

외부 파일에서 연락처를 업로드할 수 있습니다. 이 기능은 이메일 게재에만 사용할 수 있습니다. 지원되는 파일 형식은 텍스트(TXT)와 쉼표로 구분된 값(CSV)입니다. 프로필이 데이터베이스에 추가되지는 않지만 입력 파일의 모든 필드를 개인화에 사용할 수 있습니다.

>[!NOTE]
>
>가져오기 워크플로우를 작성하여 데이터베이스에서 여러 프로필을 추가하거나 업데이트할 수 있습니다. 자세히 알아보기


인터페이스에서 직접 로컬 파일의 프로필을 타겟팅하려면 다음 단계를 수행합니다.

1. 이메일 게재 만들기 창의 **대상자** 섹션에서 **대상자 선택** 버튼을 클릭하고 다음을 선택합니다. **파일에서 선택** 옵션을 선택합니다.

   ![](assets/select-from-file.png)

1. 업로드할 로컬 파일을 선택합니다.
1. 화면의 중앙 섹션에서 데이터가 매핑되는 방식을 미리 보고 확인합니다.
1. 에서 이메일 주소를 포함하는 열을 선택합니다. **주소 필드** 드롭다운. 입력 파일에 이러한 정보가 있으면 차단 목록 열을 선택할 수도 있습니다.
1. 열 설정 및 사용 가능한 옵션에서 데이터 서식 지정 방법을 조정합니다.
1. 설정이 적절하면 **확인**&#x200B;을 클릭합니다.

메시지 콘텐츠 작성 및 개인화 시 개인화 편집기의 입력 파일에서 필드를 선택할 수 있습니다.

![](assets/select-external-perso.png)

>[!CAUTION]
>
>다음을 사용할 수 없습니다. [컨트롤 그룹](control-group.md) 외부 파일에서 대상 모집단을 로드할 때.

## 샘플 파일 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="샘플 파일"
>abstract="지원되는 파일 형식: txt, csv. 첫 번째 라인을 열 머리글로 사용하십시오."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
