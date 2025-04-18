# 기본 태그1

- UTF : 문자표현 방식
- <title> A </title> : A 부분이 인터넷 상단 부분의 이름
- head부분 : 나 자신에 대한 정보
- body부분 : 우리가 보는 모든 내용을 차지
  - lang 속성 : 국가별 언어를 표시(ko,en,...)
  - meta 태그: 태그들을 설명하는 태그
  - <h1> A </h1> : 제목으로 사용할 법한 큰 글씨(h1이 가장 큰 글씨)
  - <p> A <p> : paragraph의 약자/본문 내용으로 사용할 법한 작은 글씨
  - <b> A <b> : 두꺼운 글씨체
  - <i> A </i> : 비스듬한 글씨체
  - <u> A </u> : 글씨 밑에 선
  - <del> A </del> : 가운데에 선

# 기본 태그2

- br : 줄바꿈 태그
- 닫는 태그 없음
- hr : 구분선 태그
  - 닫는 태그 없음
- 리스트 태그
  - ul 태그
    - 순서 없는 리스트(동그라미)
    - <li> 리스트 </li>
  - ol 태그
    - 순서 있는 리스트(숫자)
    - <li> 리스트 </li>
- 미디어 태그
  - a 태그
    - 링크 넣을 수 있음
    - <a href="링크"> a 태그 </a> : 원래 있던 창에서 이동
    - <a target="_blank" href="링크"> a 태그 </a> : 새로운 창에서 이동
  - img 태그 -<img src="이미지 주소 복사한 링크" alt="오류 떠서 이미지 안뜰 때 대체 문구">
    -img와 src 사이에 width="n px" 넣으면 사진 사이즈 조절 가능, 필수x
    -title="이름" : 사진에 이름 붙이기
    <video src="../"></video>
  - 오디오 태그
    - <audio src=""></audio>
    - 옵션 : controls, autoplay, loop
  - 비디오 태그
    - <video src=""></video>
    - 옵션 : controls, autoplay, loop
  - div 태그
    - division의 약자, 문서의 구획을 나누는 역할
    - 별도의 의미 없음 구역 정의 용도

# CSS 태그

- style="color : 색깔;background-color:배경색깔;width:실수px;height:실수px"
  - color : 색깔 : 글씨색
  - background-color : 배경색
  - width : 배경색 박스 가로길이
  - height : 배경색 박스 세로길이
- style="border : 3px solid 색깔; border-radius:실수px
  - border : 테두리 생성
  - border-radius : 테두리의 모서리를 둥글게 만듬(숫자 크기up->더 둥글게)
- style="background-color : 색깔 ; padding:실수px; margin:실수px; text-align:위치"
  - padding : 박스 만들기
    - background-color : 박스 배경색
    - padding : 실수px : 박스 두께
      - padding: Apx Bpx : A 상하 B 좌우 두께
    - text-align:위치 : 왼쪽/가운데/오른쪽 등 위치
    - margin : 실수px : 여백 지정
      - margin-top : 위 글씨와 거리
      - margin-bottom : 아래 글씨와 거리
      - margin-left : 왼쪽 글씨와 거리 - margin-right : 오른쪽 글씨와 거리
      - margin-legt: auto; margin-right: auto : 중앙
      - margin: Apx Bpx : A 상하 B 좌우 거리
    - text-align:위치 : 왼쪽/가운데/오른쪽 등 위치
    - font-size: Apt/px : 글씨 크기
    - font-weight: A : 글씨 두께/100단위로 써야함(100-900)

# CSS 문법2

- <head> 안에 <style>
    - <head><style>  글씨 { color: 색깔; }</style></head>
- 아래와 같이 태그를 직접 지정하고 스타일 넣으면 태그 전체에 적용됨
  - 글씨 {text-align: right; /_ 요소 안의 텍스트를 오른쪽 정렬 _/}
- *{text-align: A ;} *를 앞에 붙여주면 전체 태그 적용

# 시맨틱 태그

- 개념
  - div태그와 유사한 역할
  - 태그의 이름이으로 웹 페이지의 구조를 파악 가능

# CSS 문법3 [0408.html/0408.css 참고]

- <head> 안에 <link> 삽입 <herf> 속성 사용해 스타일 시트 파일의 경로를 지정
  - style.css 파일에서 스타일을 가져오기
    - <link rel="대상" href="이미지 주소(stylesheet)">
    - <link rel="대상" herf="CSS파일 만들기">
- font-family : 텍스트에 사용할 폰트 종류 지정
- 주로 p 태그 안에 넣음 p{코드;}
  - p{line-height:Apx;} : 텍스트 줄 간격 지정(px/%)
  - p{letter-spacing:Bpx;} : 문자 사이의의 간격 넓히기(px/%/em)
  - p{texy-decoration: 스타일 지정;} : underline(밑줄)/line-though(취소선)/overline(중앙선) 등
