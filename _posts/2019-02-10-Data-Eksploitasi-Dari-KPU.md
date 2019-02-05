---
layout: post
section-type: post
title: Data Eksploitasi Dari KPU
category: IT
tags: [ 'tech' ]
---

KPU, dengan segala fungsi dan otoritasnya, diam-diam menggunakan kewenangannya tanpa mengindahkan privasi data masyarakat Indonesia. Pasalnya, KPU telah merilis daftar <a href="https://www.cnnindonesia.com/nasional/20181215171713-32-353929/kpu-jumlah-pemilih-tetap-pemilu-2019-capai-192-juta" target="\_blank">192 juta hak pemilih 21019</a> di situsnya, yang memungkinkan dapat diakses langsung secara global.

Data yang saya maksud berupa digit NIK yang telah terenkripsi sebagian, lokasi atau tempat tinggal pemilik, dan siapa saja anggota keluarganya. 

Ya, Anda hanya perlu memeriksa NIK di <a href="https://lindungihakpilihmu.kpu.go.id/" target="\_blank">kolom pencarian daftar pemilih tetap pemilu 2019</a>, maka algoritma sistem akan mendampingi Anda menuju daftar lengkap berapa banyak anggota keluarga yang tercantum di KK dan telah memiliki KTP secara alfabetis. Bukan hanya itu, lokasi dan pemetaan nomor tempat pemungutan suara (TPS) menjadi peran sentral demi mengetahui lokasi di mana Anda tinggal. Paling tidak, jika Anda tak hidup sendirian, saya bisa langsung bertanya pada orang sekitar, di mana rumah Anda tepatnya. Bam!

Bayangkan jika orang yang tak Anda kehendaki mengetahui lokasi rumah, daftar berapa banyak dan siapa saja anggota keluarga yang Anda sayangi. Bukankah cukup riskan dan berbahaya? 

Mengingat kultur <a href="https://www.cissrec.org/publications/detail/7/SIARAN-PERS-Pengamanan-IT-KPU-Perlu-Banyak-Perbaikan.html" target="\_blank">privasi di Indonesia masih sangat ketat minimalis</a>, memungkinkan bagi sebagian orang menyepelekannya. Lagi pula siapa gerangan yang akan menyelidikinya sampai sejauh itu? Suatu pertanyaan yang tak sepatutnya.

Sebagai penggiat privasi keamanan internet, saya cukup merasa bertanggung jawab menutupi hak privasi sebagian penduduk Indonesia yang memiliki keresahan serupa melalui tulisan ini.

Mungkin Anda akan sedikit memihak KPU dengan berdalih:

“Siapa pula yang telah menghafal tujuh belas digit angka NIK saya? Pula tak seluruh nomor tersebut tercantum. Hanya yang kurang kerjaan saja sampai sejauh itu!”

Jika Anda sampai pada statement ini dan sepakat, sepertinya pepatah "ignoran iblis" (baca: <i>ignorance is bliss</i>) menjadi teman keseharian Anda. Saya sarankan jangan membaca bagian selanjutnya. Cukup cuci kaki, matikan lampu, dan tidur.

Mengetahui bahwa nomor NIK yang tersusun di KTP bukan secara acak begitu saja (<i>random and gambling</i>) mejadi bagian penting selanjutnya. Rangkaian nomor ini tersusun dari kode digit kota, kabupaten, kecamatan, tanggal lahir, dan angka susunan data komputasi. Di situsnya, KPU hanya mengenkripsi angka bulan dan tahun lahir, serta angka susunan komputasi di bagian akhir. Itu artinya baru separuh jalan saya dapat melihat kode wilayah tempat Anda tinggal. Karena enam angka pertama menunjukkan nama kota sampai tingkat wilayah kecamatan dan desa. Tetapi saya tak perlu repot-repot lagi memeriksa dompet dan KTP Anda, atau melakukan serangkaian serangan pembocoran (<i>server dumping</i>) dari KPU atau Dukcapil secara ilegal. Karena hakikatnya KPU sendiri yang telah memberikan datanya. Sebuah mekanisme manipulasi rangkai data acak dan terbuka. 

Selanjutnya meninggalkan bekas pertanyaan antara merasa bersalah atau yang bermasalah?

Sebagai contoh, A memiliki kenalan seorang pegawai (B). Dalam hal ini, umpamanya si-B calon pacar atau gebetannya. Karena tak ingin kasus berbeda keyakinan (baca: yang satu yakin bakal jadian, dan yang satunya tidak) terjadi, maka secara naluri artifisial yang maksimalis, A akan mencari tahu sepenuhnya sosok B yang menjadi targetnya. Berbekal pedoman bahwa tercemplung pada nestapa kisah cinta betepuk sebelah tangan adalah suatu kebodohan dan sebisa mungkin harus dihindari.

Selanjutnya, dengan bekal informasi perkenalan pertama kali, ia dapat mengetahui tepat kapan hari ulang tahunnya. Pada detik ini A sudah menyibak sebagian data enkripsi di KPU. Karena angka kelahiran merupakan atribut selanjutnya setelah kode wilayah. Kalau tak percaya, perhatikan dengan saksama NIK masing-masing.

Selanjutnya ia hanya butuh sedikit upaya dan kesabaran demi mengetahui rangkaian digit kode wilayah dan sistem komputasi terakhir di NIK. Bam! A dapat merekayasa pertemuan selanjutnya di TPS sambil mungkin berpura-pura gila.

PS: 
Demi menghindari penyalahgunaan wewenang, segala bukti dan interuksi terpaksa disembunyikan. Jika Anda merupakan teknisi IT di KPU atau yang terlibat, tanpa segan silakan hubungi saya lewat email untuk diskusi lebih lanjut.

