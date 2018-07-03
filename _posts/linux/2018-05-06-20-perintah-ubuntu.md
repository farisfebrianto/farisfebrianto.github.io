---
layout: post
title:  "20 Perintah CLI di Ubuntu"
categories: linux
---

### 1. adduser

```
$ adduser [options] namaUser
```

Adduser adalah perintah untuk menambahkan seorang user kedalam system.

Untuk membuat user di Ubuntu kita memerlukan akses root dengan perintah sudo. Saat membuat user kita diminta memasukkan password root dan password baru untuk user sekaligus informasi tambahan untuk user baru, kemudian ketikkan y dan enter jika selesai.

Untuk mencoba user baru tersebut kita ketikkan perintah login.

### 2. bc

```
$ bc [ - hlwsqv ] [log-options] [ file ...]
```

Bc adalah bahasa kalkulator untuk shell linux yang mendukung operasi matematika yang hampir sama dengan bahasa pemrograman C.

Kita bisa mencobanya untuk menyelesaikan operasi-operasi dasar matematika seperti penjumlahan dan perkalian. Untuk keluar dari bc kita ketikkan perintah quit

### 3. chmod

```
$ chmod [option] [mode] file
```

```
$ chmod [octal-mode] file
```

Chmod adalah perintah untuk merubah permission atau hak akses dari suatu file atau folder, yang bisa disimbolkan dengan mode (misal +x) maupun octal-number (misal 777).

Saya mencoba merubah hak akses file coba.txt agar semua bisa mengaksesnya (777) dari -rw-rw-r– menjadi -rwxrwxrwx, dimana r adalah read, w untuk write dan x untuk execute.

### 4. cp

```
$ cp [option] [source] [destination]
```

Cp adalah perintah untuk meyalin suatu file adan folder ketempat lain yang ditentukan.

Saya mencoba membuat file coba.txt dengan perintah touch kemudian menyalinnya menjadi file dengan nama tes.txt. Juga mencoba menyalinnya kefolder lain

### 5. df

```
$ df
```

Df yaitu perintah untuk melihat penggunaan space system disk.

Dengan perintah ini kalian bisa melihat semua kapasitas partisi dan disk yang masih kosong dan jumlah yang telah terisi.

### 6. dpkg

```
$ dpkg [option] action
```

Dpkg adalah package manager untuk Debian dan turunannya. Biasanya package software Debian berekstensi .deb, dpkg berguna untuk menginstal maupun meremove package software tersebut.

Contohnya kita mempunyai package softwate gstreamer di folder download, kita bisa menginstalnya dengan perintah sudo dpkg -i namaFile. Kekurangan dpkg yaitu sulit untuk menginstal package software yang tergantung (dependant) terhadap package software lain.

### 7. exit

```
$ exit
```

Exit yaitu perintah yang berguna untuk menghentikan normal proses maupun logout dari user.

Pada contoh diatas saya login menggunakan root dan caara untuk logout pada terminal yaitu dengan menggunakan perintah exit untuk kembali keuser biasa

### 8. free

```
$ free [options]
```

Free adalah perintah untuk menampilkan jumlah memory yang free dan digunakan oleh system yang secara default ditampilkan dalam satuan kilobytes.

Free mempunyai fungsi hampir sama dengan aplikasi System Monitor pada Ubuntu

### 9. halt

```
$ halt [options]
```

halt yaitu perintah untuk mematikan system dan memerlukan hak akses sebagai root.

### 10. history

```
$ history [options]
```

history berguna untuk menampilkan perintah apa saja yang pernah kita ketikkan dalam terminal. Antara satu user dengan user lain mempunyai history yang berbeda

Untuk menghapus history suatu user kita ketikkan perintah history –c

### 11. ifconfig

```
$ ifconfig namaInterface [options]
```

Ifconfig yaitu perintah untuk mengkonfigurasi network interface pada system, biasanya terdiri dari ethernet (eth), lo (loopback), dan wireless.

Jika hanya untuk melihat pengaturan dari network interface kita bisa menggunakan perintah ifconfig saja yang akan menampilkan pengaturan network interface secara mendetail.

### 12. last

```
$ last [namaUser (optional)]
```

Last yaitu perintah untuk melihat daftar terakhir user yang log in kedalam system

Kita bisa melihat dengan perintah last dapat diketahui dengan detail apa yang dilakukan user beserta waktunya.

### 13. lsb_release

```
$ lsb_release [options]
```

Yaitu perintah LSB (Linux Standard Base dan informasi spesifik distribution). Jika options tidak digunakan maka secara default -v yang akan ditampilkan.

Berikut ini opsi-opsi yang ada:

-v = melihat versi instalasi saat ini

-i = melihat distributor ID

-r = menampilkan release number

-a = menampilkan semua informasi LSB yang ada

### 14. mv

```
$ mv [options] [source] [destination]
```

Mv adalah perintah untuk memindahkan file atau foder ketempat baru bisa juga untuk merename file atau folder ketempat baru.

Pada contoh diatas kita akan memindahkan file mv.txt dari folder /home/sawah/Downloads ke /home/sawah/Documents

### 15. nano

```
$ nano [options] [[+line,column] namaFile]
```

Nano adalah shell text editor yang ringan dengan mempunyai fitur yang lengkap, bisa untuk mengedit, find, replace suatu plain text file. Misalnya jika kita melihat isi atau mengedit file /etc/profile maka tampilannya sebagai berikut

Perintah dibawah adalah shortcut-shortcut untuk mempercepat mengedit suatu text file tanda ^ maksudnya adalah Ctrl, misal untuk exit tertulis ^X yang berarti kalian harus menekan Ctrl+X

### 16. ps

```
$ ps [options]
```

Ps menampilkan informasi tentang proses yang dipilih. Secara default ps memilih semua process yang user IDnya sama

### 17. tar

```
$ tar [options] [file]
```

Tar adalah tool untuk pengarchivan file berupa tar (tarball). Perintah tar berguna untuk membuat atau mengekstrak tar file. Beberapa operasi utama tar :

-c = membuat archive baru

-t = daftar isi archive

-x = ekstrak file tar. Contohnya seperti gambar dibawah

### 18. top

```
$ top
```

Perintah top akan menampilkan semua process linux yang sedang berjalan dan secara real-time direfresh. Top mempunyai fungsi sama seperti task manager pada Microsoft Windows. Berikut screenshot process pada laptop saya.

### 19. uptime

```
$ uptime [options]
```

Perintah uptime berguna untuk menampilkan berpa lama system (komputer) dihidupkan. Untuk menampilkan secara friendly kita bisa menambahkan opsi -p seperi screenshot dibawah

### 20. vim

```
$ vim [options] [file]
```

Vim adalah text editor yang bisa digunakan untuk mengedit semua tipe plain text. Beberapa fiturnya yaitu undo, multi windows, syntax highlighting, filename completion dll. Misalnya kita ingin membuka atau mengedit file /etc/passwd

 Untuk keluar kita bisa mengetikkan perintah :quit
