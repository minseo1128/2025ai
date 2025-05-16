- input 에 할 일 입력 후 enter 누르면 추가
    - document.qeurySelector 로 input 지정

- 키보드 이벤트
    - enter일 경우 실행행
    - input.valu="" 하여 input 박스 비우기

- 할 일 추가
    - document.createElement로 div 생성/거기다가 class 추가
    - div 밑에 i 태그 4개 + 내가 입력한 할 일(input.value) 추가(textContent)
        - i 태그에 클래스 추가 + 내용(favorite 등) 추가가

- 하트 관련
    - click 이벤트
    - 채워져 있으면 비우고, textContent.favorite -> favorite_border
    - 비워져 있으면 채우고, textContent.favorite_border -> favorite

- v 관련
    - click 이벤트
    - v 사라짐(CSS) + 글씨색 변함(color) + 취소선(text-decoration)

- x 관련
    - click 이벤트
    - 부모.removeChild(자식)으로 통째로 날리기