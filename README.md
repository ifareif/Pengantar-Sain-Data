# Analisis-Pendapatan-POS
Analisis pendapatan per tahun (2024-2025) dari data transaksi POS dengan Python dan Jupyter Notebook

**Hasil (pendapatan bersih):**
| Tahun | Pendapatan Bersih |
|---|---|
| 2024 | Rp 127.406.475 |
| 2025 | Rp 135.001.100 |

## Aturan Perhitungan
- Pendapatan = jumlah x harga_satuan x (1 - diskon_persen / 100)
- Hanya transaksi berstatus SELESAI yang dihitung (BATAL dan RETUR tidak)
- Jumlah di luar 1-12 dianggap salah input dan dikeluarkan
- Baris duplikat dihapus, kode_kasir kosong diisi TIDAK_DIKETAHUI
- Hasil dikelompokkan per tahun (2024 dan 2025)

## Cara Menjalankan 
pip install -r requirements.txt

jupyter notebook analisis_pendapatan_pos.ipynb
