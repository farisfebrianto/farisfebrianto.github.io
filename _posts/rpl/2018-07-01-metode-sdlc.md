---
layout: post
title:  "Metode Software Development Cycle (SDLC)"
categories: RPL
image: metode-sdlc.png
permalink: /metode-sdlc/
comments: true
---

Metode Software Development Cycle (SDLC) merupakan metode yang diterapkan dalam siklus pengembangan perangkat lunak agar mudah dibuat, dikembangkan, dan diperbaiki jika ditemukan bug didalanya. Ada banyak macam SDLC yang bisa dipakai seuai dengan kebutuhan atau tenggat waktu pengerjaan yang diperlukan. Masing-masing metode memiliki kelebihan dan kekurangan, sehingga banyak developer menggabungkan metode-metode tersebut agar terasa pas menurut mereka. <!--more--> Metode SDLC tersebut antara lain:

## 1. Waterfall

Metode ini merupakan metode tertua dalam rekayasa perangkat lunak dan memiliki tahapan-tahapan menurun (seperti air terjun) yang dilakukan dengan pendekatan sistematik dan sekuensial mulai dari tahapan awal sampai akhir. Masing masing tahapan harus diselesaikan sebelum melangkah ketahapan selanjutnya.

Kelebihan:

1. Mudah digunakan dan dimengerti.
2. Dapat digunakan untuk staff yang belum berpengalaman.
3. Kualitas dari sistem yang dihasilkan akan baik. Ini dikarenakan oleh pelaksanaannya secara bertahap, sehingga tidak terfokus pada tahapan yang lain.
4. Dokumentasi pengembangan sistem sangat terorganisir, karena setiap tahap harus terselesaikan dengan lengkap sebelum melangkah ke tahap berikutnya. Jadi, setiap tahapan akan mempunyai dokumen tertentu.

Kekurangan:

1. Diperlukan majemen yang baik, karena proses pengembangan tidak dapat dilakukan secara berulang sebelum terjadinya suatu produk.
2. Jika terdapat kesalahan kecil akan menjadi masalah besar jika tidak diketahui sejak awal pengembangan.
3. Pelanggan sulit menyatakan kebutuhan secara langsung sehingga tidak dapat mengakomodasi kekurangan pada saat awal pengembangan.
4. Sistem yang diinginkan konsumen tidak dapat dirubah lagi jika tahap komunikasi sudah selesai.

**Pengembangan Metode Waterfall:**

### V-Model

Model ini merupakan perluasan dari model waterfall, karena tahap-tahapnya mirip dengan yang terdapat dalam model waterfall. Jika dalam model waterfall proses dijalankan secara linear, maka dalam model V proses dilakukan bercabang. Dalam model V ini digambarkan hubungan antara tahap pengembangan software dengan tahap pengujiannya.

Kelebihan:

1. Bahasa yang digunakan untuk merepresentasikan konsep V model menggunakan bahasa formal. Contoh : dengan menggunakan objek model ataupun frame-frame.
2. Meminimalisasikan kesalahan pada hasil akhir karena ada test pada setiap prosesnya.
3. Penyesuaian yang cepat pada projek yang baru
4. Memudahkan dalam pembuatan dokumen projek
5. Biaya yang murah dalam perawatan dan modifikasinya
6. V Model bersifat fleksibel.
7. V Model dikembangkan dan dikembangkan oleh banyak orang. User dari V Model berpartisipasi dalam change control board yang memproses semua change request terhadap V Model.

Kekurangan:

1. Aktifitas V-Model hanya difokuskan pada projectnya saja, bukan pada keseluruhan organisasi.
2. Metode yang ditawarkan terbatas. Sehingga kita tidak memiliki cara pandang dari metode yang lain. Kita tidak memiliki kesempatan untuk mempertimbangkan jika ada tools lain yang lebih baik.
3. Tidak ada tools untuk hardware di V-Model. Tool yang dimaksud adalah “software yang mendukung pengembangan atau pemeliharaan / modifikasi dari system IT.
4. V Model adalah model yang project oriented sehingga hanya bisa digunakan sekali dalam suatu proyek.
5. V Model terlalu fleksibel dalam arti ada beberapa activity dalam V Model yang digambarkan terlalu abstrak sehingga tidak bisa diketahui dengan jelas apa yang termasuk dalam activity tersebut dan apa yang tidak.

