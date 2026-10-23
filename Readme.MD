# Segmentasi Wilayah Pelanggan E-Commerce Shopee Menggunakan K-Means dan Hierarchical Clustering

Proyek Akhir Praktikum Data Science, Prodi Informatika UPN "Veteran" Yogyakarta.

## Ringkasan Proyek
Proyek ini mengelompokkan kota/kabupaten pembeli pada satu toko Shopee berdasarkan pola pesanan, pembayaran, dan pengiriman. Data pesanan diagregasi per wilayah, lalu dikelompokkan dengan **K-Means** dan **Agglomerative (Hierarchical) Clustering**. Hasilnya dipakai untuk merumuskan strategi ongkir, promo, dan pembayaran yang berbeda untuk tiap segmen wilayah.

Pertanyaan utama:
1. Berapa segmen wilayah yang terbentuk secara alami?
2. Apa ciri tiap segmen?
3. Mana yang lebih baik, K-Means atau Hierarchical?
4. Strategi apa yang cocok untuk tiap segmen?

Metrik: Inertia (Elbow), Silhouette Score, Cophenetic Correlation Coefficient, dan dendrogram.

## Anggota dan Kontribusi
| Nama | NIM | Kontribusi |
|---|---|---|
| `[isi]` | `[isi]` | `[isi, misalnya: Business Understanding, Data Gathering, README]` |
| `[isi]` | `[isi]` | `[isi, misalnya: EDA]` |
| `[isi]` | `[isi]` | `[isi, misalnya: Cleaning, Modelling, Evaluasi]` |

## Sumber Data
- Dataset: `[isi judul dataset di Kaggle]`
- Tautan: `[isi URL]`
- Pembuat: `[isi]`
- Lisensi: `[isi]`
- Tanggal pengambilan: `[isi]`
- Cakupan: pesanan satu toko di Shopee, Desember 2023 sampai November 2025 (20.848 baris, 19 kolom). Tidak memuat identitas pembeli, hanya kota/kabupaten dan provinsi.

## Struktur Repository
```
.
├── README.md
├── notebook_proyek_akhir.ipynb
└── data/
    └── all_months_clean.csv
```

## Panduan Menjalankan
1. Pastikan Python 3.10 atau lebih baru terpasang.
2. Pasang library:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn scipy jupyter
   ```
3. Jalankan Jupyter:
   ```
   jupyter notebook
   ```
4. Buka `proyek_akhir.ipynb` lalu jalankan semua sel dari atas ke bawah (`Run All`). Dataset dibaca dari `data/all_months_clean.csv` dengan pemisah `;`.

## Keterbatasan
Data hanya mewakili satu toko di satu platform, sehingga hasil tidak dapat digeneralisasi ke seluruh pasar e-commerce Indonesia.
