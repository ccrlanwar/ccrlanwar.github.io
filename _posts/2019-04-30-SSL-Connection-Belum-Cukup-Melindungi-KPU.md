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

Perhatikan panah hijau pada gambar 0.1

<img src="https://lh3.googleusercontent.com/xUa1lE8Pl27nY8K7CVl0uiY-dE6nF3zr2YjL5Ead2BE7N9vRvE3LNQEez1uzr0E7JShclhn7t-6clPoy8yZNqMO5aa0YZeS7VX2AAJ3UxFbmWoldTKmO1FcFuVYQGSP3LL1y2k2G_wZ68L1zVQdZtLkFq3OEhvIJmT_u-hifMt8xEYl8DUfa-POh1K-fBjVMxp6kQWS_sMWmKJWe5nKUgnfakqq-N_yhqUhOgCKXWgUWoLze_n1ActISSdoJyatQNLUudm5eTN6-tRsF3j-alIcuqqadB7sHYcCsJHHxhO3To9ODPEq0h_L542Zachq0Py8jzbGiJsb2TQTZIog41JeSXl7-ACfJoxTqawu9WKaqoBcQLi43f6UPjLEuKNQUcJG4IB87SBAjRLe-w-iH6oELlh1Q6UQHWKTJyLaH8dMX90bUU07Tgj88KBUCyoAFHvyzX2o0wFmQ_i-uZZGzlDs06up-wE9BUOoz7-fh9DB9xVNkpDx5etifMGWnmCGOZo4x7yRKrrrLIMmxn94_qFLUShTT6rh-k11ZRjgR7ZaKvTVYlifw6rxLwfRvMqXqvhTcl14Ql1aBFar3i2PAx_ym5rVY2cQkWMdGPF2px6axgIWxgOAAmWOKkKS87vVWjJ_LG7OhEsFe-VZmMqUcRHz1sDGl0g=w1113-h515-no" alt="Screenshot KPU"/>

Gambar 0.2

