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
| Joeseca Daniel | 123240007 | `[isi, misalnya: Business Understanding, Data Gathering, README]` |
| M. Afiq Fathurrahman | 123240010 | `[isi, misalnya: EDA]` |
| Ahmadshyah Anshori | 123240020 | `[isi, misalnya: Cleaning, Modelling, Evaluasi]` |
| M. Rofik Mua'dz F. | 123240038 | `[isi, misalnya: Cleaning, Modelling, Evaluasi]` |

## Sumber Data
- Sumber: Kaggle, "Indonesia E-Commerce Sales and Shipping 2023-2025"
- Tautan: https://www.kaggle.com/datasets/bakitacos/indonesia-e-commerce-sales-and-shipping-20232025
- Pembuat: BakiTacos
- Lisensi: CC BY-SA 4.0
- Tanggal pengambilan: 10-13-2026
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
4. Buka `notebook_proyek_akhir.ipynb` lalu jalankan semua sel dari atas ke bawah (`Run All`). Dataset dibaca dari `data/all_months_clean.csv` dengan pemisah `;`.

## Keterbatasan
Data berasal dari satu sumber dataset di Kaggle yang tidak menyebut nama platform maupun toko. Berdasarkan ciri datanya (ShopeePay, SPayLater, SeaBank, kurir SPX), data ini teridentifikasi berasal dari Shopee, dan kemungkinan berasal dari satu penjual, tetapi hal itu tidak dapat dikonfirmasi karena tidak ada kolom identitas toko. Hasil analisis karenanya tidak dapat digeneralisasi ke seluruh pasar e-commerce Indonesia.
