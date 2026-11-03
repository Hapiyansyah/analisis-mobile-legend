# Analisis Mobile Legends

Repositori ini berisi proyek analisis sentimen terhadap ulasan pengguna game Mobile Legends di Google Play Store. Proyek ini dilakukan dalam bentuk notebook Python dan fokus pada pemrosesan teks, analisis opini, serta pengelompokan komentar menggunakan teknik NLP dan K-Means.

## Deskripsi Proyek

Tujuan dari proyek ini adalah untuk:
- Mengambil data ulasan pengguna Mobile Legends dari Google Play Store.
- Membersihkan dan memproses teks ulasan.
- Menentukan sentimen tiap ulasan (positif atau negatif).
- Menganalisis pola komentar pengguna terkait game, performa, bug, jaringan, dan pengalaman bermain.
- Mengelompokkan komentar ke dalam cluster tertentu untuk melihat tema utama yang paling sering dibahas.

## Dataset

Dataset yang digunakan dalam proyek ini adalah file berikut:
- `mobile_legends_dataset.csv`

File CSV berisi review pengguna Mobile Legends yang mencakup:
- nama pengguna
- rating / score
- tanggal review
- isi komentar
- versi aplikasi
- informasi lain yang terkait dengan ulasan

## Struktur Repository

- `moba_analog.ipynb`  
  Notebook utama yang berisi seluruh proses:
  - scraping data dari Google Play Store
  - pembuatan DataFrame
  - preprocessing teks
  - label sentimen
  - analisis data
  - pengelompokan (clustering) menggunakan K-Means

- `mobile_legends_dataset.csv`  
  Dataset hasil scraping dan siap digunakan untuk analisis.

- `README.md`  
  Dokumentasi singkat mengenai proyek ini.

## Alur Kerja

Notebook `moba_analog.ipynb` melakukan tahapan berikut:
1. Instalasi library `google-play-scraper`
2. Scraping review Mobile Legends dari Google Play
3. Menyimpan hasil review ke dalam DataFrame
4. Pemilihan kolom yang relevan
5. Preprocessing teks:
   - lowercasing
   - pembersihan karakter khusus
   - normalisasi/penanganan kata tidak baku
6. Labeling sentimen berdasarkan skor review
7. Analisis distribusi sentimen
8. Visualisasi dan interpretasi hasil
9. Pengelompokan tema komentar menggunakan K-Means

## Teknologi yang Digunakan

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Google Play Scraper
- NLP preprocessing
- K-Means Clustering

## Hasil yang Diharapkan

Proyek ini diharapkan mampu:
- Menemukan tren opini pengguna terhadap Mobile Legends
- Mengidentifikasi masalah yang paling sering dikeluhkan pemain
- Menilai apakah pengguna cenderung memberikan feedback positif atau negatif
- Menyediakan gambaran umum mengenai isu utama dalam komunitas pemain Mobile Legends

## Cara Menjalankan

1. Clone repositori ini
2. Buka file `moba_analog.ipynb` di Jupyter Notebook atau Google Colab
3. Jalankan sel-sel notebook secara berurutan
4. Pastikan library Python yang diperlukan sudah terinstal

## Catatan

Proyek ini bersifat analisis data berbasis notebook dan belum dikembangkan menjadi aplikasi web atau backend. Fokus utamanya adalah eksplorasi data dan pemahaman sentimen pengguna terhadap game Mobile Legends.
