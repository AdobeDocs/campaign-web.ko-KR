---
audience: end-user
title: 파일에서 수신자 가져오기
description: 외부 파일에서 수신자를 가져오는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 97%

---

# 파일에서 수신자 가져오기 {#audience-from-file}

게재 인터페이스에서 텍스트 파일(TXT) 또는 쉼표로 구분된 값 파일(CSV)을 업로드하여 연락처를 추가하거나 업데이트할 수 있습니다. 추가 또는 업데이트된 연락처는 데이터베이스에 추가됩니다.

>[!NOTE]
>
>여러 프로필을 추가하거나 업데이트하는 가져오기 워크플로를 구축할 수도 있습니다.


인터페이스에서 직접 로컬 파일의 프로필을 추가하려면 다음 단계를 따르십시오.

1. 게재 생성 창에서 **대상자 선택** 버튼을 클릭한 다음 **파일에서 선택** 옵션을 선택합니다.
1. 업로드할 로컬 파일을 선택합니다.
1. 열 설정 및 데이터 형식 지정 방법을 정의합니다. **열 무시** 토글을 사용하여 열을 건너뛸 수 있습니다.
1. 화면 중앙 섹션에서 데이터가 매핑되는 방식을 미리 봅니다.
1. 설정이 적절하면 **확인**&#x200B;을 클릭합니다.

메시지 콘텐츠 작성 및 개인화 시 개인화 편집기의 입력 파일에서 필드를 선택할 수 있습니다.

## 샘플 파일 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="샘플 파일"
>abstract="지원되는 파일 형식: txt, csv. 첫 번째 라인을 열 머리글로 사용하십시오."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
