# 변수

- 변수 선언
  - let 변수명
  - const 변수명
  - var 변수명 (같은 이름으로 중복선언 가능)
- 변수 사용할 때 주의할 점
  - 대소문자 가림
  - 숫자는 맨 앞에 못 옴 (ex : let 1번동물)
  - 사용한 코드와 동일한 이름의 변수 불가능
- console.log() : 내가 원하는 내용의 데이터를 꺼내서 확인
  - 페이지에 들어가서 F12->console 들어가면 확인 가능
- alert("") : 경고문
- prompt("") : 입력칸이 있는 경고문
- confirm("") : o/x 확인할 때

# 자료형

- 실수(number) : 실수에도 "" 하면 문자가 됨
  - 수를 나타내는 수 : 1의자리수,10의자리수 등을 구별해서 읽음
  - 문자를 나타내는 수 : 끊어서 숫자 하나하나를 따로 읽음
- 문자열(string)
- 불린(boolean) : 참(true) 또는 거짓(false) 값 표현
- null : 값이 없음
- undefined : 값이 할당되지 않음
- symbol : ES6에서 추가된 자료형/유일한 값

* 참고
  - body - div - div - h1 - ul - li - li

# console.log()

- 변수에 해당되는 값, 어떤 함수가 호출되는지 F12 누르고 확인 가능
  - console.log("문자취급");

# document.queryselector()

- 개념
  - css 선택자(클래스, iD) 를 기반으로 원하는 요소를 선택
  - 단일 요소만 찾아준다. 해당하는 태그가 여러개일 경우 맨 위의 것을 선택

# Dom

- document 객체로 DOM에 접근(브라우저의 문서에 접근하는 객체)
- 원하는 태그 선택->가지고 놀기

# style 조작 방법

- 개체지정.style.**원하는css** =
- DOM에서 css 스타일 명 표기 방법
    - - 기호는 사용 안 함. 
    text-align → textAlign /  background-color → backgroundColor 으로 표기
    - 두 단어의 스타일명은 대문자로 시작함.

# 콜백함수(익명함수)

- 특정한 이벤트가 발생했거나 작업이 완료 되었을 때 호출되는 함수
- function함수이름(){}

# 이벤트

- 대상.addEventListener("이벤트종류",코드)

