# Pengantar Sains Data

Repository ini berisi kumpulan tugas mata kuliah **Pengantar Sains Data**. Pengerjaan menggunakan Python, Pandas, Matplotlib, dan Jupyter Notebook dengan dataset transaksi Point of Sale (POS) periode 2024–2025.

## Struktur Repository

```text
Pengantar-Sain-Data/
├── Tugas 5/
│   ├── Analisis_Pendapatan_POS.ipynb
│   ├── grafik_pendapatan_per_tahun.png
│   ├── hasil_pendapatan_per_tahun.csv
│   └── README.md
├── Tugas 6/
│   ├── Tugas Manipulasi_Data_Pandas_pos.ipynb
│   └── README.md
├── Tugas 7/
│   ├── Tugas7_visualisasi_matplotlib_pos.ipynb
│   ├── Hasil Ringkasan Penjualan POS Tahun 2025.png
│   └── README.md
├── paket_a_transaksi_pos_2024_2025.csv
├── requirements.txt
└── README.md
```

## Daftar Tugas

### Tugas 5 — Analisis Pendapatan POS
Analisis pendapatan transaksi POS tahun 2024–2025. Tahapan meliputi pemeriksaan dan pembersihan data, perhitungan pendapatan, pengelompokan berdasarkan tahun, serta penyajian hasil dalam grafik dan CSV.

[ Buka folder Tugas 5 ](./Tugas%205/)

### Tugas 6 — Manipulasi Data dengan Pandas
Praktik manipulasi dataset transaksi POS melalui indexing dan selection, operasi aritmatika, filtering, sorting, serta grouping dan agregasi.

[ Buka folder Tugas 6 ](./Tugas%206/)

### Tugas 7 — Visualisasi Data dengan Matplotlib
Analisis dan visualisasi transaksi POS tahun 2025 menggunakan grafik garis, grafik batang, diagram pie, dan scatter plot. Folder ini juga memuat gambar hasil ringkasan penjualan.

[ Buka folder Tugas 7 ](./Tugas%207/)

## Dataset

Dataset utama yang digunakan oleh notebook adalah `paket_a_transaksi_pos_2024_2025.csv`. Simpan file ini di direktori utama repository agar path relatif pada notebook dapat menemukannya.

## Instalasi dan Menjalankan

1. Pastikan Python 3 sudah terpasang.
2. Clone atau unduh repository ini.
3. Buka terminal pada direktori utama repository.
4. Instal seluruh dependensi:

   ```bash
   pip install -r requirements.txt
   ```

5. Jalankan Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Buka notebook pada folder tugas yang ingin dikerjakan, lalu jalankan sel secara berurutan.

## Dependensi

Daftar library yang digunakan tersedia di [requirements.txt](./requirements.txt).
