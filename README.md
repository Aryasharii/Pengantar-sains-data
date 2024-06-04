# DAFTAR ISI
- [DAFTAR ISI](#daftar-isi)
- [PENDAHULUAN](#pendahuluan)
  - [Latar Belakang](#latar-belakang)
  - [Tujuan](#tujuan)
  - [Manfaat](#manfaat)
- [METODE](#metode)
  - [Analisis Sentimen](#analisis-sentimen)
  - [Naïve Bayes](#naïve-bayes)
  - [K-Means](#k-means)
- [HASIL DAN PEMBAHASAN](#hasil-dan-pembahasan)
  - [Teknik Pengambilan Data](#teknik-pengambilan-data)
  - [Teknik Pembersihan Data](#teknik-pembersihan-data)
  - [Preprocessing](#preprocessing)
  - [Analisis](#analisis)
- [KESIMPULAN DAN SARAN](#kesimpulan-dan-saran)
  - [Kesimpulan](#kesimpulan)
  - [Saran](#saran)
- [DAFTAR PUSTAKA](#daftar-pustaka)

---

# PENDAHULUAN

## Latar Belakang
Pemindahan Ibu Kota Negara (IKN) dari Jakarta ke Kalimantan Timur merupakan salah satu kebijakan pemerintah Indonesia yang kontroversial. Kebijakan ini menimbulkan berbagai opini masyarakat di media sosial, khususnya Twitter, yang didominasi oleh sentimen negatif. Penelitian ini bertujuan untuk menganalisis sentimen pengguna Twitter terhadap IKN setelah debat calon wakil presiden pada 22 Desember 2023.

## Tujuan
Penelitian ini bertujuan untuk:
- Mengetahui sentimen pengguna Twitter terhadap IKN setelah debat calon wakil presiden.
- Mengidentifikasi faktor-faktor yang mempengaruhi sentimen tersebut.

## Manfaat
Penelitian ini bermanfaat untuk:
- Memberikan gambaran mengenai pandangan masyarakat terhadap IKN.
- Memberikan informasi kepada pemerintah mengenai sentimen masyarakat.
- Menjadi referensi bagi penelitian selanjutnya mengenai sentimen masyarakat terhadap IKN.

---

# METODE

## Analisis Sentimen
Analisis sentimen digunakan untuk mengelompokkan opini publik menjadi positif, negatif, dan netral. Tujuannya adalah untuk mengetahui opini publik yang dapat dihasilkan rekomendasi untuk perubahan atau perbaikan (Majid et al., 2023).

## Naïve Bayes
Naïve Bayes adalah algoritma klasifikasi probabilistik berdasarkan teori probabilitas Bayes, digunakan untuk analisis sentimen karena kemampuannya menghitung cepat dengan tingkat akurasi yang baik (Affandi & Sugiharti, 2023).

## K-Means
K-Means adalah algoritma unsupervised learning yang digunakan untuk mengelompokkan data tidak berlabel ke dalam kluster berdasarkan kesamaan karakteristik (Nainggolan et al., 2022).

---

# HASIL DAN PEMBAHASAN

## Teknik Pengambilan Data
Data dikumpulkan dari 22 Desember 2023 hingga 21 Januari 2024 melalui web scraping dengan kata kunci "IKN" dan hashtag "#IKN", menghasilkan 1059 tweet unik untuk analisis.

## Teknik Pembersihan Data
Teknik pembersihan data meliputi penghapusan mention, hashtag, indikator retweet, URL, karakter spesial, simbol, spasi berlebih, tanda kurung, dan tanda baca. Data yang bersih diubah menjadi huruf kecil untuk konsistensi.

## Preprocessing
Preprocessing meliputi normalisasi, penghapusan stopwords, tokenisasi, dan stemming. Data hasil preprocessing disimpan dalam format CSV untuk analisis lebih lanjut.

# Analisis Sentimen Proyek IKN

Laporan ini bertujuan untuk menganalisis sentimen masyarakat terhadap proyek Ibu Kota Negara (IKN) Nusantara berdasarkan data dari media sosial Twitter.

## Pengantar

Proyek IKN Nusantara merupakan inisiatif pemerintah Indonesia untuk memindahkan ibu kota negara dari Jakarta ke Kalimantan Timur. Proyek ini telah memicu berbagai tanggapan dan diskusi di media sosial. Laporan ini menggunakan analisis sentimen untuk memahami bagaimana masyarakat merespons proyek ini.

## Metodologi

Data diambil dari Twitter menggunakan kata kunci terkait IKN. Kami menggunakan dua metode utama untuk analisis sentimen: TextBlob dan Naive Bayes. Hasil analisis dipresentasikan dalam bentuk wordcloud dan distribusi sentimen.

## Analisis

### Wordcloud Keseluruhan
![Gambar 3.1 Cloudword](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/cloudword.png)

Wordcloud keseluruhan menunjukkan kata-kata yang paling sering muncul dalam percakapan tentang IKN. Kata-kata seperti "ikn", "bangun", "nusantara", "jadi", dan "lanjut" mendominasi pembicaraan.

### Wordcloud Berdasarkan Sentimen

#### Sentimen Positif
![Gambar 3.2 Cloudword klasifikasi positif](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/positive_cloudword.png)

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen positif.

#### Sentimen Negatif
![Gambar 3.3 Cloudword klasifikasi negatif](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/negative_cloudword.png)

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen negatif.

#### Sentimen Netral
![Gambar 3.4 Cloudword klasifikasi netral](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/neutral_cloudword.png)

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen netral.

### Distribusi Sentimen

#### TextBlob
![Gambar 3.5 Distribusi sentimen IKN (TextBlob)](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/distribusi_sentimen_textblob.png)

Distribusi sentimen berdasarkan TextBlob menunjukkan bahwa sentimen masyarakat lebih condong ke arah positif dengan 523 tweet positif, 398 tweet netral, dan 138 tweet negatif.

#### Naive Bayes
![Gambar 3.6 Distribusi sentimen IKN (Naive Bayes)](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/distribusi_sentimen_naivebayes.png)

Distribusi sentimen berdasarkan Naive Bayes menunjukkan bahwa sentimen masyarakat lebih condong ke arah netral dengan 551 tweet netral, 453 tweet positif, dan 55 tweet negatif.

### Wordcloud Berdasarkan Naive Bayes

#### Sentimen Positif
![Gambar 3.7 Cloudword klasifikasi bayes positif](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/positive_cloudword_naivebayes.png)

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen positif berdasarkan Naive Bayes.

#### Sentimen Negatif
![Gambar 3.8 Cloudword klasifikasi bayes negatif]([path/to/image](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/negative_cloudword_naivebayes.png))

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen negatif berdasarkan Naive Bayes.

#### Sentimen Netral
![Gambar 3.9 Cloudword klasifikasi bayes netral](https://github.com/Aryasharii/Pengantar-sains-data/blob/UAS/image/neutral_cloudword_naivebayes.png)

Wordcloud ini menunjukkan kata-kata yang sering muncul dalam tweet dengan sentimen netral berdasarkan Naive Bayes.

---

# KESIMPULAN DAN SARAN

## Kesimpulan
Penelitian menunjukkan bahwa sentimen masyarakat terhadap IKN setelah debat calon wakil presiden bervariasi dengan dominasi sentimen positif atau netral, tergantung metode analisis yang digunakan.

## Saran
Penelitian lebih lanjut disarankan untuk memperbaiki akurasi analisis sentimen dan mempertimbangkan metode lain untuk validasi hasil.

---

# DAFTAR PUSTAKA
Referensi yang digunakan dalam penelitian ini mencakup studi-studi terbaru mengenai analisis sentimen, algoritma Naive Bayes, dan metode K-Means, seperti yang dicantumkan di bagian referensi.
