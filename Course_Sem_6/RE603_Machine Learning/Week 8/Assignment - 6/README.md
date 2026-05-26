# Analisis Clustering K-Means pada Dataset WineQT

Repository ini berisi proyek analisis data menggunakan algoritma pembelajaran tanpa pengawasan (*unsupervised learning*), secara spesifik **K-Means Clustering**, untuk mengelompokkan variasi karakteristik kualitas anggur (*wine*).

## 📌 Identitas Pemilik
* **Nama:** Tamam Kurnia
* **NIM:** 4222311009
* **Kelas:** Malam A

---

## 📂 Ringkasan Proyek
Proyek ini mengimplementasikan algoritma K-Means untuk mengelompokkan data fisikokimia dari sampel *wine*. Hasil pengelompokkan (cluster) kemudian dievaluasi menggunakan **Elbow Method** dan **Silhouette Score**, serta dibandingkan secara visual dengan label kualitas asli (*ground-truth annotation*) bawaan dataset.

### Komponen Utama Notebook:
1. **Data Preparation & Loading:** Memuat file `WineQT.csv` ke dalam struktur data pandas.
2. **Exploratory Data Analysis (EDA):** Analisis statistik deskriptif, pengecekan nilai yang hilang (*missing values*), visualisasi distribusi kelas `quality`, serta analisis matriks korelasi menggunakan *heatmap*.
3. **Feature Engineering:** Pembersihan data duplikat, penghapusan kolom yang tidak relevan (`Id`), pemisahan fitur dengan label, serta transformasi skala fitur menggunakan `StandardScaler`.
4. **K-Means Clustering:** Pembentukan model awal dengan konfigurasi 3 cluster ($k=3$).
5. **Optimasi & Evaluasi Model:**
   * Penentuan jumlah cluster optimal via **Elbow Method** (Inertia).
   * Perhitungan skor segmentasi menggunakan **Silhouette Score**.
   * Visualisasi analisis Silhouette per cluster.
6. **Visualisasi Komparatif:** Membandingkan sebaran sekelompok fitur utama (`alcohol` vs `volatile acidity`) berdasarkan hasil cluster K-Means dengan label kualitas aslinya.

---

## 🛠️ Library yang Digunakan
Proyek ini dibangun menggunakan bahasa pemrograman Python dengan pustaka pendukung sebagai berikut:
* **Manipulasi Data:** `numpy`, `pandas`
* **Visualisasi Data:** `matplotlib`, `seaborn`
* **Machine Learning & Evaluasi:** `scikit-learn` (`StandardScaler`, `KMeans`, `silhouette_score`, `silhouette_samples`)

---