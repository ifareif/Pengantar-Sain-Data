# Tugas 5 — Analisis Pendapatan POS

Folder ini berisi pengerjaan analisis pendapatan transaksi POS untuk tahun 2024 dan 2025.

## Isi Folder

- `Analisis_Pendapatan_POS.ipynb` — notebook untuk membaca, memeriksa, membersihkan, dan menganalisis data transaksi.
- `grafik_pendapatan_per_tahun.png` — visualisasi pendapatan bersih per tahun.
- `hasil_pendapatan_per_tahun.csv` — ringkasan hasil pendapatan per tahun.

## Ringkasan Hasil

| Tahun | Pendapatan Bersih |
|---|---:|
| 2024 | Rp 127.406.475 |
| 2025 | Rp 135.001.100 |

## Tahapan Analisis

1. Membaca dataset transaksi POS.
2. Memeriksa missing value dan data duplikat.
3. Membersihkan format tanggal dan harga.
4. Menangani data yang tidak valid.
5. Menghitung pendapatan kotor dan bersih setelah diskon.
6. Mengelompokkan pendapatan berdasarkan tahun.
7. Membuat grafik dan menyimpan hasil ke CSV.

## Menjalankan Notebook

Dari direktori utama repository, jalankan:

```bash
pip install -r requirements.txt
jupyter notebook
```

Kemudian buka `Tugas 5/Analisis_Pendapatan_POS.ipynb`. Pastikan file dataset `paket_a_transaksi_pos_2024_2025.csv` tetap berada di direktori utama repository.
