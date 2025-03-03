## HTML 테이블 개요

표: 데이터 테이블, 2차원 행과 열 구조 <br>
생각보다 표 안에 들어갈 수 있는 요소가 많다.

## 테이블: TR, TD, Th 요소

- ```<td>```: 테이블 데이터 셀
- ```<tr>```: 행
- ```<th>```: 헤더 <br>
[heaviest_birds.html](/Section5/heaviest_birds.html)에 코드 작성

## 테이블: Thead, Tbody, Tfoot 요소

- ```<thead>```: 표 헤더
- ```<tfoot>```: 표 아래 정보
- ```<tbody>```: 표의 주요 데이터

## 테이블: Colspan & Rowspan

여러 열이나 행에 걸친 셀을 생성하는 방법 <br>
- ```<colspan="n">```: 열에서 n칸 차지
- ```<rowspan="n">```: 행에서 n칸 차지

## 폼(Form) 요소

폼: HTML 요소들의 모음, 여러 개별 폼 요소를 품는 컨테이너 <br>
폼 요소: 개별 컨트롤 또는 개별 입력란 <br>

- 폼 요소는 폼을 제출했을 때 폼 데이터를 어디로 보낼지 지정할 수 있다
- 부모 폼 요소에서 데이터를 어떻게, 어디로 전송할지 정한다
- ```<action>``` 속성을 통해 폼이 제출되었을 때 데이터를 보낼 위치와 시간을 지정한다
- 폼을 제출하면 HTTP 요청이 ```<action>``` 태그 경로로 전송되고, 서버에서 해당 작업을 처리한다 <br>

[forms.html](/Section5/forms.html)에 코드 작성

## 일반적인 입력 형식

- ```<input>```: 가장 일반적인 폼 컨트롤, type 속성으로 작동 방식을 변경한다
    - text: 텍스트 입력란
    - password: 비밀번호 입력란
    - color: 색상 선택기
    - number: 숫자 입력란
    - 그 외 여러가지... MDN 문서 참고 요망
- placeholder 속성으로 입력란의 임시 텍스트를 지정할 수 있다

## 가장 중요한 레이블

```<label>```의 역할 <br>
- 시각적으로 텍스트를 보여주는 것
- 특정한 입력값이나 Form control 및 텍스트와 직접적으로 연결
- 두 요소를 연결 시 레이블 자체 클릭 가능
    - ```<lable>```의 for 속성과 ```<input>```의 id 속성을 동일하게 지정
    - 한 개의 요소만 지정된 ID를 지녀야 한다
- ```<input>```을 ```<label>``` 안에 중첩하는 방법도 있으나 권장 X

## HTML 버튼

```<button>```으로 생성 가능 <br>
```<button>```이 form 안에 있으면 기본적으로 해당 폼을 제출한다. (```type="submit"```)<br>
button의 역할만 하고 싶다면 ```type="button"```을 입력해야 한다. <br>
```<input type="submit">```으로도 비슷한 역할을 생성할 수 있다.

## 이름 속성

버튼으로 제출하면 form action 측으로 HTTP 요청을 보낸다. <br>
```<input>```의 name을 통해 서버가 찾으려는 값을 전달한다. <br>
& 기호로 여러 개의 데이터가 하나의 URL로 연결된다. <br>
모든 ```<input>```에 name을 지정해야 서버에서 레이블링이 되어 구별할 수 있다.

## 구글과 레딧 검색하기

```
<form action="https://www.google.com/search">
    <input name="q" type="q">
    <button>Search Google</button>
</form>
```

## 라디오 버튼, 체크박스와 선택창

- checkbox: 체크박스, checked를 통해 처음부터 체크되어 있도록 만들 수 있다.
- radio: 라디오버튼, 그룹에서 1개만 선택 가능, 값을 전송하기 위해 value 속성을 입력해야 한다.
- select: 드롭다운 메뉴, ```<select>```가 여러 ```<option>```을 하나로 묶은 것

## 범위 및 텍스트 영역

- range: 슬라이더를 만들어 해당 범위 내에서 값을 선택
    - min, max로 범위를, step로 단위를 지정할 수 있다
    - value로 최초값을 지정할 수 있다
- min, max를 이용한 숫자 입력
- textarea: 여러 줄의 텍스트 입력, Enter 사용 가능
    - rows, cols로 사이즈 조절 가능

## HTML5 폼의 유효성 검사

유효성 검사: 일반적으로 제한을 추가하거나 사용자 입력 또는 데이터의 유효성을 확인하는 것
- 비어 있으면 안되는 필드
- 7-12 자리의 비밀번호<br>
프론트 측 유효성 검사는 형식에 맞는 데이터인지 검사하는 것이고, 서버 측 유효성 검사는 올바른 데이터인지 검사하는 것 <br>
```required``` 속성을 통해 필수 입력으로 만든다. <br>
```minlength, maxlength``` 속성을 통해 입력 길이를 지정할 수 있다. <br>
email이나 url은 기본적으로 유효성 검사 패턴이 지정되어 있고, 패턴 속성을 이용해 정규 표현식을 만들 수 있다.

## 마라톤 선수 등록 양식 만들기

[race_registration.html](/Section5/race_registration.html)에 코드 작성