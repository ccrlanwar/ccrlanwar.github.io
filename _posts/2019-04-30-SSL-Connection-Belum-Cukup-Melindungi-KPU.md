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

Akan tetapi SSL yang memiliki simbol gembok hijau di browser pada situng KPU belum cukup melindungi manipulasi front-end jumlah suara melalui inspect element di browser. Hal ini tentu sangat merugikan pihak KPU sendiri karena pihak lain mampu mengedit (mark up and down) jumlah suara masing-masing calon presiden.

| gambar 1      | gambar 2      |
|------------|-------------|
| <img src="https://media.wired.com/photos/5926db217034dc5f91becd6b/master/w_582,c_limit/so-logo-s.jpg" width="250"> | <img src="https://mk0jobadderjftub56m0.kinstacdn.com/wp-content/uploads/stackoverflow.com-300.jpg" width="250"> | 
