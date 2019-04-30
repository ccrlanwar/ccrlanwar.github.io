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
<img src="https://lh3.googleusercontent.com/xUa1lE8Pl27nY8K7CVl0uiY-dE6nF3zr2YjL5Ead2BE7N9vRvE3LNQEez1uzr0E7JShclhn7t-6clPoy8yZNqMO5aa0YZeS7VX2AAJ3UxFbmWoldTKmO1FcFuVYQGSP3LL1y2k2G_wZ68L1zVQdZtLkFq3OEhvIJmT_u-hifMt8xEYl8DUfa-POh1K-fBjVMxp6kQWS_sMWmKJWe5nKUgnfakqq-N_yhqUhOgCKXWgUWoLze_n1ActISSdoJyatQNLUudm5eTN6-tRsF3j-alIcuqqadB7sHYcCsJHHxhO3To9ODPEq0h_L542Zachq0Py8jzbGiJsb2TQTZIog41JeSXl7-ACfJoxTqawu9WKaqoBcQLi43f6UPjLEuKNQUcJG4IB87SBAjRLe-w-iH6oELlh1Q6UQHWKTJyLaH8dMX90bUU07Tgj88KBUCyoAFHvyzX2o0wFmQ_i-uZZGzlDs06up-wE9BUOoz7-fh9DB9xVNkpDx5etifMGWnmCGOZo4x7yRKrrrLIMmxn94_qFLUShTT6rh-k11ZRjgR7ZaKvTVYlifw6rxLwfRvMqXqvhTcl14Ql1aBFar3i2PAx_ym5rVY2cQkWMdGPF2px6axgIWxgOAAmWOKkKS87vVWjJ_LG7OhEsFe-VZmMqUcRHz1sDGl0g=w1113-h515-no" alt="My cool logo"/>

Perbandingan 0.2

| Sebelum      | Sesudah     |
|------------|-------------|
| <img src="https://lh3.googleusercontent.com/twpc-NeK8RjoPUK7evwN4JnkF3M3-vXN-cDETdWe1wsC-jk2qaC673S45iF8CeFAc41hF4qkODnocEItmrmM2K00TOM-PiRnz6-To7mKW0X6X9IAKaZ3asJBgc3qbccTtvvGZArk9kWukfHjkWlVprrvaRwVFMpjmnpBM0--5ilDTMYvLTeXRtFqiftynHTQfOuPKu9OY8IYZICn_uZB4VodWxr8DCOFoBRxeCXTgM_WgFVqtc0z5YkS7r63CbcOmkaEnM3z6F0JiOq4iywmv2ueuMcDwwVXIfZionjvZecWpz2AakTfNRqt146HrFK7vN_3dkEdML0xP8rAovfvXs-7T0G4kw-tuWnYszPZ3QAZtStRmZTCtBCzDhfy5-Trw3TG_7zC_mC94jRgwxJcYdCUXKCSZ-MnaD-n-NTFCb8-U-gwcUNB4_WInFnl73F6g8NJrfUQmzMcEh_Fa88GHqvha2EJK54ln5RHdCDd5O73_jV0AZVnWgk8Zce9Vr5E_00ClB7_8KmMZmsU9QoFYi07LAxWQ_-F1t9xpMpwcZuSmzSOsp_oWso6UDEzaYY2jotdxb0pVhILy8ykWe_knMPiIC4ZeZQyhINhX53V98POgEvdL4FEQIUjWGTduisr0GEwERn-y7G1oEr2J9QmOFEAHcG2bA=w672-h538-no" width="400"> | <img src="https://lh3.googleusercontent.com/lrhJn5f7yIcWdiQmWVo-4vIq_QZR-TFIbLH5nrESrAkDb32BTiRyjcn0EQ8gSCFm3uuQBYBRQ2y8qkC8-5jS3qnStyonSoLNp-0zMmMfPeulQSvfwXkl2PfvScoAN4RFChfDt1Y6VobxNox2fvTuJA213PPUtsQ_W-BN7WzxjeEQCDAiPM_t1tvGmlGqeIKjHQ-xACwBZJAzgB4q1CqmFaXquEQlE1hDIYk6zcO-lsbM5R0werQJgWyqDPHlfpPNULy-ZtYycEdYVPAcmh4Zvq3GJy2Vc0Zh0KxVGZ_4wRponuSOTVGppV3IUx0tlxtsUHn0uwvuBJvS8yZUKBJcnXaQGe-uVKyV2d07EoTFwr99R3xc-fg17Y--WNn4t--oclmQC9j34X_BfLlF-uu9UaCUScYOpYCmX65bGewzffsSFJQYi9ogMyJVTjVRbMQzjEMxGxD3pHH6fsw931QsfdBpssvL-2QG-eBmRqQZjZVll-fJmkfk7F8_r0_WzNYKu6ifnQSMB_RkYX0Iock4n-lAGC3Vjs5MSL7zSIhMnkrtlrGijS4Yo2zpy0HhA7Es2tEKoRtbujbYvPPJHtS4J7AgA75uajUi-QF24hPxUD653BYzCZIcvFjvyVTkDwFWy9m9nHb5nuhtP5kOUyJR31iNa4YQKQ=w671-h540-no" width="400"> | 
