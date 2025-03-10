## 불투명도와 알파 채널

RGBA: RAG + Alpha Channel(투명도 조절, 0-1)<br>
```background-color: rgba(255, 255, 255, 0.7)```처럼 사용<br>
해당 요소나 이걸 적용하는 부분의 배경 색상에만 영향을 준다.<br><br>

불투명도: 해당 요소의 콘텐츠 및 자손을 포함한 전체 요소의 투명도를 결정하는 특성<br>
```background-color: yellow; opacity: 0.33;```처럼 사용<br>
전체 ```<div>```가 다 불투명도의 영향을 받는다.<br>

## 위치 속성

위치 특성: 문서 내에서 요소의 위치를 설정, static, relative, absolute 등을 사용한다.<br>
위치 특성이 설정한 위치에 따라서 top, right, bottom, left 등이 결정된다.<br>
- static: 디폴트, 고정된 위치
- relative: 문서의 일반적인 흐름에 따라 위치가 정해지지만 top, left, right, bottom 등으로 현 위치와의 상대적 위치로 오프셋을 줄 수 있다.
- absolute: 요소가 문서의 일반적인 흐름에서는 제거되지만 가장 가까이 위치한 부모이 있다면 해당 부모를 기준으로 하거나 조상이 가까이 없다면 초기 컨테이닝 블록 ```<body>```를 기준으로 상대적인 위치에 배치
- fixed: 그 자리에 계속 유지, 배치되는 위치는 항상 컨테이닝 블록에 상대적이다. 내비게이션 바 등을 만드는 방법
- sticky: 시작할 때는 위쪽에 고정되지 않은 상태로 스크롤을 따라가지만 위쪽에 도달하면 그 위치에 고정된다.

## CSS 전환

한 특성값에서 다른 값으로 변화할 때 전환으로 애니메이션 효과를 주는 것<br>
```
.circle:hover {
    background-color: cyan;
}
```
현재 코드에서는 전환이 사용되고 있지 않아 한 요소에서 다른 요소로 넘어가는 지점이 어색하다.<br>
따라서 circle에 다음과 같이 코드를 추가한다.<br>
```
.circle {
    background-color: cyan;
    transition: 1s;
}
```
애니메이션 효과가 적용돼 전환이 애니메이션화 된 것을 확인할 수 있다.<br><br>

Transition 구문에는 특성 이름, 지속 시간, 대기 시간, 딜레이를 지정할 수 있다.<br>
```
transition: 특성 이름 지속 시간 딜레이;
transition: background-color 3s 1s; border-radius 2s;
```
타이밍 기능으로 ease, ease-in ease-out, linear, cubic-bezier 등 다양한 옵션으로 변화 모습을 지정할 수 있다. 

## CSS 변환이 가진 능력

transform: 사물 회전, 확대, 축소, 이동 등 다양한 요소 변형 가능<br>
```transform-origin``` 속성으로 변형 기준점을 설정할 수 있다.<br>
공백으로 나눠 한 개 이상을 적용하거나 조합해서 쓸 수 있다.<br>
- rotate: 회전, rotateX(), rotateY(), rotatez()처럼 축 기준 회전도 가능
    - ```transform: rotate(45deg);```: 45도 회전
- scale: 크기 변화(확대, 축소),X, Y, Z, 3D 등이 있다.
    - ```transform: scale(0.5);```: 1/2 사이즈로 축소
    - ```transform: scale(2, 1);```: 가로만 2배 확대
- translate: 이동, X, Y 등으로 움직일 수 있다.
    - ```transform: ranslateX(200px);```: 오른쪽으로 200px 움직인다.
- skew: 요소를 2차원 평면상에서 기울인다.
    - ```transform: skew(30deg);```: 30도 기울이기
    - ```transform: skew(10deg, 25deg);```: X는 10도, Y는 25도 기울이기

## 멋진 버튼 호버(Hover) 효과 주기

HoberButton 폴더에서 실습 진행

## 배경에 관한 진실



## 놀라운 구글의 글꼴



## 사진 블로그 코딩하기 