### Structured System Analysis and Design Method

## 2. Metode Prototyping

Metode ini digunakan saat konsumen mengetahui kebutuhan umum software yang diinginkan akan tetapi tidak mengetahui secara mendetail fungsi dan fitur-fiturnya. Metode ini bisa juga dipakai saat pengembang aplikasi tidak mengetahui secara pasti efisiensi dari suatu algoritma atau tidak tahu rancangan interaksi manusia dan komputer yang akan dipakai.

Kelebihan:

1. Komunikasi terjalin baik antara pengembang dengan konsumen sehingga dapat mengetahui kebutuhan konsumen lebih baik.
2. Konsumen juga berperan aktif dalam pengembangan sistem.
3. Menghemat waktu dalam pengembangannya.
4. Implementasi software atau sistem lebih mudah karena konsumen mengetahui apa yang diharapkan.

Kekurangan:

1. Perancangan dan kualitas sistem kurang baik karena mengedepankan aspek kenyamanan user.
2. Pengembang kadang-kadang menggunakan implementasi tidak efisien.

## 3. Metode Iterative

Merupakan metode pengembangan sistem bersifat dinamis yaitu setiap tahap dapat diulang(iterasi) jika terdapat kekurangan atau kesalahan. Setiap tahapan dapat dikerjakan berupa ringkasan dan tidak lengkap, tapi pada akhir pengembangan akan didapatkan sistem yang lengkap.

Kelebihan:

1. Dapat mengakomodasi jika terjadi perubahan pada tahapan pengembangan yang telah dilaksanakan.
2. Cocok untuk pengembangan sistem dan perangkat lunak skala besar.
3. Pengembang dan pemakai dapat lebih mudah memahami dan bereaksi terhadap resiko setiap tahapan karena system terus bekerja selama proses.

Kekurangan:

1. Hanya berlaku untuk Short-Lifetime system.
2. Tahapan proses tidak terlihat sedang berada ditahapan mana suatu pekerjaan.
3. Memerlukan alat ukur kemajuan secara regular.
4. Perubahan yang sering terjadi dapat merubah struktur system.
5. Memerlukan tenaga ahli dengan kemampuan tinggi.

**Pengembangan Metode Iterative:**

### Unified Software Development Process (USDP)

USDP terbagi atas 4 fase, yaitu Inception, Elaboration, Construction, dan Transition. Di tiap-tiap fase tersebut terdapat 6 tahap kerja (iterasi) yang harus dilakukan, yaitu Business Modeling, Requirements, Analysis & Design, Implementation, Test, dan Deployment. Ada juga referensi lain yang membagi fase tersebut menjadi 5 tahap saja (Business Modeling dan Requirements dijadikan satu) dan ada pula yang membaginya menjadi 7 tahap (fase akhir ditambah dengan Maintenance). Fase kerja ini berkaitan erat dengan peran seorang project manager, sedangkan tahap kerja (iterasi) berkaitan erat dengan peran seorang developer atau programmer.

Kelebihan:

1. USDP memungkinkan para pengembang perangkat lunak untuk bisa mengetahui resiko vital di setiap awal tahapan pengerjaan.
2. Setiap use case merepresentasikan kebutuhan dan hubungan dari tiap-tiap entity yang kemudian akan diimplementasikan dalam sistem.
3. Terdapat batasan-batasan, kontrol, dan kelas entiti dari perangkat lunak yang akan dibuat.

Kekurangan:

1.    Kurang tepat jika digunakan untuk pengembangan software berbasis struktural.
2.    Dinamic Systems Development method

## 4. Metode Incremental

