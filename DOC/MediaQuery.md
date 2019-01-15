## Media Query
미디어 쿼리를 사용하여 여러 디바이스의 맞춤 스타일 시트를 제공 할 수 있다.

### 구문

    @media not|only mediatype and (expressions) {
        CSS-Code;
    }

지정된 문서가 표시되는 장치 유형(mediatype)과 일치하고 미디어 쿼리의 모든 표현식(expressions)이 참이면 쿼리의 결과는 true이다. not 혹은 only 연산자를 사용하지 않았다면 기본 all 형식이 적용된다.

`<link rel="stylesheet" media="mediatype and|not|only (expressions)" href="print.css">`

이런식으로 표현식에 따라 CSS를 다르게 적용할 수 도 있다.

### 표현식

    @media screen and (min-width: 480px) {
        body {
            background-color: lightgreen;
        }
    }

뷰포트의 너비가 480px 이상 인 경우 (max-width: 480px)로 쓰면 이하인 경우
