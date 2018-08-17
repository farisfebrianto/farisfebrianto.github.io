---
layout: post
title:  "Konversi Bilangan"
categories: math
---

Konversi bilangan merupakan problem dasar selain konversi suhu ataupun konversi satuan. Bilangan-bilangan non desimal ini biasanya diperlukan untuk hal-hal khusus seperti pada pemrograman yang biasanya menggunakan bilangan biner dan heksa dibanding bilangan desimal atau pada standar pewarnaan RGB yang menggunakan bilagan heksa desimal. <!--more--> Nah biasanya konversi bilangan muncul dalam soal-soal ujian atau lebih spesifik lagi untuk menghitung network (jaringan), agar tidak bingung penghitungan dasar konversi bilangan ini dikelompokkan menjadi 4 bagian.

1. Biner yaitu bilangan berbasis dua yang terdiri dari 0 dan 1
2. Oktal yaitu bilangan berbasis delapan yang terdiri dari 0, 1, 2, 3, 4, 5, 6, dan 7
3. Desimal yaitu bilangan berbasis sepuluh yang terdiri dari 0, 1, 2, 3, 4, 5, 6, 7, 8, dan 9
4. Heksadesimal yaitu bilangan berbasis enam belas yang terdiri dari 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A (10), B (11), C (12), D (13), E (14), dan F (15)

## A. BILANGAN DESIMAL

### 1. Bilangan Desimal ke Biner
Contoh 254 (10) = ….. (2)

Bagi bilangan tersebut dengan dua sampai bilangan tersebut tidak bisa lagi dibagi dua (kurang dari dua) dengan mencatat setiap sisa pembagian.

254 : 2 = 127 sisa 0

127 : 2 = 63 sisa 1

63 : 2 = 31 sisa 1

31 : 2 = 15 sisa 1

15 : 2 = 7 sisa 1

7 : 2 = 3 sisa 1

3 : 2 = 1 sisa 1

1 : 2 = sisa 1

Jadi 254 (10) = 11111110 (2) diurutkan dari sisa pembagian terakhir sebagai MSB (Most Significant Bit)

### 2. Bilangan Desimal ke Oktal

Contoh 254 (10) = ….. (8)

Bagi bilangan tersebut dengan delapan sampai bilangan tersebut tidak bisa lagi dibagi delapan (kurang dari delapan) dengan mencatat setiap sisa pembagian.

254 : 8 = 31 sisa 6

31 : 8 = 3 sisa 7

3 : 8 = sisa 3

Jadi 254 (10) = 376 (8) diurutkan dari sisa pembagian terakhir sebagai MSB (Most Significant Bit)

### 3. Bilangan Desimal ke Heksadesimal

Contoh 254 (10) = ….. (16)

Bagi bilangan tersebut dengan enam belas sampai bilangan tersebut tidak bisa lagi dibagi enam belas (kurang dari enam belas) dengan mencatat setiap sisa pembagian.

254 : 16 = 15 sisa 14 atau E

15 : 16 = sisa 15 atau F (lihat tabel di atas)

Jadi 254 (10) = FE (16) diurutkan dari sisa pembagian terakhir sebagai MSB (Most Significant Bit)

## B. BILANGAN BINER

### 1. Bilangan Biner ke Desimal

Contoh 1100100 (2) = ….. (10)

Kalikan bilangan-bilangan tersebut dengan dua yang telah dipangkatkan sesuai urutan 0,1,2,4, dan seterusnya kemudian menjumlahkannya.

0 x 2 pangkat 0 = 0

0 x 2 pangkat 1 = 0

1 x 2 pangkat 2 = 4

0 x 2 pangkat 3 = 0

0 x 2 pangkat 4 = 0

1 x 2 pangkat 5 = 32

1 x 2 pangkat 6 = 64

4+32+64 = 100

Jadi 1100100 (2) = 100 (10)

### 2. Bilangan Biner ke Oktal

Contoh 1100100 (2) = ….. (8)

