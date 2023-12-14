---
audience: end-user
title: 쿼리 모델러를 사용하여 첫 번째 쿼리 작성
description: Adobe Campaign 웹 쿼리 모델러에서 첫 번째 쿼리를 빌드하는 방법을 알아봅니다.
source-git-commit: e620df0ff9af0d32fc353a904e3dde37501495d0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 79%

---

# 표현식 편집 {#expression}

표현식을 편집하려면 수동으로 조건을 입력하여 규칙을 만듭니다. 이 모드에서는 고급 기능을 사용할 수 있습니다. 이러한 함수를 사용하면 날짜, 문자열, 숫자 필드, 정렬 등과 같은 특정 쿼리를 수행하는 데 사용되는 값을 조작할 수 있습니다.

이러한 작업은 쿼리 모델러 표현식 편집 단추에서 사용할 수 있으며, 사용자 지정 조건을 구성할 때 속성 및 값 필드에 사용할 수 있습니다.

![](assets/edit-expression.png)

표현식 편집기에서 제공하는 사항:

* 표현식이 정의된 입력 필드.
* 표현식에서 사용할 수 있고 쿼리의 타겟팅 차원에 해당하는 사용 가능한 필드 목록.
* 카테고리별로 정렬한 사용 가능한 함수 목록.

입력 필드에 직접 표현식을 입력하거나 사용 가능한 필드 및 함수 목록을 사용하여 표현식을 편집합니다. 이렇게 하려면 요소를 추가할 비표현식에 커서를 놓고 원하는 필드 또는 표현식을 두 번 클릭합니다.

워크플로우의 이벤트 변수를 사용하여 표현식을 작성할 수 있습니다. 자세한 내용은 xxxx를 참조하십시오.

## 표현식 구문 {#expression-syntax}

### 표준 구문 {#standard-syntax}

표준 표현식은 다음 구문 요소와 관련된 하나 또는 여러 조건으로 구성됩니다.

* 각 조건은 **&lt;값1> &lt;비교 연산자> &lt;값2>** 형식을 취합니다.

   * **&lt;값1>**&#x200B;은 필드 또는 함수입니다. 예를 들어 프로필이 생성된 날짜의 경우 **@created** 또는 프로필이 생성된 연도의 경우 **Year(@created)**&#x200B;가 있습니다.
   * **&lt;comparison operator=&quot;&quot;>** 는 비교 연산자 섹션에 나열된 연산자 중 하나입니다. 이 연산자는 **&lt;값1>**&#x200B;과 **&lt;값2>** 간의 비교 방법을 정의합니다.
   * **&lt;값2>**&#x200B;는 수동으로 입력되는 필드, 함수 또는 값입니다.

  >[!NOTE]
  >
  >**&lt;값1>** 및 **&lt;값2>**&#x200B;의 형식 데이터는 동일해야 합니다. 예를 들어 **&lt;값1>**&#x200B;이 날짜인 경우 **&lt;값2>**&#x200B;도 날짜여야 합니다.

* 여러 조건을 사용하려면 논리 연산자를 사용하여 결합할 수 있습니다.

   * **[!UICONTROL 및]**: 두 가지 조건이 교차됩니다.
   * **[!UICONTROL 또는]**: 두 가지 조건이 결합됩니다.

예제:

```
Year(@created) = Year(GetDate()) AND Month(@created) = Month(GetDate())
```

이 예에서는 생성 날짜가 현재 월 및 연도인 프로필이 타겟팅됩니다.

### JavaScript 구문 {#javascript-syntax}

HTML 콘텐츠 편집기의 텍스트 유형 블록의 가시성 조건을 정의할 때는 JavaScript 유형 구문이 있는 표현식을 사용해야 합니다.

JavaScript 표현식은 하나 이상의 조건으로 구성되며 다음 구문 요소를 사용합니다.

* 각 조건은 **&lt;컨텍스트> &lt;비교 연산자> &lt;값2>** 형식을 취합니다.

   * **&lt;컨텍스트>**&#x200B;는 컨텍스트를 지정할 수 있는 필드 또는 함수입니다. 예를 들어 **context.profile@email**&#x200B;의 프로필 이메일 주소 또는 **context.profile.firstName.length()**&#x200B;의 프로필 이름의 문자 수가 있습니다.
   * **&lt;comparison operator=&quot;&quot;>** 는 비교 연산자 섹션에 나열된 연산자 중 하나입니다. 이 연산자는 **&lt;컨텍스트>**&#x200B;와 **&lt;값2>** 간의 비교 방법을 정의합니다.
   * **&lt;값2>**&#x200B;는 수동으로 입력되는 필드, 함수 또는 값입니다.

  >[!NOTE]
  >
  **&lt;컨텍스트>** 및 **&lt;값2>**&#x200B;의 형식 데이터는 동일해야 합니다. 예를 들어 **&lt;컨텍스트>**&#x200B;가 날짜인 경우 **&lt;값2>**&#x200B;도 날짜여야 합니다.

