# Ringkasan Tugas 7 – Visualisasi Data dengan Matplotlib

## Gambaran umum
Tugas ini menganalisis data transaksi Point of Sale (POS) tahun 2025 menggunakan Python, Pandas, NumPy, dan Matplotlib. Hasil akhirnya berupa satu gambar yang memuat empat grafik dalam susunan 2 baris × 2 kolom.

Dataset yang digunakan adalah `paket_a_transaksi_pos_2024_2025.csv` yang berada di folder utama repository.

## Tahapan pengolahan data
1. Membaca dataset sebagai teks agar format tanggal dan harga yang beragam tidak salah ditafsirkan.
2. Menghapus data duplikat: dari 5.030 baris menjadi 5.000 baris.
3. Membersihkan format harga dan tanggal, mengubah jumlah serta diskon menjadi angka.
4. Mengubah jumlah negatif menjadi nilai positif, mengisi kode kasir kosong dengan `K_UNKNOWN`, dan menghapus 12 baris dengan jumlah di atas 12.
5. Menghitung nilai penjualan bersih dengan rumus:

   `Total_Bersih = harga_satuan × jumlah × (1 − diskon_persen/100) × 1,11`

   Rumus tersebut menerapkan diskon sebelum PPN 11%.
6. Memilih transaksi tahun 2025. Dari 2.502 transaksi tahun tersebut, 2.365 berstatus `SELESAI`.

## Empat visualisasi dan hasil utama

| No. | Visualisasi | Jenis grafik | Ringkasan temuan |
|---|---|---|---|
| 1 | Penjualan bersih per bulan | Grafik garis | Penjualan tertinggi terjadi pada Maret sebesar sekitar Rp16,2 juta. Penjualan terendah terjadi pada April sebesar sekitar Rp10,9 juta. Desember juga menunjukkan kenaikan dengan sekitar Rp15,5 juta. |
| 2 | 10 produk terlaris | Batang horizontal | Produk RMT1408 menjadi produk terlaris berdasarkan unit terjual sekaligus memiliki omzet tertinggi dalam hasil analisis. |
| 3 | Status transaksi | Diagram pie | Sebanyak 94,5% transaksi berstatus SELESAI, sedangkan 5,5% merupakan gabungan BATAL dan RETUR. Pembatalan lebih sering terjadi daripada retur. |
| 4 | Jumlah pembelian dan diskon | Scatter plot dan garis rata-rata | Hubungan jumlah beli dengan diskon sangat lemah/tidak tampak berarti. Korelasi Pearson (r) dan Spearman (rho) masing-masing sekitar -0,013. |

## Kesimpulan
Visualisasi membantu melihat pola penjualan bulanan, produk yang paling banyak dibeli, komposisi status transaksi, serta hubungan diskon dengan jumlah pembelian. Berdasarkan hasil analisis, Maret merupakan bulan dengan penjualan tertinggi, RMT1408 menjadi produk terlaris, sebagian besar transaksi berhasil diselesaikan, dan besarnya diskon tidak menunjukkan hubungan yang berarti dengan jumlah unit yang dibeli.

## Catatan perhitungan
Total penjualan bersih pada tugas ini adalah **Rp151.478.786**. Nilainya berbeda dari tugas Analisis Pendapatan karena analisis ini menambahkan PPN 11%, mengubah jumlah negatif menjadi positif, serta membatasi perhitungan pada transaksi tahun 2025.

## File
- Notebook: [Tugas7_visualisasi_matplotlib_pos.ipynb](./Tugas7_visualisasi_matplotlib_pos.ipynb)
- Dataset: [paket_a_transaksi_pos_2024_2025.csv](../paket_a_transaksi_pos_2024_2025.csv)
- Gambar hasil akan tersimpan otomatis di folder `hasil/` setelah seluruh sel notebook dijalankan.
