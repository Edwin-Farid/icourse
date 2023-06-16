---
title: "Dasar CSS (Cascading Style Sheets)"
date: 2023-06-11T19:16:42+08:00
draft: false

tags: ["Web Developer", "CSS", "Dasar CSS"]

series: ["Web Developer"]
series_order: 2
---

## Pengenalan CSS

- Bahasa yang digunakan untuk menentukan tampilan dan gaya elemen-elemen pada
  halaman web.
- CSS bukan bahasa pemrograman

## Jenis-jenis CSS

- Inline CSS
- Internal CSS
- Eksternal CSS

## Anatomi CSS

![CSS Anatomy](img/cssanatomy.png)

## Selector

### Selector sederhana

Memilih element berdasarkan tag, id, kelas dan universal

|                                  |                                  |                                  |
| -------------------------------- | -------------------------------- | -------------------------------- |
| ![Selector 1](img/selector1.png) | ![Selector 2](img/selector2.png) | ![Selector 3](img/selector3.png) |
| ![Selector 4](img/selector4.png) | ![Selector 5](img/selector5.png) |                                  |
|                                  |                                  |                                  |

### Selector Combinator

#### Descendant

Descendant selector (spasi) => pemilihan secara keturunan
![Descendant Selector](img/descendant_selector.png)

#### Child

Child selector (>) => pemilihan elemen yang merupakan anak dari element tertentu
![Child Selector](img/child_selector.png)

#### Adjacent Sibling

Adjacent Sibling Selector (+) => pemilihan berdasarkan saudara element terdekat
![Adjacent Sibling](img/adjancent_selector.png)

#### General Sibling

General Sibling Selector (~) => pemilihan berdasarkan saudara element berikutnya
![General Sibling](img/general_sibling.png)

### Selector Attribute

Dimungkinkan untuk menata elemen HTML yang memiliki atribut atau nilai atribut
tertentu.

|                                                   |                                                  |
| ------------------------------------------------- | ------------------------------------------------ |
| ![Attribut Selector ](img/attribut_selector1.png) | ![Attribut Selector](img/attribut_selector2.png) |
|                                                   |                                                  |

## Psuedo-class

Kelas semu yang dimiliki oleh element html, yang membuat kita dapat
mengimplementasikan style pada Keadaan tertentu dari elemen tersebut

### Psuedo-class yang berhubungan dengan link

#### :link

style default pada sebuah link (a yang memiliki href)

#### :hover

Style Ketika kursor mouse berada di atas elemen

#### :active

style Ketika sebuah link di-klik

#### :visited

style Ketika sebuah link sudah pernah dikunjungi (mengguanakaan browser yang
sama)

### Psuedo-class yang berhubungan dengan posisi element

#### :first-child

Memilih elemen pertama dari sebuah parent (elemen pembungkusnya)

#### :last-child

Memilih elemen terakhir dari sebuah parent

#### :nth-child(n)

memilih element ke-n dari sebuah parent, dimana n bisa (1), (2)…..atau bisa
menggunakan pola (2n), (3n+1) atau (odd) dan (even)

## Specificity CSS

Setiap deklarasi css (selector) memiliki berat yang berbeda. Berat tersebut
menentukan seberapa spesifik elemen yang dipilih oleh selector

![Hirarki Kekhususan 1](img/hirarki_kekhususan1.png)
![Hirarki Kekhususan](img/hirarki_kekhususan2.png)
