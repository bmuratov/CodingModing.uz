---
layout: post
title: "Barcha elementlarni o'z ichiga olgan namuna post"
description: "CodingModingda ishlatilishi mumkin bo'lgan barcha elementlar quyida ko'rsatib o'tilgan"
og_image: "documentation/sample-image.jpg"
tags: [design, jekyll]
---

 CodingModing Jekyll'ining default sintaksis yoritgich `gem`(paket) Rouge'ni ishlatadi. Paket o'zida kerakli stillarni jamlagan.
 `highlight` tegi kod blokini bildiradi. Quyidagi kod `highlight html`  tegi orqali yozilgan. :

{% highlight html %}
<!-- Bu izoh -->
<div class="grid">
  <h1>HTML dagi sarlavha</h1>
  <p>
    Bu paragraf.
  </p>
</div>
{% endhighlight %}

## Sarlavhalar

Shablonda 3 hil sarlavhalar mavjud:

## Eng katta sarlavha (1-daraja)
### O'rtacha Sarlavha (2-daraja)
#### Eng kichik Sarlavha (3-daraja)

{% highlight markdown %}
## Eng katta sarlavha (1-daraja)
### O'rtacha Sarlavha (2-daraja)
#### Eng kichik Sarlavha (3-daraja)
{% endhighlight %}

## Ro'yhatlar

Tartiblanmagan ro'yxat namunasi:
* Tartiblanmagan ro'yxat elementi 1
* Tartiblanmagan ro'yxat elementi 2
* Tartiblanmagan ro'yxat elementi 3
* Tartiblanmagan ro'yxat elementi 4

Tartiblangan ro'yxat namunasi:
1. Tartiblangan ro'yxat elementi 1
2. Tartiblangan ro'yxat elementi 2
3. Tartiblangan ro'yxat elementi 3
4. Tartiblangan ro'yxat elementi 4

{% highlight markdown %}
* Tartiblanmagan ro'yxat elementi 1
* Tartiblanmagan ro'yxat elementi 2

1. Tartiblangan ro'yxat elementi 1
2. Tartiblangan ro'yxat elementi 2
{% endhighlight %}

## Matndan parcha (quote)

Matndan parcha/Iqtibos quyidagi ko'rinishga ega:

> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.

{% highlight markdown %}
> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.
{% endhighlight %}

## Media

Rasmlar HTML dagi standart  `<img>` tegi orqali qo'yilishi mumkin.
Agar qo'ygan rasmingiz kattalashishini  hohlasangiz, quyidagi atributlarni yozing:
If you wish that an image can be enlarged on click use the image include tag. You can pass 3 variables:
- `path`: Rasmning joylashuvi.
- `path-detail`: Kattaroq rasm joylashuvi.
- `alt`: Rasm haqida

{% include image.html path="documentation/sample-image.jpg" path-detail="documentation/sample-image@2x.jpg" alt="Namuna rasm" %}

{% highlight html %}
{% include image.html path="documentation/sample-image.jpg" path-detail="documentation/sample-image@2x.jpg" alt="Namuna rasm" %}
{% endhighlight %}

Videolar standart holatda adaptiv dizayn ga ega (4x3 standart, 16x9 ham qilinishi mumkin).

<div class="embed-responsive embed-responsive-16by9">
<iframe src="https://www.youtube.com/embed/vO7m8Hre72E?modestbranding=1&autohide=1&showinfo=0&controls=0" frameborder="0" allowfullscreen></iframe>
</div>

{% highlight html %}
<div class="embed-responsive embed-responsive-16by9">
<iframe src="url-to-video" frameborder="0" allowfullscreen></iframe>
</div>
{% endhighlight %}
