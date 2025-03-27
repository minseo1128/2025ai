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

- <p style="color : 색깔></p> : 색상 바꾸기
- <p style="color : 색깔;background-color:배경색깔;width:원하는 크기px;height:원하는 높이px"> darkslateblue </p></h3>
    - color : 색깔 : 글씨색
    - background-color : 배경색
    - width : 배경색 박스 가로길이
    - height : 배경색 박스 세로길이
