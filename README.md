# Prediksi Harga Mobil Bekas Menggunakan Regresi Linear

Repositori ini berisi *notebook* proyek untuk Ujian Tengah Semester (UTS) mata kuliah Data Mining. Proyek ini bertujuan untuk membangun model *machine learning* yang dapat memprediksi harga mobil bekas.

- **Nama:** Rizky Baruna
- **NPM:** 2310631170115
- **Kelas:** 5A Informatika

---

## 📝 Deskripsi Proyek

Proyek ini berfokus pada pembangunan model Regresi Linear untuk mengestimasi harga mobil bekas berdasarkan berbagai atribut yang relevan. Model dilatih untuk menemukan pola dan hubungan antara fitur-fitur mobil (seperti tenaga mesin, kilometer yang telah ditempuh, dan tahun pembuatan) dengan harga jualnya di pasaran.

## 💾 Dataset

Dataset yang digunakan adalah **"Used Cars Price Prediction"**, yang berisi informasi mengenai 6019 mobil bekas. Fitur-fitur utama dalam dataset ini antara lain:

- `Name`, `Location`, `Year`, `Kilometers_Driven`
- `Fuel_Type`, `Transmission`, `Owner_Type`
- `Mileage`, `Engine`, `Power`, `Seats`
- `Price` (sebagai variabel target yang akan diprediksi)

## ⚙️ Metodologi

Proyek ini mengikuti alur kerja standar dalam *data science*, yang terdiri dari beberapa tahapan utama:

1.  **Data Profiling & EDA:** Memahami struktur data, distribusi, dan korelasi antar fitur menggunakan statistik deskriptif, histogram, dan *heatmap*.
2.  **Data Cleaning:** Menangani nilai yang hilang (*null values*) dengan metode imputasi rata-rata dan menghapus data pencilan (*outliers*) yang signifikan (sebanyak 29.14% dari data).
3.  **Feature Selection:** Menganalisis varians fitur menggunakan `VarianceThreshold` untuk mengidentifikasi fitur yang paling informatif.
4.  **Modelling:** Mempersiapkan data dengan *Label Encoding* dan *Standard Scaling*, kemudian melatih model Regresi Linear setelah membagi data menjadi set latih dan set uji.
5.  **Evaluasi Model:** Mengevaluasi performa model dengan membandingkan harga aktual dan harga prediksi menggunakan visualisasi *scatter plot*.

## 📊 Hasil Utama

- Dari analisis data, ditemukan bahwa fitur **`Power` (tenaga mesin)** dan **`Engine` (kapasitas mesin)** memiliki korelasi positif terkuat terhadap `Price`.
- Model Regresi Linear yang dibangun menunjukkan performa yang cukup baik, di mana hasil prediksi cenderung mengikuti pola harga aktual seperti yang ditunjukkan pada *scatter plot* evaluasi.

## 🚀 Cara Menjalankan

1.  Pastikan Anda memiliki lingkungan yang dapat menjalankan Jupyter Notebook (disarankan menggunakan **Google Colab**).
2.  Buka file `UTS_Rizky Baruna_23115 - Colab.ipynb`.
3.  Jalankan sel-sel kode secara berurutan dari atas ke bawah. Seluruh *library* yang dibutuhkan sudah diimpor di dalam *notebook*.

## 🛠️ Teknologi yang Digunakan

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
