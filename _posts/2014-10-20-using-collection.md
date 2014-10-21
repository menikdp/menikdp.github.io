---
layout: post
title: "Using Collection"
date: 2014-10-20 02:56:58 +0700
comments: true
categories: 
tags: 
---
Kemarin saya habis tanya ama Tuan, masak iya tiap mau bikin link harus ditulis satu persatu di tiap bagian yang mau disambungkan? Kemudian di deskripsiin satu persatu di bagian bawah kode postingan? Kata Tuan sih bisa pakai collection. Jadi link-link yang akan biasa kita gunakan dikumpulin jadi satu, kemudian tinggal manggil aja. Saya mah gak mudeng, tau-tau udah dibikinin aje ama Tuan, saya tinggal manggil dan nambahin aja hahahaha

Cara bikinnya gampang :

1. Buat folder baru di direktori blog, kalau di blog saya sih namanya `_data`, jadi di dalam menikdp.github.io ada tambahan folder itu.

2. Buat file dengan format `.yml` (saya kurang ngerti dengan jenis-jenis file di RoR muehehehe), taruh di dalam folder `_data`. Misal `links.yml` . Nah, kita nanti bakal masukin link-link yang biasa kita gunakan disini.

3. Buka file `links.yml` dengan text editor (notepad++ atau apalah yang sejenis). Disini kita bakal mendefinisikan link-link yang akan kita gunakan. Untuk setiap link, ada 3 bagian (saya sendiri tidak tau nama persisnya apa, ini hanya berdasarkan perkiraan saya saja XD) yaitu nama-label,nama-panggilan, dan link yang dituju.

<div class="highlight"><pre><code class="language-ruby" data-lang="ruby"><span class="nb">blogku:<br>label: blogku<br>href: http://menikdp.github.io</span></code></pre></div>