Model incremental adalah model pengembangan sistem pada software engineering berdasarkan requirement software yang dipecah menjadi beberapa fungsi atau bagian sehingga model pengembangannya secara bertahap. dilain pihak ada mengartikan model incremental sebagai  perbaikan dari model waterfall dan sebagai standar pendekatan topdown.

Kelebihan:

1. Merupakan model dengan manajemen yang sederhana.
2. Pengguna tidak perlu menunggu sampai seluruh sistem dikirim untuk mengambil keuntungan dari sistem tersebut. Increment yang pertama sudah memenuhi persyaratan mereka yang paling kritis, sehingga perangkat lunak dapat segera digunakan.
3. Resiko untuk kegagalan proyek secara keseluruhan lebih rendah. Walaupun masalah masih dapat ditemukan pada beberapa increment. Karena layanan dengan prioritas tertinggi diserahkan pertama dan increment berikutnya diintegrasikan dengannya, sangatlah penting bahwa layanan sistem yang paling penting mengalami pengujian yang ketat. Ini berarti bahwa pengguna akan memiliki kemungkinan kecil untuk memenuhi kegagalan perangkat lunak pada increment sistem yang paling bawah.
4. Nilai penggunaan dapat ditentukan pada setiap increment sehingga fungsionalitas sistem disediakan lebih awal.
5. Memiliki risiko lebih rendah terhadap keseluruhan pengembagan sistem.
6. Prioritas tertinggi pada pelayanan sistem adalah yang paling diuji.

Kekurangan:

1. Kemungkinan tiap bagian tidak dapat diintegrasikan
2. Dapat menjadi build and Fix Model, karena kemampuannya untuk selalu mendapat perubahan selama proses rekayasa berlangsung
3. Harus Open Architecture
4. Mungkin terjadi kesulitan untuk memetakan kebutuhan pengguna ke dalam rencana spesifikasi masing-masing hasil increment.

## 5. Metode Spiral

Model ini ditemukan sekitar tahun 1988 oleh Barry Boehm pada artikel A Spiral Model of Software Development and Enhancement. Spiral model adalah salah satu bentuk evolusi yang menggunakan metode iterasi natural yang dimiliki oleh model prototyping dan digabungkan dengan aspek sistimatis yang dikembangkan dengan model waterfall. Spiral model dibagi menjadi beberapa framework aktivitas, yang disebut dengan task regions. Kebanyakan aktivitas tersebut dibagi antara 3 sampai 6 aktivitas. Berikut adalah aktivitas-aktivitas yang dilakukan dalam spiral model:

1. Customer communication.
2. Planning.
3. Analysis risk.
4. Engineering.
5. Construction & Release.
6. Customer evaluation.

Kelebihan:

1. Model ini sangat baik digunakan untuk pengembangan sistem software dengan skala besar.
2. Karena progres perkembangan dari SE dapat dipantau oleh kedua belah pihak baik developer maupun user/customer, sehingga mereka dapat mengerti dengan baik mengenai software ini begitu juga dengan resiko yang mungkin didapat pada setiap aktivitas yang dilakukan.
3. Model ini melakukan tahap-tahap yang baik, didefinisikan dengan model waterfall dan ditambah dengan iterasi yang menyebabkan model ini lebih realistis untuk merefleksikan dunia nyata.

Kekurangan:

1. Dibutuhkan kombinasi kemampuan manajerial dan teknis tersendiri untuk mengontrol model ini sehingga dengan sendirinya dapat meyakinkan user/customer tersebut.
2. Mengenai analisis resiko yang terdapat pada model ini dibutuhkan kemampuan expert tersendiri agar tahap ini dapat berjalan dengan baik
3. Dibutuhkan kemampuan manajemen yang tinggi untuk melakukan perkiraan resiko, karena jika ada resiko yang luput untuk dievaluasi, dikhawatirkan dapat muncul di kemudian hari yang dapat menghambat proses SE.
4. Masih jarang digunakan dan kurang populer.

