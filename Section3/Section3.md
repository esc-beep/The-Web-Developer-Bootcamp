## HTML 개요

- 마크업(텍스트나 데이터의 구조를 명시) 언어
- 텍스트 콘텐츠를 마크업하여 구조화하기 위해 사용
- 태그 구문 사용
- 웹 문서를 마크업하면 웹 페이지에 반영됨

## 우리의 첫 HTML 페이지

확장자: ```.html``` <br>
[chicken.html 작성](/Section3/chicken.html)

## 팁: Mozilla Developer Network

[Mozilla Developer Network](https://developer.mozilla.org/ko/)

## 단락 요소

- ```<p>```: 단락 태그, 블록 레벨 요소

## 제목 요소

- ```<h1>```부터 ```<h6>```까지 존재함
- ```<h1>```: 페이지의 최상위 제목, 페이지 당 1개만
- 상위 제목 태그부터 사용해야 함, ```<h4>```가 없는데 ```<h5>```를 사용하면 X

## Chrome Inspector 개요

- 크롬 개발자 도구
- Mac: Cmd + option + C
- Window: F12

## HTML 상용구

모든 HTML 문서에 들어가야 하는 표준화된 마크업
! 입력하고 tab만 눌러도 자동으로 완성됨 <br>

- ```<!DOCTYPE html>``` - HTML5를 사용하고 있다는 표시
- ```<html>``` - HTML 요소 추가
    - ```<head>``` - 메타데이터 정보
        - ```<title>``` - 문서 제목
    - ```<body>``` - 문서의 모든 내용을 담고 있는 요소

## VSCode 팁 : 자동 포맷

- Mac: Shift + option + F
- Window: Shift + Alt  + F

## 목록 요소

- ```<ol>```: 순서가 있는 목록
- ```<ul>```: 순서가 없는 목록
- ```<li>```: list item, 목록 하위 요소

## 앵커 태그

- ```<a>```: 앵커 요소, 다른 위치로 연결 가능
- ```<a href="URL">``` 형태로 사용
- 인라인 태그 - 블록 처리 X

## 이미지

- ```<img>``` 태그 안에 속성 추가 필요
- ```<img src="이미지 주소" alt="이미지 설명">```
- alt 속성을 넣어 이미지의 설명을 적어 접근성 향상 가능

## 주석

- ```<!-- 주석 내용 -->```
- 메모, 피드백, 리마인더 용도
- Mac: Cmd + '+' + /
- Window: Ctrl + K + C