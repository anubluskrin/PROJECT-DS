# Ketentuan Proyek Akhir Praktikum Data Science

Prodi Informatika, UPN "Veteran" Yogyakarta

Dokumen ini merangkum ketentuan Proyek Akhir Praktikum Data Science, yaitu ketentuan dataset, pemilihan model, isi notebook, isi repository, dan bobot penilaian.

## Tanggal Penting

| Keterangan | Tanggal |
|---|---|
| Batas pengumpulan repository, termasuk pemilihan metode | 30 Oktober 2026 |

---

## 1. Dataset

Beberapa hal yang harus dicek sebelum memilih dataset:

1. Dataset boleh dari sumber mana saja, **selain yang digunakan di praktikum**.
2. Dataset minimal terdiri dari **100 baris** dan **4 fitur** (di luar kolom target dan ID). Untuk forecasting, syarat 4 fitur tidak berlaku.
3. Dataset **diusahakan kotor**, yaitu memiliki setidaknya salah satu dari outlier, missing value, atau duplikat. Jika dataset sudah bersih, penilaian tahap Cleaning dan Preprocessing tidak maksimal.
4. Dataset yang sudah tercatat di spreadsheet **tidak boleh digunakan kelompok lain**. Jika ada dataset kembar antar kelompok, kelompok yang tercatat lebih dulu yang berhak.
5. Dataset harus **asli, kredibel, dan valid**. Harus ada asal data, lisensi data, deskripsi masing-masing kolom yang jelas, serta hal lain yang membuktikan kredibilitas data.
6. Dataset **tidak boleh sintetis** atau data karangan sendiri.
7. Scraping data diperbolehkan asalkan dapat dipertanggungjawabkan. Sertakan hasil dan tanggal pengambilan.
8. **Dilarang** mengambil atau menggunakan **data pribadi**.

Contoh tempat mencari dataset: BPS, data.go.id, Satu Data Indonesia, World Bank, Our World in Data, UCI, Kaggle, paper ilmiah, dan sumber kredibel lainnya.

---

## 2. Pemilihan Model

- Satu kelompok memilih **salah satu metode**: Clustering, Klasifikasi, Regresi, atau Forecasting.
- Pemilihan metode harus sudah ada saat pengumpulan repository pada **30 Oktober 2026**.
- Model yang dipakai boleh lebih dari satu, tergantung keputusan kelompok dan karakteristik data.
- Model harus **bersumber dari materi praktikum**. Model di luar materi praktikum tidak dinilai.

---

## 3. Notebook

Output akhir proyek adalah **notebook yang selesai**, berisi alur lengkap dari Business Understanding sampai Konklusi, dengan semua hasil dan penjelasan tertulis di dalamnya.

Tidak perlu deployment, aplikasi web, API, atau dashboard. Penilaian tidak didasarkan pada bagus tidaknya output, tetapi pada **alasan dan proses berpikir** selama mengerjakan.

Isi notebook:

### a. Business Understanding
- Masalah
- Pertanyaan yang ingin dijawab
- Metode yang ingin digunakan
- Metrik yang digunakan

### b. Data Gathering
- Data yang dimuat
- Sumber dan tautan dataset
- Pengertian dataset: arti setiap kolom, data ini mengenai apa, kenapa memilih dataset ini, dan sebagainya

### c. EDA
- Statistik deskriptif
- Visualisasi data yang dibutuhkan untuk insight
- Penjelasan temuan di bawah setiap visual

### d. Cleaning dan Preprocessing
- Pengecekan data dan penanganan data berdasarkan hasil EDA
- Perlihatkan kondisi data **sebelum dan sesudah** diproses
- Proses **Feature Selection**, dengan penjelasan alasan membuang, membuat, dan menggunakan fitur

### e. Modelling
- Pemilihan dan pembuatan model
- Alasan di setiap kode yang dijalankan
- Jika memakai model pembanding, jelaskan perbandingan antar model

### f. Evaluasi
- Metrik penilaian dan grafik pendukung
- Jika memakai model pembanding, bandingkan metriknya dan jelaskan pemilihan model terbaik

### g. Konklusi
- Jawaban atas pertanyaan-pertanyaan di Business Understanding
- Terjemahan metrik atau temuan ke bahasa yang bermakna (contoh: "MAE 45 juta artinya prediksi harga rata-rata meleset sekitar 45 juta")
- Keputusan yang diambil
- Keterbatasan

---

## 4. Repository

Repository minimal berisi:

1. **README.md**, yang memuat:
   - Ringkasan proyek
   - Informasi anggota beserta kontribusinya
   - Sumber data
   - Panduan menjalankan proyek
2. **Notebook** yang sesuai ketentuan di atas
3. **Dataset** yang digunakan

---

## 5. Bobot Penilaian

| Komponen | Bobot |
|---|---|
| Business Understanding dan Data Gathering | 15 |
| EDA | 10 |
| Cleaning dan Preprocessing | 10 |
| Modelling | 10 |
| Evaluasi dan Konklusi | 20 |
| Pengumpulan Repository beserta kelengkapannya | 5 |
| Presentasi dan Tanya Jawab | 30 |
| **Total** | **100** |

Catatan:
- Penjelasan di sel markdown berdampak kuat pada penilaian notebook.
- Nilai anggota dalam satu kelompok bisa berbeda, terutama lewat tanya jawab individu.

---

## Checklist Cepat

- [ ] Dataset sudah dicatat di spreadsheet
- [ ] Dataset asli (bukan sintetis), ada sumber, lisensi, dan deskripsi kolom
- [ ] Minimal 100 baris dan 4 fitur (kecuali forecasting)
- [ ] Dataset mengandung data kotor (outlier, missing value, atau duplikat)
- [ ] Tidak memuat data pribadi
- [ ] Metode ditentukan sebelum 30 Oktober 2026
- [ ] Model hanya dari materi praktikum
- [ ] Notebook lengkap dari Business Understanding sampai Konklusi
- [ ] Penjelasan di markdown untuk setiap kode dan visual
- [ ] Kondisi data sebelum dan sesudah cleaning ditampilkan
- [ ] README.md berisi ringkasan, anggota dan kontribusi, sumber data, dan panduan menjalankan
- [ ] Notebook dan dataset ada di repository
- [ ] Semua anggota paham setiap keputusan untuk tanya jawab individu
