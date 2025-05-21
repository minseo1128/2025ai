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
  - select  : 드롭다운 목록을 만들 때 사용/option 태그로 드롭다운 목록을 생성
  - datalist : input 태그와 함께 사용하여 입력 가능한 값 목록을 제공/select와 유사하나, 키보드로 값을 입력하는 것도 가능
    - input의 list와 datalist의 id가 일치해야함
  - textarea : 태그는 여러 줄의 긴 텍스트를 입력 받을 때 사용
      rows 속성은 텍스트 영역의 줄 수를, cols 속성은 텍스트 영역의 칸 수를 지정
  

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

# CSS + @

- cursor 속성
  - auto : 기본값/브라우저가 자동으로 커서 모양을 결정
  - pointer : 링크가 있는 요소 위에 마우스가 올라갈 때 손가락 모양으로 변경
  - move : 이동 가능한 요소 위에 마우스가 올라갈 때 십자가 모양으로 변경
  - text : 텍스트가 입력 가능한 요소 위에 마우스가 올라갈 때 I자 모양으로 변경
  - wait : 브라우저나 시스템이 작업을 처리 중일 때 시계 모양으로 변경
  - help : 도움말이 필요한 요소 위에 마우스가 올라갈 때 물음표 모양으로 변경
  - not-allowed : 사용 불가능한 요소 위에 마우스가 올라갈 때 금지 모양으로 변경
  - cell : 엑셀에서 자주 사용함/+ 모양
- border
  - 테두리 두께
  - border-style/border-width/border-color 세 가지 옵션을 각각 따로 사용하는 것으로 분리도 가능
  - border-radius 속성은 px가 아닌 % 단위로도 조절 가능
  - 가로세로 다르게 조절 가능/top-left, bottom-left 등 한 모서리만 적용 가능
  - box-sizing:border-box; : 크기를 아무리 설정해도 고정(안바뀜)
- width, height
  - px : 고정된 크기를 설정함
  - % : 웹 브라우저나 부모의 크기에 비례하여 크기가 조절됨
- rgba
  - red green blue의 비율로 색상을 표현하는 방법
  - 색상을 red 등의 이름이 아니라 숫자로도 지정 가능
  - 알파채널로 투명도 조절 가능
- **margin-left:auto; margin-right:auto; : 가운데 정렬**
  - margin: 0 auto; : 가운데 정렬

# overflow

- overflow : 속성은 태그의 내용이 태그의 크기보다 넘칠 때 어떻게 처리할지를 지정하는 속성

  - overflow: visible : 기본값/내용이 태그의 크기를 초과하더라도 그대로 표시
  - overflow: hidden : 내용이 크기를 초과하는 부분은 잘림
  - overflow: scroll : 내용이 크기를 초과하는 경우 스크롤바가 표시
  - overflow: auto : 내용이 크기를 초과하는 경우 스크롤바가 표시O/크기를 초과하지 않는 경우는 스크롤바가 표시X

# 블록레벨과 인라인레벨

- 블록레벨
  - 블록레벨 태그는 화면 전체의 가로폭을 차지하는 태그/각 태그를 작성할 때마다 새로운 줄에서 내용이 작성
    - <div> : 시맨틱태그
    - <p> : 문장이나 단락을 나타내는 태그
    - <h1>~ <h6>
    - <ul> / <ol> / <li>
    - <table> / tr
- 인라인레벨
  - 인라인레벨 태그는 텍스트의 일부로 취급/내용 만큼만 영역을 차지/텍스트로 취급/다른 인라인레벨 태그와 같은 줄에 위치
  - width/height/margin/padding 속성 적용X
    - <a>
    - <span>
    - <img>
    - <label> / <input> / <button>

# display

- 태그의 표시 방법을 지정
  - display: block : 블록 레벨 요소로 지정/화면 전체의 가로폭을 차지, 새로운 줄에서 시작
  - display: inline : 인라인 레벨 요소로 지정/내용만큼의 가로폭을 차지, 다른 요소와 같은 줄에 위치
  - display: inline-block : 인라인 레벨 요소처럼 내용만큼의 가로폭을 차지, 블록 레벨 요소의 CSS를 적용할 수 있음
  - display: none : 요소를 화면에서 숨김

