## CSS란?

CSS: 문서를 시각적으로 표현하고 나타내기 위해서 사용하는 언어 <br>
디자인적 요소

## 방대한 CSS에 당황하지 않기

CSS를 적용할 수 있는 다양한 특성들이 있다. <br>
[CSS Reference](https://developer.mozilla.org/ko/docs/Web/CSS/Reference)에서 필요한 내용을 찾아보자. <br>

## 스타일을 올바르게 담기

CSS 작성 스타일 <br>
1. HTML 요소에 직접 작성 - 다른 요소와 스타일 공유와 수정이 어려움
2. 요소와 중첩되거나 포함되지 않는 스타일 요소를 사용해 CSS를 직접 작성 - 여러 페이지에 적용 어려움
3. 외부 스타일 시트(.css 파일)에서 스타일 작성
    - ```<header>```에 포함
    - ```<link>``` 요소를 사용하고 href 속성을 지정

## 색 및 배경색 속성

기본적인 CSS rule은 다음과 같다. <br>
```
selector {
        property: value;
}
```
- color: 텍스트 색상 변경
- background-color: 배경 색상 변경

## 색상 시스템: RGB와 알려진 색상

140가지의 색깔은 red, dark khaki처럼 명명되어 있다. <br>
조금 더 상세한 색상을 선택하고 싶다면 RGB 색상으로 rgb (0, 0, 0)와 같이 입력해 색을 지정할 수 있다. <br>

## 색상 시스템: 16진법

HEX 방식으로 색을 ```#ffffff```와 같이 표현할 수 있다. <br>

## 세미콜론과 CSS

CSS에서는 매 특성 선언 끝에 세미콜론(;)를 필수적으로 작성해야 한다. <br>

## 일반 텍스트 속성

- text-align: 텍스트 정렬(요소 내적인 정렬)
- font-weight: 폰트 굵기, bolder같은 키워드나 400같은 숫자로 지정 가능
- text-decoration: 텍스트를 꾸미는 선(underline, overline, line-through)
    - text-decoration-color로 색을, text-decoration-style로 선 종류 지정 가능
    - 굳이 요소를 넣지 않아도 입력하면 알아서 지정됨
- line-height: 줄 간격
- letter-spacing: 자간 조절

## 픽셀로 글꼴 크기 지정하기

- font-size: 글꼴 크기 지정, 단위로는 주로 px 사용
- px은 절대적인 사이즈이기 때문에 반응형 웹사이트에는 추천 X

## 글꼴 집합

font-family: 요소의 폰트를 변경할 때 사용 <br>
내장 폰트가 아닌 것은 따로 설치해서 사용해야 한다. <br>
font-stack: 사용하려는 폰트를 순서대로 적은 목록 <br>
```font-family: 글꼴1, 글꼴2, 글꼴3;``` 처럼 적으면 백업 폰트를 지정할 수 있다.<br>