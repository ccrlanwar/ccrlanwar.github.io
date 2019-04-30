---
layout: post
section-type: post
title: SSL Connection belum cukup melindungi KPU
category: IT
tags: [ 'tech' ]
---

Selepas pemilihan umum yang diselenggarakan pada 17 April 2019, KPU mulai berjuang menginput data <a href="https://pemilu2019.kpu.go.id/#/ppwp/hitung-suara/" target="\_blank">di situs resminya</a> sesuai salinan form C1 di setiap TPS di seluruh Indonesia.

Tentu selama proses input data suara rakyat terdapat <a href="https://nasional.tempo.co/read/1197483/kesalahan-input-data-kpu-murni-human-error/full&view=ok" target="\_blank">kesalahan-kesalahan karena, menurut pengakuan Arif Budiman selaku ketua, murni faktor human error belaka</a>.

Di samping kesalahan yang telah diklarifikasi tersebut, tentu patut pula kita perhatikan dari segi perlindungan teknis menyangkut situng KPU. Di mana banyak sekali ditemukan <a href="https://www.cnnindonesia.com/teknologi/20190424231311-185-389417/kpu-sebut-situsnya-diretas-ratusan-hacker-setiap-hari" target="\_blank">serangan pihak ke tiga di situsnya</a>. Beruntung dari segi front-end KPU telah dilindungi <a href="http://info.ssl.com/article.aspx?id=10241" target="\_blank">SSL connection</a> (sertifikat koneksi yang terenkripsi).

Akan tetapi SSL yang memiliki simbol gembok hijau di address bar Situng KPU belum cukup melindungi manipulasi jumlah suara melalui inspect element di browser. Hal ini tentu sangat merugikan pihak KPU sendiri karena pihak lain mampu mengedit (menambah dan, atau mengurangi) jumlah suara masing-masing paslon capres dan cawapres.

SS 0.1
<img src="https://i.imgur.com/oLNBrSL.jpg" />

Kalau kita perhatikan gambar SS 0.1 di atas terdapat penampang logo KPU yang telah berubah (lih: tanda panah hijau). Alih-alih berupa logo resmi, penampang SS 0.1 menyajikan manipulasi logo serta icon tab tengkorak. Penampang pada SS 0.1 di atas patut kita pertanyakan keasliannya karena SSL tidak menyertakan indikator sambungan keamanan situs yang ditunjukkan dengan <a href="https://blog.mozilla.org/security/2015/11/03/updated-firefox-security-indicators-2/" target="\_blank"> indikoator ikon warning di address bar browser Firefox</a>. Artinya perubahan logo dan ikon bukan berasal dari front-end KPU, tetapi dari pihak ke tiga yang berusaha memanipulasi melalui browser di komputer.

SS 0.2
<img src="https://i.imgur.com/HQLAEMa.jpg" />

Gambar SS 0.2 di atas merupakan penampang laman Situng KPU tanpa manipulasi.

SS 0.3
<img src="https://i.imgur.com/DH11H0R.jpg" />

Kasus gambar SS 0.3 tetap menunjukkan indikator address bar Situng KPU aman dengan proses manipulasi (pengurangan) jumlah suara regional (Aceh) untuk masing-masing paslon capres dan cawapres (lih: tanda panah hijau).

Kesimpulan:

Tentu dengan adanya sertifikat keamanan sambungan SSL (HTTPS) di address bar dapat membantu masyarakat dalam membedakan informasi resmi dan tidak. Gambar SS 0.1 menunjukkan informasi yang tidak resmi dengan indikator sambungan yang tidak aman jika dibandingkan dengan penampang laman Situng KPU resmi yang ditunjukkan gambar SS 0.2. Perbedaan antara informasi murni dan hasil manipulasi dapat diperhatikan melalui perbedaan setiap indikator keamanan sambungan SSL (ikon gembok).

Saran:

Kasus gambar SS 0.3 mengingatkan kita akan pentingnya keamanan jumlah suara secara menyeluruh, dan terintegrasi langsung dengan sertifikat SSL di address bar. Segala bentuk manipulasi jumlah suara paslon capres dan cawaapres dapat dipastikan kebenarannya melalui indikator sambungan yang aman dan tidaknya, sehingga masyarakat awam dapat mengetahui informasi yang benar.