- 주로 a 태그 안에 넣음 a{코드;}
  - text-decoration: none : 링크 밑줄 없애기
  - font-style: 스타일 지정 : 텍스트 스타일(기울임) 정함(기울임:italic/보통/normal/해제obiaue)
  - texy-shadow: Apx Bpx Cpx 색깔 : 텍스트에 그림자 추가(A:가로/B:세로/C:흐림정도)
  - font-family: "글씨체",serif; : 글씨체 바꾸기(밑에 글씨체 코드 복붙해야함)

# table [0415-1.html 참고] 

- 표를 만드는 데에 사용하는 태그
  - <table></table> 태그 안에 <tr> 태그 여러 개 중첩시켜 행 만들기-><td> 태그 여러 개 중첩시켜 셀을 만듬
  - 스타일은 table 태그 안에 집어 넣음
    - border : 테이블 셀들의 테두리 두께를 지정
    - colspan : 셀이 차지하는 열의 수를 지정
    - rowspan : 셀이 차지하는 행의 수를 지정
  - 시맨틱 태그
  - thead: "테이블의 header"를 나타내는 태그/표의 맨 위에 위치/일반적으로 표의 열 제목을 포함
  - tbody : "테이블 본문"을 나타내는 태그/표의 행(row)들을 포함
  - tfoot : "테이블 footer"를 나타내는 태그/표의 맨 아래에 위치/일반적으로 표의 요약 정보나 추가적인 정보를 포함
- caption 태그 : 캡션을 달기 위해 사용
- th 태그 : 강조용으로 사용
  ※ h: header
- colgroup, col : 열 전체에 효과를 줄 때 사용/div의 일종
  - col은 colgroup 태그 내부에 와야함
  - col은 열의 개수만큼 써야함
  - col 태그를 사용하여 특정 열의 속성을 정의->해당 열의 모든 셀(cell)에 일괄적으로 적용

# form [0415-2.html 참고]

- <form> 태그
  - 사용자로부터 입력을 받을 수 있는 요소
  - form 태그 안
    - fieldset : 그룹화된 요소들을 하나로 묶어주는 역할/영역을 그룹으로 나누어 레이아웃을 구성
    - legend : fieldset 요소 내에서 그룹의 제목을 정의/시각적으로 그룹의 제목을 표시
- <label> 태그
  - 태그는 사용자가 입력해야 할 내용에 대한 설명 제공
  - label 태그에 input 포함할 때
    - <label> 이메일 : <input type="email" name="email"> </label>
  - lable 태그와 input을 따로 작성할 때
    - <input type="checkbox" id="agree">
      <label for="agree">동의합니다.</label>

# input태그1 [0415-2.html 참고]

- 태그는 데이터를 입력할 수 있는 영역/type 속성을 사용하여 입력 필드의 종류를 지정
- 태그의 종류
  - text : 일반적인 텍스트를 입력 받을 때 사용
  - password : 비밀번호를 입력 받을 때 사용/입력한 값이 별표(*)로 표시
  - email : 이메일 주소를 입력 받을 때 사용
  - tel : 전화번호를 입력 받을 때 사용
  - 선택형 input 태그
    - checkbox : 다중 선택이 가능한 옵션을 제공할 때 사용(네모 안에 체크 표시시)
    - radio : 여러 옵션 중 하나만 선택할 때 사용(동그라미 안에 체크 표시)
    - name : 속성을 사용해서 동일한 input 그룹끼리 묶어줄 때 사용(통일해줘야함)
    - checked : 해당 옵션이 기본적으로 선택되어 있음
  - input 태그의 속성
    - placeholder : 입력란에 안내 문구를 표시
    - autfocus : 입력 요소가 페이지 로드 시 자동으로 선택 

# button

- 태그는 클릭 가능한 버튼을 만드는 태그/버튼은 텍스트,이미지,아이콘 등의 콘텐츠를 포함할 수 있음
  - type 속성은 버튼의 유형을 지정
    - submit : 폼을 제출할 때 사용/form 태그의 action에 지정한 서버로 전송
    - reset : 폼의 내용을 초기화할 때 사용
    - button : 클릭 가능한 버튼을 만들 때 사용

# input태그2 [0417.html 참고]

- input태그의 종류
  - number : 사용자로부터 숫자 값을 입력 받을 때 사용/문자나 다른 유형의 데이터를 입력할 수 없음
  - min max 속성: 입력할 수 있는 숫자의 범위를 제한/사용자가 이 범위를 벗어난 값을 입력하면 브라우저는 경고를 표시
  - step 속성: 입력 값이 증가 또는 감소하는간격을 설정할 수 있음
               [예시] step="2"를 설정하면 사용자가 입력하는 값은 항상 2의 배수가 됨
  - value 속성: 입력 필드의 초기값을 설정/사용자가 아무런 값을 입력하지 않은 경우 이 값이 기본으로 표시