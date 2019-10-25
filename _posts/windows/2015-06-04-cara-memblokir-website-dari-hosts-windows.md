---
layout: post
title:  "Cara Memblokir Website dari Hosts Windows"
categories: Windows
image: blokir-website-dari-hosts-windows.png
permalink: /blokir-website-dari-hosts-windows/
comments: true
---

Blokir website ini sebenarnya hanya mengarahkan link-link tertentu agar mengarah ke alamat *dummy* seperti 127.0.0.1 (localhost) sehingga link tersebut seolah-olah down atau tidak bisa diakses. Biasanya tujuan pemblokiran ini antara lain agar saat browsing kita tidak terganggu iklan internet (blok host iklan) atau dalam rangka memblokir pemeriksaan keaslian suatu software, misalnya dalam tahap-tahap aksi ilegal cracking Adobe Photoshop.

<!--more-->

1. Pertama kalian masuk ke directory `C:\Windows\System32\drivers\etc` dan buka file hosts
2. Setelah anda membuka file hosts anda akan di suruh untuk memilih program untuk membukanya. Saya merekomendasikan memakai program Notepad bawaan Windows
3. Isikan alamat websites yang ingin anda blokir tetapi jangan lupa anda tambahi dengan 0.0.0.0 baru nama websites Contoh:
```
0.0.0.0 www.faceebook .com
```
4. Save file hosts, jika anda kesulitan dalam menyimpannya hal ini karena anda tidak mempunyai hak akses untuk write di folder tsb. Solusinya simpan di Documents kemudian replace file hosts dengan file yang sudah di-edit tadi. Dijamin PC yang telah anda program untuk memblokir websites tidak akan dapat membuka websites yang telah anda blokir, selamat mencoba.
