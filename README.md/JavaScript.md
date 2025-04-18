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

- 대상.addEventListener("이벤트종류",functuin(){})

# 할당 연산자 [0409.html 참고]

- = : 오른쪽 피연산자의 값을 왼쪽 피연산자에 할당
- += : 왼쪽 피연산자에 오른쪽 피연산자를 더하고 그 결과를 다시 왼쪽 피연산자에 할당(이름++)
- -= : 왼쪽 피연산자에서 오른쪽 피연산자를 빼고, 그 결과를 다시 왼쪽 피연산자에 할당
- *= : 왼쪽 피연산자에 오른쪽 피연산자를 곱하고, 그 결과를 다시 왼쪽 피연산자에 할당
- /= : 왼쪽 피연산자를 오른쪽 피연산자로 나눈 몫을 다시 왼쪽 피연산자에 할당
- %= : 왼쪽 피연산자를 오른쪽 피연산자로 나눈 나머지를 다시 왼쪽 피연산자에 할당

# 반복문

- for문 [0409.html/0411.html 참고]
  - for(let i=값; i<최대값; i=커질 값){console.log(출력할 값)}
    - [예시] : for(let i=1; i<11; i+=1){console.log(i)} : i를 1로 지정/i는 11까지 커짐/i는 1씩 증가/i값을 출력
  - 할당 연산자 : 지금 변수의 값을 업데이트 하는 것
  - 중간 연산자 : 변수++ 변수-- 값을 1 증가하거나 감소
- while [0411.html 참고]
- do-while : while 반복문과 매우 유사/조건에 상관없이 먼저 코드 블록을 실행 -> 조건식을 검사 -> 조건식이 참(true)인 동안  
  반복문을 실행
  - let i = 0;do {console.log(i);i++;} while (i < 10);
- do-while 반복문은 코드 블록이 최소 한 번은 무조건 실행 ->  조건식을 검사하 -> 조건식이 참(true)인 동안 반복문 실행

# DOM

- 변수.setAttribute("바꿀 속성","무엇으로 바꿀지") : 태그의 속성을 바꾸는 기능 
- 속성조작 : src, href, 등 태그가 가진 속성을 수정하는 기능/대상.setAttribute("속성", "값") 형식으로 사용할 수 있음
  - img태그지정.setAttribute('src', 'newImage.jpg');
- 속성 가져오기 : src, href, 등 태그가 가진 속성을 가져오는 기능/대상.getAttribute(”속성”) or (”값”) 형식으로 사용
  - img태그지정.getAttribute('src');
- value 가져오기 : input의 값을 가져오는 것은 value로 접근해야 함  
  - const 이름 = document.querySelector('#username') // 대상 지정
  - let 값 = 이름.value;

# 객체 생성과 삭제

- 생성하기
  - let 새로운 태그
    새로운 태그 = document.createElement('div');
  - 만든 객체를 부모에게 붙이기: 태그를 만들어 변수에 저장->부모에게 붙여야 화면에 나타남
    - 부모 바꾸기 : 부모태그.appendChild(만든div태그);
- 삭제하기
  - 부모 지정
  - 부모에서 removeChild 함수를 사용하여 원하는 자식을 제거
  - const 부모 = document.querySelector('#parent');
  - const 삭제대상 = document.querySelector('#child');
  - 부모.removeChild(삭제대상);