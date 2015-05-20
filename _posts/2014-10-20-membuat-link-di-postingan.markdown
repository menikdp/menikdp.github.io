---
layout: post
title: "Membuat Link di Postingan"
date: 2014-10-20 03:06:25 +0700
comments: true
categories: tutorial
tags: link di ruby, tutorial link
thumbnail:
---
Berdasarkan postingan yang ini, kita bisa ngumpulin link-link yang biasa kita pake kemudian kita tinggal panggil aja. Nah kalo link-ya cuma kepake sekali, mending ditulis di postingan aja lah ya hahaha

Cara bikin link di postingan sebenarnya gampang, kok. Misal dalam kalimat "Untuk tutorial lengkapnya bisa dilihat di sini", kita mau bikin link dalam kata `di sini`. Penulisannya jadi kayak gini :
{% gist 61bada87cf9469f358a9 %}

Nah,nanti di bagian bawah postingan, kita deskripsikan link itu mengarah kemana, contohnya kata `di sini` merujuk ke `http://guides.rubyonrails.org/index.html`, maka kita tulis kode ini di bagian paling bawah postingan :
{% gist c5ec32aec8a2e8a08b35 %} , jadi deh tulisan `di sini` akan nge-link ke alamat website tadi :D

Gampang, kan? 