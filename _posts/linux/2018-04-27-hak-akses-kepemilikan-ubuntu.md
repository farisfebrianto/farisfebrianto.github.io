---
layout: post
title:  "Mengatur Hak Akses dan Kepemilikan di Terminal Ubuntu"
categories: Linux
image: hak-akses-kepemilikan-ubuntu.png
permalink: /hak-akses-kepemilikan-ubuntu/
comments: true
---

Sebagai pengguna Ubuntu, untuk mengubah hak akses dan kepemilikan lebih afdol kalau menggunakan perintah di terminal (command line) meskipun dengan GUI juga bisa, akan tetapi pada kebanyakan kasus kita diminta harus menggunakan terminal seperti mengerjakan tugas, laporan, dll. <!--more--> Perintah untuk mengubah hak akses dan kepemilikan ada 3 yaitu:

1. chmod – merubah hak akses, bisa juga disebut permission
2. chown – merubah kepemilikan user
3. chgrp – merubah kepemilikan grup

### Hak Akses (chmod)

Perintah chmod untuk file yaitu:

```
# chmod ugo+rwx namaFile
```

Sedangkan untuk folder adalah:

```
# chmod -R ugo+rwx namaFolder
```

Keterangan:

\# = tanda pagar merupakan tanda kalau perintah ini harus dijalankan dengan superuser, caranya kalian tambahkan perintah sudo sebelum kata chmod

-R = perintah ini untuk mengubah hak akses parent folder dan objek didalamnya
ugo = kepemilikan hak akses, boleh ditulis 1 atau lebih misal

```
sudo chmod u+rw,o+r namaFile
```

u = mengubah hak akses untuk ‘user’

g = mengubah hak akses untuk ‘group’

o = mengubah hak akses untuk ‘other’, other disini mengandung arti untuk ‘every one’

\+ = menambah properti hak akses, tanda ini bisa diganti – untuk mengurangi properti hak akses atau = untuk menyamakan sesuai properti. Properti yang dimaksud yaitu r, w, dan x

r = properti read

w = properti write

x = properti execute

Ada perintah chmod lain yaitu menggunakan kode biner yang sama penggunaannya dengan chmod ugo= dengan acuan

r w x

ugo 4 2 1

contoh kita ingin merubah properti rw—xr– menjadi –x—rwx kita menggunakan perintah

```
sudo chmod 107 namaFile
```

User mendapat 1 karena diberi hak execute, group mendapat 0 karena tidak diberi hak akses sama sekali, dan other mendapat 7 karena mendapat semua hak akses (rwx=4+2+1=7)

### Kepemilikan User (chown)

Perintah chown untuk file yaitu:

```
# chown namaUser namaFile
```

Untuk folder yaitu:

```
# chown -R namaUser namaFolder
```

### Kepemilikan Group (chgrp)

Perintah chown untuk file yaitu:

```
# chgrp namaGrup namaFile
```

Untuk folder yaitu:

```
# chgrp -R namaGrup namaFolder
```
