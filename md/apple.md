# 🟢 Introduction

- 과제: Apple 메인 페이지 구현
- 날짜: 2024년 10월 20일
- 배포 주소: https://photoby64.github.io/homework/apple/apple.html

# 🟢 Table of Contents

1. [마크업](#-마크업)
2. [HTML](#-html에-대하여)
3. [CSS](#-css-설명)
4. [결과](#-결과)
5. [문제점 및 구현 과정에서의 어려움](#-문제점-및-구현-과정에서의-어려움)
6. [과제를 마치며..](#-과제를-마치며)
   <br />
   <br />

## 🧐 마크업

![마크업](./../md/images/apple-markup.jpg)
<br>

```
 <article class="card card-black ipod-pro">
        <h2 class="card-headline">iPad Pro</h2>
        <p class="card-subhead">놀라우리만치 얇다.<br />엄청나게 강력하다.</p>
        <p class="card-subhead2">출시일 추후 공개</p>
        <div class="button-wrapper">
          <a role="button" class="button button-blue button-left" href="https://www.apple.com/kr/ipad" aria-label="아이패드 프로 더 알아보기">더 알아보기</a>
          <a role="button" class="button button-blue button-right" href="https://www.apple.com/kr/shop/buy-ipad" aria-label="아이패드 프로 가격 보기">가격 보기</a>
        </div>
      </article>
```

<br><br>

## 🏘️ HTML

1. `article`태그를 사용

- 각각의 카드는 같은 스타일의 디자인이지만 다른 내용으로 일종의 기사와 같은 형태를 띠고 있고 있다 생각했다.

2. `h2`를 사용.

- 제품의 이름은 컨포넌트 관점에서 가장 중요하다고 생각해 제목요소로 작성했다.

3. `p`태그를 사용.

- 제품의 설명은 `h3`, 부제목을 하기엔 그 다음에 나올 내용이 없고, 본문의 내용을 함축하는 것도 아니기에 p태그를 선택했다.

4. button 컴포넌트는 `<a>`요소로 마크업.

- 처음엔 `<button>`으로 구상해봤는데 이 버튼은 단순 링크를 연결해주는 버튼인데 이 기능이 접근성 측면에서 적합한가를 고민하며 인터넷을 검색하다가 유튜브 ['AOA11y 채널'](https://www.youtube.com/watch?v=dhsr2LGTA-s)의 영상을 참고하여 최종적으로 `<a>`요소로 작성했다.

---

<br />
<br />

## 🛋️ CSS

1. 카드 컴포넌트

- 카드 컨포넌트는 배치되는 방식이 설정에 따라 유연하게 변할 수 있는 flex를 사용했다.

2. 버튼 컴포넌트
   button-blue, button-black을 나누어서 각각 hover되는 버튼 스타일을 따로 설정했다.

3. 레이아웃

- grid를 사용하여 Small Screen(1024px 미만)일때는 1열로 배치하고, Large Screen(1024px 이상)일때는 2열로 구성했다.

---

<br />
<br />

## 🌈 결과

### **1024px 이하 Small Screen**

![스몰](./../md/images/small-screen.gif)

### **1024px 이상 Large Screen**

![라지](./../md/images/large-screen.gif)

### **1024px 이상 X-Large Screen**

![라지2](./../md/images/large-screen-2.gif)

  <br />
  <br />

---

## 💦 문제점 및 구현 과정에서의 어려움

1. `<br>`태그의 문제점
   제품의 내용의 줄바꿈을 위해 사용한 `<br>`태그가 보이스오버를 실행시키고 확인해보니 **"그룹이다비어있음. 그룹이 다 비어있음에 있습니다."** 라고 나왔다.

2. 줄바꿈
   도저히 구현이 안됐다...

---

<br />
<br />

## 🙂 과제를 마치며..

이번 과제는 좀 더 오래 고민하고 생각하며 재미있게 도전해본 과제였다. 중간에는 도저히 구현이 안되서 포기할까 생각했는데 하루라는 시간이 더 있어서 그런지 완성이 중요한게 아니라 끝까지 도전해보자!! 라는 마음으로 다시 시도해볼 수 있었다. 근데 하도 고민을 오해 하다보니까 md파일 제대로 작성할 시간이 많이 없어서 아쉬웠다.

---

<br />
<br />
