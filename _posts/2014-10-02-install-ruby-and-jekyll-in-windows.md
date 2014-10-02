---
layout: post
title: "Install Ruby and Jekyll in Windows"
date: 2014-10-02 19:18:47 +0700
comments: true
categories: tutorial
tags: install ruby in windows, intall jekyll in windows
---


Keren kan kalau melihat alamat blog yang kaya gini [menikdp.github.io][blogku] ? muehehehe Saya coba mencari kesana kemari *alah*, sepertinya jarang ada tutorial tentang github dan jekyll yang berbahasa Indonesia, apalagi tutorial Ruby :( Postingan ini menjawab keresahan buat para pemula yang bener-bener mulai dari nol seperti saya (apalagi dengan OS Windows!), dan juga sebagai *self reminder* kalau-kalau saya inul si Jepie dan lupa cara bikin blog yang kece ini :P Langkah-langkahnya kadang mudah <del>kadang bikin gemes</del>, *you wanna try?*

1. Buat akun di [Github][github], setelah melakukan verifikasi email, bisa langsung membuat repositori(selanjutnya kita bilang repo aja ya biar gak rempong) baru di [Github][github]. Punya saya nama repo-nya yaitu menikdp.github.io

2. *Download* [Ruby Installer dan Ruby DevKit][devkit] sekalian. Jangan lupa <b>perhatikan versi Ruby dan versi DevKitnya</b> ya. Setelah itu, jalankan *installer* Ruby sampai selesai. Kemudian dobel klik juga pada devKit, taruh di folder yang gampang diketik (yang namanya simpel dan tidak mengandung spasi), punya saya di C:/sites

3. Melalui cmd atau *command prompt*, masuk ke folder C:/sites (sengaja saya kumpulin jadi satu), *clone* repo yang ada di [Github][github] dengan cara : 
{% highlight ruby%}
	git clone git@github.com:username/<repo>.git
{% endhighlight %}

4. Download [Poole][poole], kemudian ekstrak ke folder yang di-*clone* tadi. Jadi isi ekstrak [Poole][poole] ada di dalam folder menikdp.github.io

5. Masih di cmd, install Jekyll dengan ketik `gem install Jekyll` kemudian tunggu sampai prosesnya selesai. 

6. Kalo nurut [disini][winjekyll], mustinya install Python juga, tapi saya lewati saja. Hanya saja di `_config.yml` pada bagian pygment nilainya diganti false

7. Ketik `jekyll serve` di cmd, akan muncul keterangan kalau servernya udah jalan

8. Ketik `localhost:4000` di browser, tadaaaa :D

9. Push folder ke github dengan cara :
{% highlight ruby %}
	git add .
git commit -m "your comment here"
git push origin master
{% endhighlight %}

10. Ketik nama folder tadi di browser, kalau berhasil nanti munculnya sama dengan yang di localhost:4000


Fiuuuh, lumayan rempong yak? Sampai sini dulu yak. Penjelasan lainnya nyusul, saya mau belajar lagi sama Tuan nyiahahaha XD Kalau ada yang kurang jelas atau gak beres, monggo colek saya di menik.damayanti.p@gmail.com


[blogku]: http://menikdp.github.io
[github]: http://github.com
[poole]: https://github.com/poole/poole
[winjekyll]: http://jekyllrb.com/docs/installation/
[devkit]: http://rubyinstaller.org/downloads/