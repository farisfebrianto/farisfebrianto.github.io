---
layout: post
title:  "Menyembunyikan Drive Letter Windows"
categories: windows
---

Banyak cara yg bisa kita gunakan untuk menyembunyikan drive letter partisi drive Windows agar seperti sistem operasi Linux. Akibat dari tindakan tersebut, Windows tidak meng-assign partisi tersebut sehingga seolah-olah tidak ada dan tentunya tidak mudah diketahui oleh orang lain. <!--more--> Nah caranya ada dua macam, bisa melalui CMD atau lewat GUI.

## Cara Text Mode

1. Klik Start, Klik Run dan ketik `diskpart` dan Enter.
2. Akan muncul jendela DOS, ketik `list volume`, Enter.
3. Jika Drive E yang akan disembunyikan, pilih dulu volumenya, ketik `select volume 3`, dan  tekan Enter.
4. Ketik `remove letter E` , tekan Enter.
5. Untuk mengembalikan kembali Drive E yang disembunyikan, pilih  volume yang disembunyikan misal volume E ketik `select volume 3` kemudian `assign letter E`, Enter.

## Cara GUI

1. Klik Start, Klik kanan pada My Computer pilih Manage.
2. Setelah muncul window Computer Management pilih Storage, Disk Management.
3. Pilih salah satu partisi misalnya Drive E, kemudian klik kanan pilih Change Drive Letter and Paths.
4. Pilih Remove maka Drive akan menghilang dan untuk mengembalikannya pilih add dan OK

Lakukan  cara di atas bila ingin menyembunyikan drive lainnya. Dengan cara ini anda dapat menyembunyikan lebih dari satu drive. Jangan khawatir jika komputer anda minta reboot karena dengan melakukan ini data anda tidak akan terhapus atau hilang, efeknya seperti meng-hidden partisi. Saya sarankan jangan menyembunyikan drive c (drive sistem) supaya tidak membingungkan anda.
