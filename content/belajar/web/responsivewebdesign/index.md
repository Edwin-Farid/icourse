---
title: "Responsive Web Design"
date: 2023-06-20T14:14:05+08:00
draft: false

tags: ["Web Developer", "CSS", "CSS3", "CSS Lanjutan", "Responsive Web"]

series: ["Web Developer"]
series_order: 5
---

## Responsive Web Design

Sebuah pendekatan yang menyarankan agar proses perancangan dan pembangunan
sebuah web app harus merespon terhadap perilaku pengguna berdasarkan dari ukuran
layer, platform dan orientasi layer.

![Display Size](img/display_size.png)

![Display Size](img/display_size2.png)

![Display Size](img/display_size3.png)

## Prinsip Responsive Web Design

### Viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

| Viewport Meta Tag                               | Tanpa Viewport Meta Tag                                     |
| ----------------------------------------------- | ----------------------------------------------------------- |
| ![Viewport meta tag](img/viewport_meta_tag.png) | ![Tanpa viewport meta tag](img/tanpa_viewport_meta_tag.png) |

### Breakpoint

![Breakpoint](img/breakpoint.png)

### Media Query

```css
@media (min-width: 576px) {
}

@media (min-width: 768px) {
}

@media (min-width: 992px) {
}

@media (min-width: 1200px) {
}

@media (min-width: 1400px) {
}
```

### Fixed vs Fluid Layout

![Fixed vs Fluid Layout](img/fixed_fluid_layout.png)

### Mobile First Design

![Mobile First Design](img/mobile_first_design.png)

![Why Mobile](img/why_mobile.png)
