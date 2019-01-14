# CSS
CSS란 Cascading style sheet 의 준말이다. HTML 요소를 표시하는 방법을 설명한다.

## CSS를 사용하는 이유
CSS는 디자인, 레이아웃 및 다양한 장치 및 화면 크기에 대한 디스플레이의 변형을 포함하여 웹 페이지의 스타일을 정의하는데 사용된다.

## CSS Syntax 및 Selector

### CSS Syntax

`h1 {color:blue; font-size:12px;}`

h1 : Selector

color:blue; : Declaration

font-size:12px; : Declaration

### element selector
Element Selector는 element 이름을 기반으로 선택한다.

    p {
     text-align: center;
     color: red;
    }

위와 같이 작성한 경우 모든 p 요소에 대해 작동한다.

### id selector
id selector는 HTML 요소의 id 속성을 사용하여 특정 요소를 선택한다. id는 고유하므로 하나의 고유 요소를 선택하는데 사용된다.

id 이름은 숫자로 시작할 수 없다.

        #para1 {
          text-align: center;
          color: red;
        }

### class selector
class selector는 특정 클래스 속성이 있는 요소를 선택한다.

클래스 이름은 숫자로 시작할 수 없다.

    .center {
      text-align: center;
      color: red;
    }

class명이 center인 요소에 적용된다.

### group selector
코드를 최소화 하기 위해 같은 선언을 할 selector 끼리 묶는게 좋다.

    h1, h2, p {
        text-align: center;
        color: red;
    }

## CSS를 사용하는 방법

1. 외부 스타일 시트
2. 내부 스타일 시트
3. 인라인 스타일

## 스타일 시트가 여러개 있는 경우
가장 마지막에 읽힌 값이 적용 된다.

***우선 순위:*** <br>
인라인 스타일 > 외부 및 내부 스타일 시트 > 브라우저 기본 값

1. 동일한 요소가 두 번 쓰였다면 마지막에 쓴 값으로 가까워진다.
2. id 선택자는 속성 선택자보다 높은 우선 순위를 갖는다. (id를 쓰지 말라고 하는 이유)
3. 클래스 선택기는 요소 선택기보다 높은 우선 순위를 갖는다.
