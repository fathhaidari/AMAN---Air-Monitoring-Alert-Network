# Sistem Pemantauan Jaringan Pipa Distribusi Air PDAM

Proyek kelompok **Ithaca** (Kelas A) untuk mata kuliah Pengembangan Aplikasi Berbasis Web (PABW), Semester Ganjil 2026/2027, Universitas Islam Indonesia.

Aplikasi web untuk memantau debit dan tekanan air pada jaringan pipa distribusi PDAM, menampilkan status tiap titik pipa, dan memberi peringatan otomatis saat terjadi gangguan.

## Proses bisnis

Proses bisnis berasal dari topik yang ditetapkan pada mata kuliah MPTI: pemantauan dan penanganan kebocoran atau penurunan aliran air pada jaringan pipa distribusi PDAM di wilayah Kelurahan Hargobinangun.

Saat ini prosesnya berjalan manual:

1. Petugas melakukan patroli fisik keliling untuk mencari titik kerusakan pipa.
2. Warga melapor setelah pasokan air di rumah mereka mati atau jalanan tergenang.
3. Petugas menuju lokasi, mencari titik kebocoran, lalu memperbaikinya.

Proses yang akan didigitalkan pada versi pertama:

1. Memantau debit dan tekanan air per titik pipa dalam satu layar.
2. Menampilkan status titik pipa (Normal, Waspada, Bahaya).
3. Memberi peringatan otomatis dan menyediakan riwayat debit dan tekanan untuk analisis.

## Masalah

Pendeteksi kebocoran atau penurunan aliran air pada jaringan pipa distribusi berjalan lambat atau tidak terpantau secara terus-menerus.

Akibatnya:

- air bersih banyak terbuang sia-sia,
- biaya kerugian operasional membengkak,
- perbaikan layanan ke rumah warga memakan waktu lama,
- tidak dapat memantau kualitas air secara real-time.

## Pelaku

| Pelaku | Peran terhadap sistem |
| --- | --- |
| Petugas Operasional | Memantau status kondisi titik pipa tanpa berkeliling |
| Petugas Lapangan | Menerima peringatan dini dan mengetahui titik kebocoran secara instan |
| Supervisor PDAM | Menganalisis riwayat debit dan tekanan untuk melihat penurunan performa aliran |
| Admin Sistem | Mengatur batas aman (*threshold*) debit dan tekanan (tahap berikutnya) |
| Warga Kelurahan Hargobinangun | Terdampak tidak langsung; bukan pengguna sistem pada versi pertama |

## Fitur

Wajib (versi pertama):

1. Melihat kartu status kondisi titik pipa (Normal, Waspada, Bahaya).
2. Menerima peringatan dini otomatis saat debit atau tekanan anomali.
3. Melihat grafik riwayat debit dan tekanan air per lokasi.

Tahap berikutnya:

4. Mengirim form laporan gangguan fisik dari petugas lapangan.
5. Mengatur batas aman (*threshold*) debit dan tekanan.

## Di luar cakupan

- Pengecekan kualitas air secara kimiawi (pH, kekeruhan)
- Sambungan ke tagihan meteran pelanggan
- Aplikasi HP (Android/iOS)
- Pemasangan pipa fisik di seluruh wilayah kota

Pada demo expo, data debit dan tekanan berasal dari simulasi.

## Anggota kelompok

| NIM | Nama | Peran |
| --- | --- | --- |
| 25523167 | Muhammad Fath Haidari | Project manager, Front-end developer |
| 25523125 | Bryant Agus Junior Saputra | UI/UX Designer & System Analyst |
| 25523190 | Ahmad Dani Maulana | Web Developer (Back-end), Server & Security Engineer |
| 25523231 | Zerga Naufal Arkaan | Network Engineer |

## Alur kerja Git

- Cabang utama: `main`. Jangan commit langsung ke `main` setelah commit pertama.
- Setiap pekerjaan dikerjakan di cabang sendiri (misalnya `fitur/kartu-status`), lalu digabung lewat pull request yang ditinjau minimal satu anggota lain.
- Pesan commit singkat dan jelas, misalnya `Tambah kartu status titik pipa`.

## Status

Tahap kick-off (P14). Dokumen worksheet, diagram use case, dan wireframe akan dilengkapi sebelum proposal pada P17.
