---
layout: post
---

## ใน CSS 2.1 เราจะใช้สิ่งที่เรียกว่า “Layout Mode” 
---
layout: post
title: Grid in CSS
subtitle: ฝึกใช้ CSS Grid กันเถอะ
tags: [flex, css]
---

กลับมาอีกครั้งกับหมวด CSS ครับ วันนี้ผมจะมาลองเล่น Grid ใน CSS ดูกัน ส่วนบล็อคนี้จะเป็นเครื่องมือช่วยจำให้ผมนะครับ เผื่อใครอยากลองก็สามารถทำตามและลองเล่นไปด้วยกันได้ครับ

เอาล่ะ มาเริ่มกันเลย !!!!

เริ่มกันที่สร้าง html ขึ้นมาก่อน พร้อม CSS เริ่มต้นด้วย elements ประมาณนี้

```
  body {
    padding: 0;
    margin: 0;
    background-color: black;
  }

  .grid {
    display: grid;
  }

  .card {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    height: 100%;
    width: 100%;
    background-color: slategrey;
    transition: all 0.3s;
    cursor: pointer;
    font-size: 3rem;
  }

  .card:hover {
    box-shadow: rgba(2, 8, 20, 0.1) 0 0.255rem 1.1rem, rgba(2, 8, 20, 0.08) 0 0.255rem 1.1rem;
    transform: translateY(-5px) scale(1.1);
  }
 ```
 
 ```
   <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <link rel="stylesheet" href="style.css" />
      <title>Grid CSS</title>
    </head>
    <body>
      <div class="grid">
        <div class="card">1</div>
        <div class="card">2</div>
        <div class="card">3</div>
        <div class="card">4</div>
        <div class="card">5</div>
        <div class="card">6</div>
        <div class="card">7</div>
        <div class="card">8</div>
        <div class="card">9</div>
        <div class="card">10</div>
        <div class="card">11</div>
        <div class="card">12</div>
        <div class="card">13</div>
        <div class="card">14</div>
        <div class="card">15</div>
        <div class="card">16</div>
        <div class="card">17</div>
        <div class="card">18</div>
      </div>
    </body>
  </html>
 ```
 
## GAP
gap ใน CSS ที่ใช้ร่วมกับ display: grid นั้นจะเป็นเหมือนการเว้นช่องไฟระหว่าง Element ที่อยู่ใน grid ตัวอย่างเช่น
```
  .grid {
    display: grid;
    gap: 1rem;
  }
```

แปลว่าจะมีช่องว่างระหว่าง Element อยู่ 1 rem

ผลที่ได้

![preview picture](https://miro.medium.com/max/3000/1*dpz0XPVaO0OeSY5qhj7sNQ.png)

[Read more](https://medium.com/@pozterz.jojo/%E0%B8%9D%E0%B8%B6%E0%B8%81%E0%B9%83%E0%B8%8A%E0%B9%89-css-grid-%E0%B8%81%E0%B8%B1%E0%B8%99%E0%B9%80%E0%B8%96%E0%B8%AD%E0%B8%B0-6a18a05036da)