Pisahkan bilangan tersebut menjadi beberapa bagian dimulai dari bilangan paling kanan (LSB). Setiap bagian terdiri dari tiga angka, jika bagian terakhir (paling kiri) kurang dari tiga angka, dapat menambahkan bilangan 0.
1100100 dipisahkan menjadi tiga bagian menjadi 1-100-100 atau 001-100-100

100 (2) = 4 (8)

100 (2) = 4 (8)

001 (2) = 1 (8)

Jadi 1100100 (2) = 144 (8)

### 3. Bilangan Biner ke Heksadesimal

Contoh 1100100 (2) = ….. (16)

Pisahkan bilangan tersebut menjadi beberapa bagian dimulai dari bilangan paling kanan (LSB). Setiap bagian terdiri dari empat angka, jika bagian terakhir (paling kiri) kurang dari empat digit, dapat menambahkan bilangan 0.

1100100 dibagi empat bagian menjadi 110-0100 atau 0110-0100

0100 (2) = 4 (16)

0110 (2) = 6 (16)

Jadi 1100100 (2) = 64 (16)

## C. BILANGAN OKTAL

### 1. Bilangan Oktal ke Desimal

Contoh 200 (8) = ….. (10)

Kalikan bilangan-bilangan tersebut dengan delapan yang telah dipangkatkan sesuai urutan 0,1,2,4, dan seterusnya kemudian jumlahkan hasilnya.

0 x 8 pangkat 0 = 0

0 x 8 pangkat 1 = 0

2 x 8 pangkat 2 = 128

Jadi 200 (8) = 128 (10)

### 2. Bilangan Oktal ke Biner

Contoh 200 (8) = ….. (2)

Dengan cara melihat tabel di atas kemudian tulis dalam tiga digit, setelah itu diurutkan (disatukan).

0 (8) = 000 (2)

0 (8) = 000 (2)

2 (8) = 010 (2)

Jadi 200 (8) = 010000000 (2) atau 10000000 (2)

### 3. Bilangan Oktal ke Heksadesimal

Contoh 200 (8) = ….. (16)

Konversikan ke Desimal atau ke Biner terlebih dahulu kemudian konversi lagi ke Heksadesimal. Jika konversi dilakukan ke bilangan Biner, maka hasil konversi dipisahkan menjadi beberapa bagian dimana setiap bagian terdiri dari empat angka dimulai dari sebelah kanan (LSB) kemudian dikonversi ke Heksadesimal.

200 (8) = 010000000 (2)

010000000 menjadi 0-1000-0000 atau 0000-1000-0000

0000 (2) = 0 (16)

1000 (2) = 8 (16)

0000 (2) = 0 (16)

Jadi 200 (8) = 080 (16) atau 80 (16)

## D. BILANGAN HEKSADESIMAL

### 1. Bilangan Heksadesimal ke Biner

Contoh FA (16) = ….. (2)

Masing-masing angka Heksadesimal dikonversi menjadi empat angka Biner

A (16) = 1010 (2)

F (16) = 1111 (2)

Jadi FA (16) = 11111010 (2)

### 2. Bilangan Heksadesimal ke Oktal

Contoh FA (16) = ….. (8)

Konversi bilangan tersebut ke Biner terlebih dahulu kemudian gunakan cara konversi bilangan Biner ke Oktal.

FA (16) = 11111010 (2)

11111010 menjadi 11-111-010 atau 011-111-010

010 (2) = 2 (8)

111 (2) = 7 (8)

011 (2) = 3 (8)

Jadi FA (16) = 372 (8)

### 3. Bilangan Heksadecimal ke Desimal

Contoh FA (16) = ….. (10)

Dengan cara mengalikan bilangan-bilangan tersebut dengan enam belas yang telah dipangkatkan sesuai urutan

0,1,2,4, dan seterusnya kemudian menjumlahkannya.

A x 16 pangkat 0 atau 10 x 16 pangkat 0 = 10

F x 16 pangkat 1 atau 15 x 16 pangkat 1 = 240

10+240 = 250

Jadi FA (16) = 250 (10)
