### 1일차

### 팝업 P-1

![깃헙2](https://github.com/GEUMAIN/webDesignPop_Tab/assets/128437656/8e32f5bd-42f0-4b85-9149-bf709ecee7cc)

---

### HTML

```html
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>웹디자인기능사 팝업 P-1</title>
    <link href="https://webfontworld.github.io/gmarket/GmarketSans.css" rel="stylesheet">
    <link rel="stylesheet" href="CSS/style.css">
</head>

<body>
    <div id="wrap">
        <header id="header">
            <h1 class="logo"></h1>
            <nav class="nav"></nav>
        </header>

        <article id="slider"></article>

        <main id="contents">
            <section class="content1"></section>
            <section class="content2"></section>
            <section class="content3">
                <a href="#" class="popup-btn">팝업</a>
            </section>
        </main>

        <footer id="footer">
            <div class="footer1"></div>
            <div class="footer2"></div>
            <div class="footer3"></div>
        </footer>

        <div class="popup-view">
            <a href="#" class="popup-close">닫기</a>
        </div>
    </div>

    <script src="JS/script.js"></script>
</body>

</html>
```

---

### CSS

```css
* {
    margin: 0;
    padding: 0;
    font-family: 'GmarketSans';
}

a {
    text-decoration: none;
    color: #000;
}

#wrap {
    width: 1200px;
    margin: 0 auto;
}

#header {
    width: 100%;
    display: flex;
}

#header .logo {
    width: 20%;
    height: 100px;
    background-color: #efefef;
}

#header .nav {
    width: 80%;
    height: 100px;
    background-color: #e3e3e3;
}

#slider {
    width: 100%;
    height: 300px;
    background-color: #d9d9d9;
}

#contents {
    width: 100%;
    display: flex;
}

#contents .content1 {
    width: 33.3333%;
    height: 200px;
    background-color: #d1d1d1;
}

#contents .content2 {
    width: 33.3333%;
    height: 200px;
    background-color: #c7c7c7;
}

#contents .content3 {
    width: 33.3333%;
    height: 200px;
    background-color: #bcbcbc;
}

#footer {
    width: 100%;
    display: flex;
}

#footer .footer1 {
    width: 20%;
    height: 100px;
    background-color: #b1b1b1;
}

#footer .footer2 {
    width: 60%;
    height: 100px;
    background-color: #a3a3a3;
}

#footer .footer3 {
    width: 20%;
    height: 100px;
    background-color: #9d9d9d;
}

#wrap {
    position: relative;
}

.content3 {
    display: flex;
    align-items: center;
    justify-content: center;
}

.popup-btn {
    background-color: rgba(255, 255, 255, 0.6);
    padding: 10px;
    display: inline-block;
}

.popup-view {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    width: 400px;
    height: 400px;
    background-color: #a2a2a2;
    border: 3px solid #000;
    z-index: 1000;
    display: none;
}

.popup-close {
    background-color: #fff;
    padding: 10px;
    display: inline-block;
}
```

---

### JavaScript

```jsx
window.onload = function () {
    document.querySelector(".popup-btn").addEventListener("click", function (e) {
        e.preventDefault();
        document.querySelector(".popup-view").style.display = "block";
    });
    document.querySelector(".popup-close").addEventListener("click", function (e) {
        e.preventDefault();
        document.querySelector(".popup-view").style.display = "none";
    });
}
```

---

### 탭 T-1

![깃헙3](https://github.com/GEUMAIN/webDesignPop_Tab/assets/128437656/55e4909c-0af6-4cfd-8d4a-b781fb469f71)

---

### HTML

```html
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>웹디자인기능사 슬라이드 T-1</title>
    <link href="https://webfontworld.github.io/gmarket/GmarketSans.css" rel="stylesheet">
    <link rel="stylesheet" href="CSS/style.css">
</head>

<body>
    <div id="wrap">
        <header id="header">
            <h1 class="logo"></h1>
            <nav class="nav"></nav>
        </header>

        <article id="slider">
        </article>

        <main id="contents">
            <section class="content1">
                <div class="tab-menu">
                    <div class="tab-btn">
                        <ul>
                            <li class="active"><a href="#">탭메뉴1</a></li>
                            <li><a href="#">탭메뉴2</a></li>
                        </ul>
                    </div>
                    <div class="tab-cont">
                        <div>
                            탭메뉴1<br>탭메뉴1<br>탭메뉴1<br>탭메뉴1
                        </div>
                        <div>
                            탭메뉴2<br>탭메뉴2<br>탭메뉴2<br>탭메뉴2
                        </div>
                    </div>
                </div>
            </section>
            <section class="content2"></section>
            <section class="content3"></section>
        </main>

        <footer id="footer">
            <div class="footer1"></div>
            <div class="footer2"></div>
            <div class="footer3"></div>
        </footer>

    </div>

    <script src="JS/script.js"></script>
</body>

</html>
```

---

### CSS

```css
* {
    margin: 0;
    padding: 0;
    font-family: 'GmarketSans';
}

a {
    text-decoration: none;
    color: #000;
}

#wrap {
    width: 1200px;
    margin: 0 auto;
}

#header {
    width: 100%;
    display: flex;
}

#header .logo {
    width: 20%;
    height: 100px;
    background-color: #efefef;
}

#header .nav {
    width: 80%;
    height: 100px;
    background-color: #e3e3e3;
}

#slider {
    width: 100%;
    height: 300px;
    background-color: #d9d9d9;
}

#contents {
    width: 100%;
    display: flex;
}

#contents .content1 {
    width: 33.3333%;
    height: 200px;
    background-color: #d1d1d1;
}

#contents .content2 {
    width: 33.3333%;
    height: 200px;
    background-color: #c7c7c7;
}

#contents .content3 {
    width: 33.3333%;
    height: 200px;
    background-color: #bcbcbc;
}

#footer {
    width: 100%;
    display: flex;
}

#footer .footer1 {
    width: 20%;
    height: 100px;
    background-color: #b1b1b1;
}

#footer .footer2 {
    width: 60%;
    height: 100px;
    background-color: #a3a3a3;
}

#footer .footer3 {
    width: 20%;
    height: 100px;
    background-color: #9d9d9d;
}

.tab-menu {
    padding: 20px;
}

.tab-menu .tab-btn ul {
    display: flex;
}

.tab-menu .tab-btn li {
    list-style: none;
}

.tab-menu .tab-btn li.active a {
    text-decoration: underline;
}

.tab-menu .tab-btn li a {
    display: block;
    padding: 10px;
    background-color: #6b6b6b;
}

.tab-menu .tab-cont>div {
    padding: 10px;
    background-color: #b0b0b0;
    line-height: 1.6;
}
```

---

### JavaScript

```jsx
const tabBtn = document.querySelectorAll(".tab-btn > ul > li");
const tabCont = document.querySelectorAll(".tab-cont > div");

tabCont.forEach(el => el.style.display = "none");
tabCont[0].style.display = "block";

tabBtn.forEach((tab, index) => {
    tab.addEventListener("click", (e) => {
        e.preventDefault();
        tabBtn.forEach(tab => tab.classList.remove("active"));
        tab.classList.add("active");

        tabCont.forEach(cont => cont.style.display = "none");
        tabCont[index].style.display = "block";
    });
});
```
