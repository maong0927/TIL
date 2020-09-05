# ❤️ 9/5 Today I Learned ❤️

# 🌈 오늘한 것

- [x]  CSS 공부
- [x]  git 공부

# ❤️ CSS 공부 ❤️

```css
div {
  background-image: url('../img/bg.png');
	background-repeat: no-repeat;
}
```

- repeat : 이미지가 가로 세로 바둑판 식으로 반복되어 보임.
- repeat-x : 이미지가 x축(가로)로만 반복
- repeat-y : 이미지가 y축(세로)로만 반복
- no-repeat : 이미지를 한번만 보여주고 반복 x
- inherit : 부모 속성 상속

```css
div {
  background-position: 100% 16px; /* x y */
  /* 또는 */
  background-position: right bottom;
}
```

- 좌표 값이 양수로 커질 수록 x축에서는 오른쪽, y축에서는 아래쪽으로 이동. 0보다 작은 음수로 내려갈수록 각각 왼쪽, 위쪽으로 이동
- 단위를 %로 줄 경우에는 %는 이미지 사이즈를 기준으로 변환됩니다. 때문에 만약 x 축을 100%로 주게 될 경우, 이미지의 가장 오른쪽으로 보여지게 되고, 50%를 줄 경우 가운데 정렬이 됩니다. 이를 'left','center','right'로 표현 할 수 있습니다.
- px : 맨 위, 왼쪽을 px의 절대값으로 이미지 이동
- left, right = 0%, 100% - x 축에서 쓸 수 있는 속성
- top, bottom = 0%, 100% - y 축에서 쓸 수 있는 속성 / 가장 위에서 보여줄지 아래에서 보여줄지 선택가능
- center : x축 y축 둘다 사용 가능.

```css
div {
  background-attachment : local;
}
```

- background - attachment

→ scroll : 요소에 고정 

→ local : 요소 안 내용에 고정 

![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.16.19.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.16.19.png)

- border : div 나 여러 요소에 테두리 속성을 줄 수 있는 border 속성을 살펴 봄.

    ![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.30.30.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.30.30.png)

- border 을 구성하는 세가지 요소 : 각 변마다 선의 굵기(width), 선의 형태(style), 선의 색상(color)를 지정 가능

```css
div {
  border-top-width : 3px;
	border-right-style : dotted;
	border-bottom-color : #aaa;
	border-top : 3px dotted red; /* top style 한꺼번에 지정 */
	border-width: 3px; /* 모든 변이 3px의 굵기 */
	border-width: 3px 1px 2px; /* top, ( right + left ), bottom */
	border-color : red #333; /* (top + bottom) / (right+ left)*/
	border : 1px solid red; /* 모든 변에 동일하게 적용 */
}
```

![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.32.32.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.32.32.png)

```css
<div style="margin-bottom:10px;">Box 1</div>
<div style="margin-top:30px;">Box 2</div>
```

→ Box 1 과 Box 2 중 큰 간격으로 벌어짐. 

![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.46.20.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__4.46.20.png)

- padding : 패딩은 요소 안, 내부 여백을 주는 속성임. 작성하는 방식은 margin과 동일

```css
div {
  padding-top: 10px;
  padding-bottom: 10px;
  /* 또는 */
  padding: 10px 0;
}
```

![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__5.26.27.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__5.26.27.png)

![%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__5.26.49.png](%E2%9D%A4%EF%B8%8F%209%205%20Today%20I%20Learned%20%E2%9D%A4%EF%B8%8F%20d693ba85ba544305b05bd51b4c97ac30/_2020-09-05__5.26.49.png)

- margin - 바깥 여백.
- margin과 margin이 만날 경우, 각 요소의 바깥 여백이 만날 경우 둘 중 큰 여백에 맞춰짐.
- padding - 안 여백.
- width, height - 너비와 높이.
- 박스의 실질적인 전체 너비와 높이는 margin을 제외한 (width 또는 height) + padding + border의 값.
- 정확한 너비/높이 값을 주기 위해서는 padding과 border를 고려해가며 주어야 함.

