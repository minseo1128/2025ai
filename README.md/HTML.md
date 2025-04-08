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

# CSS 문법3(0408.html/0408.css 참고)

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

