---
title: "CSS 3"
date: 2023-06-16T20:42:40+08:00
draft: false

tags: ["Web Developer", "CSS", "CSS3", "Dasar CSS"]

series: ["Web Developer"]
series_order: 4
---

## CSS 3

Generasi ke-3 dari dari spesifikasi css

![CSS 2 VS CSS 3](img/css2vscss3.jpg)

Topik yang akan di bahas :

- Font Face
- Transform
- Transition
- Animation
- Flexbox

## Font Face

```html
font-family: "Arial Narrow", arial, sans-serif;
```

Kita juga bisa menggunakan font dari google

https://fonts.google.com

Menggunakan Teknik @font-face

![Font Face](img/font-face.png)

https://www.fontsquirrel.com/

## Transform

Memungkinkan kita dapat memanipulasi format visual (ukuran, bentuk, atau posisi)
dari elemen HTML

```html
transform: < fungsi >
```

Fungsi transform

- Scale => memberpesar / memperkecil
- Rotate => memutar
- Skew => membuat condong miring
- Translate => mengubah posisi

## Transition

Memungkinkan kita dapat mengubah nilai dari property HTLM secara halus

transition vs animation

### transition

Transition hanya mempunyai 2 keadaan yaitu keadaan awal dan keadaan akhir,
sedangkan animation bisa lebih

```html
transition: < durasi > [fungsi] [delay];
```

![Animatable](img/animatable.png)

![Non Animatable](img/non_animatable.png)

## Animation

![Animation](img/animation.png)

![Keyframe Animation](img/keyframeanimation.png)

![Animation Properties](img/animation_properti.png)

### Iteration Count

```css
<angka> | infinite
```

### Direction

```css
normal | reverse | alternate | alternate-reverse
```

### Fill-mode

```css
none | forwards | backwards | both
```

### Play-state

```css
running | paused
```

## Flexbox

Digunakan untuk memudahkan kita mengatur layout.

![Flexbox](img/flexbox1.png)

![Flexbox](img/flexbox2.png)

Sebuah modul layout yang dapat mengatur jarak dan penjajaran antar item adalam
sebuah container.

### Display

```css
.container {
  display: flex;
}
```

Membuat sebuah elemen parent menjadi sebuah flexbox dan membuat elemen-elemen di
dalamnya bisa berperilaku flex juga

### Flex-direction

![Flex-direction](img/flex_direction.png)

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

### Flex-direction

![Flex-wrap](img/flex_wrap.png)

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

### Justify Content

![Justify Content](img/justify_content.png)

### Align Items

![Align Items](img/align_items.png)