## 6. Metode Rapid Aplication Development

Rapid application development (RAD) menekankan pada siklus pembangunan pendek, singkat, dan cepat. Waktu yang singkat adalah batasan yang penting untuk model ini. Rapid application development menggunakan metode iteratif (berulang) dalam mengembangkan sistem dimana working model (model bekerja) sistem dikonstruksikan di awal tahap pengembangan dengan tujuan menetapkan kebutuhan (requirement) user dan selanjutnya disingkirkan. Working model digunakan kadang-kadang saja sebagai basis desain dan implementasi sistem final.

Kelebihan:

1. Waktu pengembangan yang lebih singkat.
2. Biaya yang relatif lebih murah.
3. Component based construction ( pemrograman berbasis komponen bukan prosedural).
4. Penekanan pada penggunaan ulang (reuse) komponen perangkat lunak yang telah ada.
5. Pembangkitan kode program otomatis/semi otomatis.
6. Multiple team (banyak tim), tiap tim menyelesaikan satu tugas yang selevel tapi tidak sama. Banyaknya tim tergantung dari area dan kompleksitasnya sistem yang dibangun.

Kekurangan:

1. Model RAD memerlukan sumber daya yang cukup besar, terutama untuk proyek dengan skala besar.
2. Model RAD memerlukan komitmen yang kuat antara pengembang dan pemesssan, bahkan keduanya bisa tergabung dalam 1 tim.
3. Sistem yang tidak bisa dimodularisasi tidak cocok untuk model ini.
4. Penghalusan dan penggabungan dari beberapa tim di akhir proses sangat diperlukan dan ini memerlukan kerja keras.
5. Proyek bisa gagal karena waktu yang disepakati tidak dipenuhi dan resiko teknis yang tinggi juga kurang cocok untuk model ini.

## 7. Metode Agile

Metode Agile adalah proses pengembangan software yang berkembang pada tahun 1990. Kata Agile berarti bersifat cepat, ringan, bebas bergerak, waspada. Metodologi yang dikenal sebagai agile method ini mengutamakan fleksibilitas terhadap perubahan-perubahan yang terjadi selama pengembangan. Model-model dari agile diantaranya Rational Unified Process (1994), Scrum (1995), Crystal Clear, Extreme Programming (1996), dan Adaptive Software Development, Feature Driven Development, and Dynamic Systems Development Method (DSDM) (1995). Dan pada akhirnya terbentuklah pada tahun 2001 proses pengembangan agile.

Kelebihan:

1. Meningkatkan kepuasan kepada klien.
2. Pembangunan system dibuat lebih cepat.
3. Mengurangi resiko kegagalan implementasi software dari segi non-teknis.
4. Jika pada saat pembangunan system terjadi kegagalan,kerugian dar segi materi relative kecil.

Kekurangan:

1. Kurang cocok untuk pengembang software pemula

**Pengembangan Metode Agile:**
* Crystal Clear
* Scrum
* **XP (Xtreme Programming)**

XP dikembangkan oleh Beck, Cunningham, dan Jeffries dan ini merupakan lightweight discipline pengembangan perangkat lunak berdasarkan empat core value, yaitu komunikasi, kesederhanaan, feedback, dan courage.

Kelebihan:

1. Menjalin komunikasi yang baik dengan client.
2. Meningkatkan komunikasi dan sifat saling menghargai antar developer.
3. Cocok untuk kebutuhan sistem selalu berubah-ubah.
4. XP cocok digunakan saat client membutuhkan waktu yang cepat dalam pembuatan sistem.

Kekurangan:

1. Developer harus selalu siap dengan perubahan karena perubahan akan selalu diterima.
2. Tidak bisa membuat kode yang detail di awal (prinsip simplicity dan juga anjuran untuk melakukan apa yang diperlukan hari itu juga).
3. XP tidak memiliki dokumentasi formal yang dibuat selama pengembangan. Satu-satunya dokumentasi adalah dokumentasi awal yang dilakukan oleh user.
