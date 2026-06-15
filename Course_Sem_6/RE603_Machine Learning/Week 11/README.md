# Analisis Fungsi Aktivasi MLP pada Dataset Iris

Repositori ini berisi analisis perbandingan performa arsitektur jaringan saraf tiruan **Multi-Layer Perceptron (MLP)** menggunakan tiga fungsi aktivasi yang berbeda: **Sigmoid (Logistic)**, **Tanh (Hyperbolic Tangent)**, dan **ReLU (Rectified Linear Unit)** menggunakan dataset Iris.

## 📋 Deskripsi Proyek
Proyek ini bertujuan untuk mengevaluasi bagaimana pemilihan fungsi aktivasi memengaruhi metrik evaluasi model klasifikasi pada dataset yang relatif sederhana dan arsitektur MLP yang dangkal.

### Arsitektur Jaringan:
* **Hidden Layers:** 2 Layer dengan masing-masing 10 neuron `(hidden_layer_sizes=(10, 10))`
* **Proporsi Data:** 70% Training, 30% Testing (Stratified)
* **Penskalaan Fitur:** `StandardScaler` (Z-score normalization)
* **Maksimum Iterasi:** 2000

---

## 📊 Hasil Evaluasi

Berikut adalah hasil performa dari masing-masing fungsi aktivasi setelah dilakukan pengujian:

| Fungsi Aktivasi | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Tanh** | **0.955556** | **0.955556** | **0.955556** | **0.955556** |
| **Sigmoid** | 0.933333 | 0.934524 | 0.933333 | 0.933259 |
| **ReLU** | 0.911111 | 0.915535 | 0.911111 | 0.910714 |

---

## 📌 Kesimpulan
1. **Tanh** memberikan performa paling optimal dan seimbang di seluruh metrik evaluasi dengan akurasi mencapai **95,56%**. Sifatnya yang *zero-centered* membantu stabilitas pada arsitektur kecil ini.
2. **Sigmoid** menempati posisi kedua dengan akurasi **93,33%**, membuktikan bahwa fungsi non-linear klasik masih sangat mumpuni untuk dataset linear-terpisah seperti Iris.
3. **ReLU** secara tidak terduga menghasilkan performa terendah (**91,11%**). Hal ini menunjukkan bahwa pada arsitektur dangkal dan dataset sederhana, keunggulan ReLU dalam mencegah *vanishing gradient* tidak terlalu berdampak signifikan dibandingkan fungsi aktivasi berbasis *smooth-curve* seperti Tanh.

---
