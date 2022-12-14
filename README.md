[![Netlify Status](https://api.netlify.com/api/v1/badges/d07cf9d9-8012-4144-ba84-a8af40458941/deploy-status)](https://app.netlify.com/sites/transcendent-naiad-733465/deploys)

# ๐ iPad

์์ดํจ๋ ์ ํ ํ์ด์ง๋ฅผ ๋ง๋๋ ์์ ์๋๋ค.

[DEMO](https://transcendent-naiad-733465.netlify.app/)

![Screenshots](./images/screenshot1.jpg)

### Reset.css

๊ฐ ๋ธ๋ผ์ฐ์ ์ ๊ธฐ๋ณธ ์คํ์ผ์ ์ด๊ธฐํํฉ๋๋ค.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css" />
```

### Google Fonts

Apple SF Pro ํฐํธ๋ ๊ณต์  ๋ฐ ๋ฐฐํฌํ  ์ ์๊ธฐ ๋๋ฌธ์,  
๊ฐ์ฅ ์ ์ฌํ ์น ํฐํธ๋ก ๋์ฒดํฉ๋๋ค.

์๋ฌธ: [Roboto](https://fonts.google.com/specimen/Roboto)
ํ๊ธ: [Noto Sans KR](https://fonts.google.com/noto/specimen/Noto+Sans+KR)

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;700&family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
```

### ์คํ ๊ทธ๋ํ ๋ฐ ํธ์ํฐ ์นด๋ ์ ๋ณด

์นํ์ด์ง๊ฐ ์์ ๋ฏธ๋์ด๋ก ๊ณต์ ๋  ๋ ์ฐ์ ์ ์ผ๋ก ํ์ฉ๋๋ ์ ๋ณด๋ฅผ ์ง์ ํฉ๋๋ค.

```html
<!--Open Graph-->
<meta property="og:type" content="website" />
<meta property="og:site_name" content="Apple (KR)" />
<meta property="og:title" content="iPad 10.2" />
<meta property="og:description" content="๊ฐ๋ ฅํ A13 Bionic ์นฉ์ ํ์ฌํ iPad. ์ผํฐ ์คํ์ด์ง ๊ธฐ์ ์ด ์ ์ฉ๋ 12MP ์ธํธ๋ผ ์์ด๋ ์ ๋ฉด ์นด๋ฉ๋ผ, True Tone ๋์คํ๋ ์ด ๊ธฐ์  ๋ฐ 64GB ์ ์ฅ ์ฉ๋๊น์ง ๊ฐ์ท์ต๋๋ค." />
<meta property="og:image" content="./images/ipad-seo.png" />
<meta property="og:url" content="https://www.apple.com/kr/ipad-10.2/" />

<!--Twitter Card-->
<meta property="twitter:card" content="summary" />
<meta property="twitter:site" content="Apple (KR)" />
<meta property="twitter:title" content="iPad 10.2" />
<meta property="twitter:description" content="๊ฐ๋ ฅํ A13 Bionic ์นฉ์ ํ์ฌํ iPad. ์ผํฐ ์คํ์ด์ง ๊ธฐ์ ์ด ์ ์ฉ๋ 12MP ์ธํธ๋ผ ์์ด๋ ์ ๋ฉด ์นด๋ฉ๋ผ, True Tone ๋์คํ๋ ์ด ๊ธฐ์  ๋ฐ 64GB ์ ์ฅ ์ฉ๋๊น์ง ๊ฐ์ท์ต๋๋ค." />
<meta property="twitter:image" content="./images/ipad-seo.png" />
<meta property="twitter:url" content="https://www.apple.com/kr/ipad-10.2/" />
```
### Sprite Icon Animation

์ฌ๋ฌ ์ด๋ฏธ์ง๋ฅผ ํ ์ด๋ฏธ์ง๋ก ํฉ์ณ ๊ด๋ฆฌํ๋ ๋ฐฉ์์ **์ด๋ฏธ์ง ์คํ๋ผ์ดํธ ๊ธฐ๋ฒ** ์ด๋ผ๊ณ  ํฉ๋๋ค.

<img src="./images/sprite_apps.png" alt="์ด๋ฏธ์ง ์คํ๋ผ์ดํธ" width="300" />

```css
@keyframes sprite-icon {
  /* 1~10 */
  0.00% { background-position: 0 0; }
  1.67% { background-position: -100px 0; }
  3.33% { background-position: -200px 0; }
  5.00% { background-position: -300px 0; }
  6.67% { background-position: -400px 0; }
  8.33% { background-position: -500px 0; }
  10.00% { background-position: 0 -100px; }
  11.67% { background-position: -100px -100px; }
  13.33% { background-position: -200px -100px; }
  15.00% { background-position: -300px -100px; }

  /* 11~20 */
  16.67% { background-position: -400px -100px; }
  18.33% { background-position: -500px -100px; }
  20.00% { background-position: 0 -200px; }
  21.67% { background-position: -100px -200px; }
  23.33% { background-position: -200px -200px; }
  25.00% { background-position: -300px -200px; }
  26.67% { background-position: -400px -200px; }
  28.33% { background-position: -500px -200px; }
  30.00% { background-position: 0 -300px; }
  31.67% { background-position: -100px -300px; }

  /* 21~30 */
  33.33% { background-position: -200px -300px; }
  35.00% { background-position: -300px -300px; }
  36.67% { background-position: -400px -300px; }
  38.33% { background-position: -500px -300px; }
  40.00% { background-position: 0 -400px; }
  41.67% { background-position: -100px -400px; }
  43.33% { background-position: -200px -400px; }
  45.00% { background-position: -300px -400px; }
  46.67% { background-position: -400px -400px; }
  48.33% { background-position: -500px -400px; }

  /* 31~40 */
  50.00% { background-position: 0 -500px; }
  51.67% { background-position: -100px -500px; }
  53.33% { background-position: -200px -500px; }
  55.00% { background-position: -300px -500px; }
  56.67% { background-position: -400px -500px; }
  58.33% { background-position: -500px -500px; }
  60.00% { background-position: 0 -600px; }
  61.67% { background-position: -100px -600px; }
  63.33% { background-position: -200px -600px; }
  65.00% { background-position: -300px -600px; }

  /* 41~50 */
  66.67% { background-position: -400px -600px; }
  68.33% { background-position: -500px -600px; }
  70.00% { background-position: 0 -700px; }
  71.67% { background-position: -100px -700px; }
  73.33% { background-position: -200px -700px; }
  75.00% { background-position: -300px -700px; }
  76.67% { background-position: -400px -700px; }
  78.33% { background-position: -500px -700px; }
  80.00% { background-position: 0 -800px; }
  81.67% { background-position: -100px -800px; }

  /* 51~60 */
  83.33% { background-position: -200px -800px; }
  85.00% { background-position: -300px -800px; }
  86.67% { background-position: -400px -800px; }
  88.33% { background-position: -500px -800px; }
  90.00% { background-position: 0 -900px; }
  91.67% { background-position: -100px -900px; }
  93.33% { background-position: -200px -900px; }
  95.00% { background-position: -300px -900px; }
  96.67% { background-position: -400px -900px; }
  98.33% { background-position: -500px -900px; }
}
```

JS๋ก ๊ฐ ํ๋ ์ ์์น ๋ฐ ์์ฑ๊ฐ ์ฝ๊ฒ ๋ง๋ค๊ธฐ

```js
let x = 0
let y = 0
let frames = ''
for (let i = 0; i < 60; i += 1) {
  // frames += `${(100 / 60 * i).toFixed(2)}% { background-position: ${x}px ${y}px; }<br />` // HTML์ผ๋ก ์ถ๋ ฅ!
  frames += `${(100 / 60 * i).toFixed(2)}% { background-position: ${x}${x === 0 ? '' : 'px'} ${y}${y === 0 ? '' : 'px'}; }\n`
  if (x <= -500) {
    x = 0
    y -= 100
    continue // ํ์ฌ ๋ฐ๋ณต์ ์ข๋ฃํ๊ณ  ๋ค์ ๋ฐ๋ณต์ผ๋ก ๋์ด๊ฐ๊ธฐ!
  }
  x -= 100
}
// document.body.innerHTML = frames // HTML์ผ๋ก ์ถ๋ ฅ!
console.log(frames)
```

### IntersectionObserver

[IntersectionObserver(์์์ ๊ฐ์์ฑ ๊ด์ฐฐ)](https://heropy.blog/2019/10/27/intersection-observer/)  
๋ธ๋ผ์ฐ์  ๋ทฐํฌํธ(Viewport)์ ์ค์ ํ ์์(Element)์ ๊ต์ฐจ์ ์ ๊ด์ฐฐํ์ฌ, ์์๊ฐ ๋ณด์ด๋์ง ๋ณด์ด์ง ์๋์ง ๊ตฌ๋ณํ๋ ๊ธฐ๋ฅ.

```js
// ์์์ ๊ฐ์์ฑ ๊ด์ฐฐ ๋ก์ง!
const io = new IntersectionObserver(entries => {
  // entries๋ `io.observe(el)`๋ก ๋ฑ๋ก๋ ๋ชจ๋  ๊ด์ฐฐ ๋์ ๋ฐฐ์ด.
  entries.forEach(entry => {
     // ์ฌ๋ผ์ง ๋.
    if (!entry.isIntersecting) {
      return
    }
    entry.target.classList.add('show')
  })
})
// ๊ด์ฐฐํ  ์์๋ค ๊ฒ์
const infoEls = document.querySelectorAll('.info')
// ๊ด์ฐฐ ์์!
infoEls.forEach(el => io.observe(el))
```