* 여러 조건을 사용하려면 논리 연산자를 사용하여 결합할 수 있습니다.

   * **[!UICONTROL &amp;&amp;]**: 두 가지 조건이 교차됩니다.
   * **[!UICONTROL ||]**: 두 가지 조건이 결합됩니다.

예제:

```
context.profile.age > 21 && context.profile.firstName.length() > 0
```

이 예제의 경우 21세 이상이고 이름이 제공된 프로필입니다(**firstName** 필드에 하나 이상의 문자 포함).

## 비교 연산자 {#comparison-operators}

일부 규칙의 경우 쿼리 편집기를 사용하여 조건을 정의할 값을 선택할 수 있습니다.

다음 연산자 중 하나를 사용하여 조건을 값에 연결해야 합니다.

<table> 
 <thead> 
  <tr> 
   <th> 연산자<br /> </th> 
   <th> 표준 구문<br /> </th> 
   <th> JavaScript 구문<br /> </th> 
   <th> 설명<br /> </th> 
   <th> 예제<br /> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <span class="uicontrol">같음</span> <br /> </td> 
   <td> =<br /> </td> 
   <td> ==<br /> </td> 
   <td> 첫 번째 값은 두 번째 값과 완전히 같아야 합니다.<br /> </td> 
   <td> <strong>@lastName = Martin</strong>은 완전히 같은 문자만 사용하여 성이 'Martin'인 프로필을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">보다 큼</span> <br /> </td> 
   <td> &gt;<br /> </td> 
   <td> &gt;<br /> </td> 
   <td> 첫 번째 값은 두 번째 값보다 명확히 커야 합니다.<br /> </td> 
   <td> <strong>@age &gt; 50</strong> 은 '50'보다 나이가 많은 프로필을 검색하므로 '51', '52' 등을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">보다 작음</span> <br /> </td> 
   <td> &lt;<br /> </td> 
   <td> &lt;<br /> </td> 
   <td> 첫 번째 값은 두 번째 값보다 명확히 작아야 합니다.<br /> </td> 
   <td> <strong>@created &lt; DaysAgo(100)</strong>은 100일 전 데이터베이스에 생성된 모든 프로필을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">크거나 같음</span> <br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> 첫 번째 값은 두 번째 값보다 크거나 같아야 합니다.<br /> </td> 
   <td> <strong>@age &gt;= 30</strong>은 30세 이상의 프로필을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">작거나 같음</span> <br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> 첫 번째 값은 두 번째 값보다 작거나 같아야 합니다.<br /> </td> 
   <td> <strong>@age &lt;= 60은</strong> 60세 이하의 프로필을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">다름 </span> <br /> </td> 
   <td> !=<br /> </td> 
   <td> !=<br /> </td> 
   <td> 첫 번째 값은 두 번째 값과 달라야 합니다.<br /> </td> 
   <td> <strong>@language != English</strong>는 영어를 사용하지 않는 프로필을 검색합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">포함</span> <br /> </td> 
   <td> IN<br /> </td> 
   <td> N/A<br /> </td> 
   <td> 첫 번째 값은 두 번째 값을 포함해야 합니다.<br /> </td> 
   <td> <strong>@domain IN mail</strong>. 여기서 'mail' 값이 있는 모든 도메인 이름이 결과로 반환됩니다. 따라서 'gmail.com' 도메인 이름은 반환된 결과의 일부를 구성합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">비슷함</span> <br /> </td> 
   <td> LIKE<br /> </td> 
   <td> N/A<br /> </td> 
   <td> <span class="uicontrol">비슷함</span>은 <span class="uicontrol">포함</span> 연산자와 매우 유사합니다. 검색 중인 값에 <span class="uicontrol">%</span> 와일드카드 문자를 삽입할 수 있습니다.<br /> </td> 
   <td> <strong>@lastName LIKE Mart%n</strong>. 여기서 대체 문자 <strong>%</strong> 는 철자가 틀린 가상의 사례에서 이름 "Martin"을 찾기 위해 "조커" 역할을 합니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">비슷하지 않음</span> <br /> </td> 
   <td> NOT<br /> </td> 
   <td> N/A<br /> </td> 
   <td> <span class="uicontrol">비슷함</span>과 유사합니다. 입력한 값을 복구할 수 없습니다. 여기서도 입력한 값은 <span class="uicontrol">%</span> 와일드카드 문자를 포함해야 합니다.<br /> </td> 
   <td> <strong>@lastName NOT Smi%h</strong>. 여기에서 이름 'Smi%h'(Smith 등)에 해당하는 수신자는 결과로 반환되지 않습니다.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">비어 있음</span> <br /> </td> 
   <td> IS NULL<br /> </td> 
   <td> N/A<br /> </td> 
   <td> 첫 번째 값은 빈 값에 해당해야 합니다.<br /> </td> 
   <td> <strong>@mobilePhone IS NULL</strong>은 휴대전화 번호가 제공되지 않은 모든 프로필을 검색합니다.<br /> </td> 
  </tr> 
 </tbody> 
</table>