# 레이아웃 구성

- display: inline-block : div 박스를 한 줄에 나열하면 박스를 글씨로 취급하므로 여백이 생김
    - 해결 방법 : 부모의 font-size를 0으로 설정해야함

# CSS 선택자 [0513.html 참고]

- .mom > div{} : mom의 자식인 div만을 선택
- .mom div{} : mom의 후손인 모든 div를 선택
- 속성 선택자 : [attribute=value] - 지정한 속성 값을 가진 요소 선택
- 자식 선택자 : parent > child - 지정한 부모 요소의 직계 자식 요소 선택
- 자손 선택자 : ancestor descendant - 지정한 조상 요소의 후손 요소 선택
- 인접 형제 선택자 : prev + next - 지정한 형제 요소 중 첫 번째 인접 요소 선택
- 일반 형제 선택자 : prev ~ siblings - 지정한 형제 요소 모두 선택

# CSS 가상 클래스 [0513.html 참고]

-특정 조건에서 스타일을 바꾸는 것것
  - :hover : 마우스 커서가 올라가면 스타일 적용
  - :active : 마우스 클릭 중일 때 스타일 적용
  - :nth-child() : 모든 자식 중에서 지정된 순서의 태그를 선택
    - [예시] nth-child(2) : 부모 요소의 두 번째 자식을 선택(*종류에 상관없이 부모 요소의 모든 자식을 대상으로 적용)
  - :nth-of-type() : 지정된 유형의 태그 중에서 원하는 위치의 태그를 선택
    - [예시] nth-of-type(2) : 지정된 태그 중 2번째 태그를 선택(*같은 종류의 태그끼리만 비교)
  - even or (2n) 짝수 태그들을 선택
  - odd or (2n+1) : 홀수 태그들을 선택
  - :focus : 사용자가 키보드를 사용하여 요소를 선택하거나 마우스를 사용하여 클릭하여 요소에 포커스가 이동할 때 적용 주로 입력 요소나 링크 등 사용자가 상호작용할 수 있는 요소에 사용
  - :link : 링크가 걸려있는 상태일 때 스타일 적용
  - :visited : 링크를 방문한 적이 있을 때 스타일 적용
  - :first-child : 첫 번째 자식 요소에 스타일 적용
  - :last-child : 마지막 자식 요소에 스타일 적용

# 가상요소 [0515.html 참고]

- ::before : 요소의 내용 이전에 콘텐츠를 삽입
- ::after : 요소의 내용 이후에 콘텐츠를 삽입
- ::selection : 텍스트를 드래그하여 선택된 부분에 스타일을 적용
- ::first-letter : 요소의 첫 번째 글자에 스타일을 적용
- ::first-line : 요소의 첫 번째 줄에 스타일을 적용

# flex [0520.html/11회차 flex 참고]

- flex
  - 태그들을 한 줄로 유연하게 배치하기 위한 방법
  - 부모 밑의 자식 태그들을 한 방향(수평 혹은 수직)으로 정렬하고 간격을 조절할 때 사용
    (*주로 부모에게 적용 - display:flex; : 부모한테 적용 -> 자식이 모두 정렬)
- justify-content
  - 가로 축에서 태그들을 어떻게 정렬할지 설정
    - flex-start : item들을 왼쪽으로 정렬
    - flex-end : item들을 오른쪽으로 정렬
    - center : item들을 중앙으로 정렬
    - **space-between** : item들 한줄로 사이(between)에 고르게 간격을 두고 배치
    - space-around : item들의 주위(around)에 고르게 간격을 두고 배치 첫 번째와 마지막 item은 고정된 간격을 갖게 됨
    - space-evenly : 아이템들의 사이와 양 끝에 균일한 간격을 만들어줌 이 기능을 지원하지 않는 브라우저가 있음
- align-items 
  - gap : item 사이가 멀어짐(margin과 다름)
  - stretch : flex item들을 cross axis에 맞게 늘림/기본값으로 설정되어 있음/cross axis의 높이를 자동으로 맞춰주는 역할
  - flex-start : 시작점에 item들을 정렬
  - flex-end : 끝점에 item들을 정렬
  - center : 중앙에 item들을 정렬
  - baseline : item들의 텍스트 베이스라인을 맞춤