→ 속성을 주는 요소는 보통 다른 요소들을 감싸는 가장 큰 요소와, 공통으로 사용하는 요소를 먼저 주는 것이 작업 상 편합니다.

# ❤️ HTML 공부 ❤️

- **Semantic Web  :** 컴퓨터가 웹 페이지를 단순한 HTML의 나열이 아니라 '의미'를 가진 무언가로 해석할 수 있는 것을 의미
- **<header> 태그** : '머리글'이라고 생각하시면 이용하기 편할 것 같습니다. 웹 페이지든 특정 글 영역이든 해당 부분의 머리글 역할을 한다고 보시면 됩니다. 그리고 <nav> 태그를 담는 용도로도 사용됩니다.
- **<nav> 태그** : navigator 의 약자에서 따온 <nav> 태그 입니다. <nav> 태그는 주로 '메뉴'들을 담는 역할을 합니다. 다른 페이지로 navigate 해주는 역할을 하는 것이지요.
- **<aside> 태그** : 사이드 메뉴로 주로 많이 쓰이지만 본래 역할은 본문과 구분되는 별도의 한 구역을 만드는 데 사용합니다.
- **<article> 태그** : 기사 영역, 즉 본문이 들어가는 영역입니다.
- **<footer> 태그** : 주로 문서 하단에 위치하며 주로 작성자 / copyright / 관련 문서 링크 등의 정보를 담는 영역입니다. 실제로 문서 하단에 위치할 필요는 없으며 앞서 말한 정보들을 담고 있으면 <footer> 태그로 감쌀 수 있습니다.
- **<section> 태그 :** section 자체가 부분, 구획 이라는 뜻을 지니고 있기 때문에 이 태그야말로 정말 구역을 나누는 태그라고 할 수 있습니다. 챕터, 메뉴 탭으로 구성된 요소에서 특정 탭이 가리키는 영역 등 유사한 내용을 담고 있는 요소들을 하나로 묶어주는 역할을 하는 태그입니다.

[[HTML을 배워보자] 구역을 만드는 태그(header, nav, aside, section, article)](https://m.blog.naver.com/PostView.nhn?blogId=tk2rush90&logNo=221212779027&proxyReferer=https:%2F%2Fwww.google.com%2F)

- tag == $0의 의미!

[WWW.PHPSCHOOL.COM](https://www.phpschool.com/gnuboard4/bbs/board.php?bo_table=tipntech&wr_id=81340)

→ gnb, lnb, snb, fnb 용어 설명 

[GNB·LNB·SNB·FNB 용어 설명](https://youngkeol.tistory.com/29)

# ❤️ GIT 공부 ❤️

[3. 브랜치 병합하기 【튜토리얼1: 브랜치를 사용해 보자] | 누구나 쉽게 이해할 수 있는 Git 입문~버전 관리를 완벽하게 이용해보자~ | Backlog](https://backlog.com/git-tutorial/kr/stepup/stepup2_4.html)

1. isseu1 branch 의 변경사항을 master branch에 병합하기

```bash
$ git merge <commit>
```

→ 지정한 commit 내용이 HEAD 가 가리키고 있는 branch에 들어감. 

```bash
$ git checkout master
```

→ master branch에 HEAD 가 위치하게 만듦. 

```bash
$ git merge issue1
```

→ 이제 'master' 브랜치가 가리키는 커밋이 'issue1'과 같은 위치로 이동함. 

## 🍒 branch 병합하기

[6. 병합할 때 발생하는 충돌 해결하기 【튜토리얼1: 브랜치를 사용해 보자] | 누구나 쉽게 이해할 수 있는 Git 입문~버전 관리를 완벽하게 이용해보자~ | Backlog](https://backlog.com/git-tutorial/kr/stepup/stepup2_7.html)

[7. rebase로 병합하기 【튜토리얼1: 브랜치를 사용해 보자] | 누구나 쉽게 이해할 수 있는 Git 입문~버전 관리를 완벽하게 이용해보자~ | Backlog](https://backlog.com/git-tutorial/kr/stepup/stepup2_8.html)