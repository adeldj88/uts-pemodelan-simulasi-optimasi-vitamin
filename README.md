# uts-pemodelan-simulasi-optimasi-vitamin
Program optimasi biaya racikan suplemen vitamin menggunakan program linear untuk UTS Pemodelan dan Simulasi Informatika Universitas Udayana.
# Optimasi Biaya Racikan Suplemen Vitamin

Repositori ini berisi kode program untuk Ujian Tengah Semester
mata kuliah Pemodelan dan Simulasi, Program Studi Informatika,
Fakultas Matematika dan Ilmu Pengetahuan Alam, Universitas Udayana.

## Identitas Kelompok

Kelompok: [Nomor kelompok]

| No. | NIM | Nama |
| --- | --- | --- |
| 1 | [2408561016] | Kanya Kardisa Kanani |
| 2 | [2408561047] | I Gede Surya Tanajaya |
| 3 | [2408561115] | Ni Putu Nadia Earlyvania Paramitha |
| 4 | [2408561118] | Luh Adelia Pratiwi Djelantik |

## Deskripsi Kasus

Laboratorium farmasi ingin meracik suplemen menggunakan
Ekstrak Jeruk dan Ekstrak Wortel dengan biaya minimum.

Setiap gram Ekstrak Jeruk mengandung 3 unit Vitamin C dan
1 unit Vitamin D dengan biaya Rp15.000. Setiap gram Ekstrak
Wortel mengandung 1 unit Vitamin C dan 2 unit Vitamin D
dengan biaya Rp10.000.

Racikan harus memenuhi kebutuhan minimal 15 unit Vitamin C
dan 10 unit Vitamin D.

## Model Matematika

Variabel keputusan:
- x: jumlah Ekstrak Jeruk dalam gram.
- y: jumlah Ekstrak Wortel dalam gram.

Fungsi tujuan:
Minimalkan Z = 15000x + 10000y.

Kendala:
- 3x + y >= 15.
- x + 2y >= 10.
- x >= 0 dan y >= 0.

Jumlah bahan diperbolehkan berupa pecahan gram.

## Isi Repositori

- `Optimasi_Biaya_Suplemen_Vitamin.ipynb`: notebook yang
  berisi kode optimasi, pemeriksaan kendala, dan grafik.
- `README.md`: penjelasan proyek dan cara menjalankannya.

## Pustaka yang Digunakan

- SciPy: menyelesaikan optimasi menggunakan `linprog`.
- NumPy: menyiapkan data untuk grafik.
- Matplotlib: menggambar garis kendala, daerah layak,
  dan titik optimal.

## Cara Menjalankan

1. Unduh notebook dari repositori ini.
2. Buka Google Colab dan unggah notebook tersebut.
3. Jalankan seluruh sel secara berurutan, mulai dari
   kode optimasi kemudian kode grafik.
4. Periksa hasil optimasi dan grafik yang ditampilkan.

Jika pustaka belum tersedia, jalankan pada sel terpisah:

!pip install scipy numpy matplotlib

## Ringkasan Hasil

Solusi optimal berdasarkan model:
- Ekstrak Jeruk: 4 gram.
- Ekstrak Wortel: 3 gram.
- Biaya minimum: Rp90.000.
- Vitamin C yang dihasilkan: 15 unit.
- Vitamin D yang dihasilkan: 10 unit.

Kombinasi tersebut memenuhi seluruh kendala dan sesuai
dengan hasil perhitungan manual.

## Batasan Model

Model mengasumsikan harga dan kandungan vitamin per gram
tetap, bahan tersedia mencukupi, serta tidak terjadi
kehilangan vitamin selama pencampuran. Biaya tambahan
di luar biaya bahan baku tidak diperhitungkan.
