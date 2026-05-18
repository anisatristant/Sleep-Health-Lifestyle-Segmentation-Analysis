# 🌙 Sleep Health & Lifestyle Segmentation Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Machine-Learning-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Clustering](https://img.shields.io/badge/Algorithm-K--Means-green)](https://scikit-learn.org/stable/modules/clustering.html)

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk mengidentifikasi segmen atau profil gaya hidup masyarakat berdasarkan pola perilaku sehari-hari dan dampaknya terhadap kesehatan tidur. Menggunakan algoritma **K-Means Clustering**, penelitian ini mengeksplorasi hubungan antara konsumsi kafein, paparan layar (*screen time*), aktivitas fisik, dan jam kerja terhadap kualitas tidur serta tingkat stres.

## 📂 Struktur Repositori
Proyek ini disusun secara modular untuk memudahkan pengelolaan data dan analisis:
- **`data/`**: Berisi dataset mentah dalam format CSV.
- **`notebooks/`**: File Jupyter Notebook (.ipynb) yang berisi seluruh alur kerja mulai dari pembersihan data hingga pemodelan.
- **`images/`**: Kumpulan grafik hasil visualisasi analisis (untuk referensi visual).
- **`output/`**: Daftar data individu yang telah diberi label cluster (hasil segmentasi).

## 📊 Hasil Analisis dan Temuan Utama
Analisis ini menghasilkan 6 segmen gaya hidup yang berbeda secara signifikan. Berikut adalah poin-poin temuan utamanya:

### 1. Optimalitas Segmen
Berdasarkan pengujian menggunakan **Elbow Method** dan **Silhouette Score**, ditemukan bahwa pembagian populasi ke dalam **6 Cluster** memberikan hasil yang paling seimbang dan representatif bagi dataset ini.

### 2. Karakteristik Cluster (Profil Gaya Hidup)
Setiap kelompok memiliki pola perilaku yang unik:
*   **Cluster Sehat & Aktif:** Memiliki rata-rata langkah kaki di atas 8.000/hari, durasi olahraga rutin, dan konsumsi kafein yang minimal. Kelompok ini memiliki skor kualitas tidur tertinggi.
*   **Cluster Berisiko (High Screen Time):** Ditandai dengan penggunaan gadget di atas 60 menit sebelum tidur. Kelompok ini secara konsisten memiliki skor stres yang lebih tinggi.
*   **Cluster Pekerja Keras (High Workload):** Memiliki jam kerja harian yang tinggi. Meskipun aktif bergerak, kelompok ini seringkali memiliki durasi tidur yang lebih pendek namun efisiensi tidur yang stabil.

### 3. Dampak Terhadap Kesehatan
*   **Kualitas Tidur:** Terdapat korelasi positif yang kuat antara aktivitas fisik harian dengan skor kualitas tidur.
*   **Tingkat Stres:** Paparan layar sebelum tidur dan konsumsi alkohol/kafein yang berlebihan di malam hari menjadi pemicu utama rendahnya perasaan segar saat bangun (*felt rested*).

## 🛠️ Metodologi & Teknologi
- **Algoritma:** K-Means Clustering (Unsupervised Learning).
- **Preprocessing:** Standardisasi fitur menggunakan `StandardScaler` dan Reduksi Dimensi dengan `PCA`.
- **Library Utama:** `Pandas`, `NumPy`, `Scikit-Learn`, `Seaborn`, `Matplotlib`, dan `Yellowbrick`.

## 🚀 Cara Menjalankan Proyek
1. Clone repositori ini ke komputer Anda.
2. Install library yang diperlukan:
   ```bash
   pip install pandas scikit-learn seaborn matplotlib yellowbrick plotly

© 2026 [annisatristant]
