---
layout: post
title: "Membuat Aplikasi dengan Ruby on Rails"
date: 2015-05-22 13:05:32 +0700
comments: true
categories: 
tags: 
thumbnail:
---

Membuat aplikasi/project di RoR sangat mudah, karena segala sesuatunya seringkali menggunakan perintah *generate*. Untuk orang awam seperti saya, hal ini sangatlah menyenangkan, setidaknya lumayan untuk menghindari typo dalam penulisan nama class. RoR menggunakan konsep MVC (Model View Controller), yang intinya antara model (database) dan view(yang tampak/ditampilkan di layar) akan dijembatani oleh controller. Sebelumnya saya pernah mencoba belajar konsep MVC menggunakan CI, tapi yagitudeh, banyakan bingungnya hahaha Untuk pemula banget seperti saya, mungkin bisa belajar terlebih dahulu di [{{site.data.links.codecademy.label}}]({{ site.data.links.codecademy.href}}){:target="_blank"}.

Berikut langkah-langkah dasar membuat aplikasi dengan RoR :

1. Buka terminal, ketik `rails new <nama_projet>`, kemudian enter. Maka secara otomatis, komputer akan men-generate sebuah project sesuai dengan `<nama_project>`, misalnya blog.

2. Ketik `bundle install` untuk menginstall gem-gem dasar yang dibutuhkan.

3. Buat database dengan perintah `rake db:create`, kemudian ketikkan `rake db:migrate`

4. Buat model dengan menjalankan perintah `rails generate model <nama_model>`, hasilnya bisa dilihat di folder db/migrate/...<nama_model> dan juga di folder app/models dengan nama file <nama_model>.rb

File yang ada di db/migrate bisa diutak-atik untuk menentukan jumlah kolom dalam tabel model, juga untuk relasinya dnegan tabel yang lain. Oh iya, tidak perlu membuat id_number di sini, karena secara otomatis sudah ditambahakan setiap kita bikin tabel. Setelah selesai menambahkan kolom ataupun relasi, jangan lupa di eksekusi dengan perintah `rake db:migrate`

 File di folder app/models berfungsi sebagai tempat kita mendefinisikan perintah/fungsi apa saja yang bisa dilakukan untuk tabel tersebut, misal show untuk menampilkan semua yang ada di tabel, new untuk menambah data di tabel, dan seterusnya.

 5. Buat controller dengan perintah `rails generate controller <nama_controller>s`

bikin mew app
bikin db untuk app
	rake db:create trus rake db:migrate
bikin model
	rails generate model Article
	buka db/migrate/...article tambahkan apa aja yang hendak dimasukkan di tabel article
	rake db:migrate
	atau bisa juga dnegan scaffold
bikin controller