# Supervised Learning - Regression

Repository ini berisi materi hands-on project untuk memprediksi harga rumah menggunakan metode **Linear Regression** (Regresi Linear).

## Deskripsi
Program ini merupakan latihan *Supervised Learning* menggunakan bahasa pemrograman Python. Dataset yang digunakan dalam latihan ini adalah dataset bawaan Google Colab, yaitu `USA_Housing.csv`. 

Jupyter Notebook di dalam repository ini (`Supervised_Learning_Hands_On_Regresi.ipynb`) mencakup tahapan-tahapan machine learning dari awal hingga evaluasi model, antara lain:
1. **Preparation**: Mengimpor seluruh library yang dibutuhkan.
2. **Exploratory Data Analysis (EDA)**: Melakukan pengecekan data, statistika deskriptif, dan visualisasi data untuk memahami korelasi antar variabel.
3. **Modeling**: Membangun model machine learning menggunakan algoritma *Linear Regression*.
4. **Evaluation**: Menguji akurasi model menggunakan metrik evaluasi regresi.

## Dependencies / Library yang Digunakan
Pastikan Anda sudah menginstal library berikut sebelum menjalankan program:
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn` (`sklearn`)
- `statsmodels`
- `scipy`

## Kesimpulan Evaluasi Model
Dari hasil pengujian model, diperoleh beberapa kesimpulan sebagai berikut:
1. **Error yang relatif rendah:** Rata-rata kesalahan prediksi model (MAE) berada di sekitar **8.17%** dari harga rumah rata-rata.
2. **Akurasi sangat baik:** Model memiliki skor **R-squared (R²) sekitar 0.92**, yang berarti model ini mampu menjelaskan **92% variansi** dalam data uji. 
3. **Outliers:** Nilai RMSE yang sedikit lebih tinggi dari MAE menunjukkan adanya beberapa prediksi dengan error yang cukup besar (outliers), namun secara keseluruhan masih dalam batas yang wajar.

## Cara Menjalankan
1. *Download* atau salin file `Supervised_Learning_Hands_On_Regresi.ipynb`.
2. Upload notebook tersebut ke Google Colab atau jalankan di Jupyter environment lokal.
3. Pastikan file dataset `USA_Housing.csv` berada di direktori yang sama, lalu jalankan setiap sel (cell) secara berurutan.
