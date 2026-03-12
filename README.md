# California-Housing-FE
A comprehensive Feature Engineering approach to optimize the California Housing dataset for Machine Learning. This project focuses on data distribution analysis, outlier detection, and advanced scaling techniques to improve model readiness.

# 🏠 California Housing: Feature Engineering & Data Preprocessing

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![SciPy](https://img.shields.io/badge/Library-SciPy-8CAAE6?logo=scipy&logoColor=white)](https://scipy.org/)

## 📌 Project Overview
Tujuan utama dari proyek ini adalah melakukan **Feature Engineering** tingkat lanjut pada *California Housing Dataset*. Sebelum data masuk ke tahap pemodelan, sangat penting untuk memastikan fitur-fitur memiliki distribusi yang baik dan bebas dari gangguan *outliers* yang dapat menurunkan performa model.

Proyek ini mencakup alur kerja *data science* yang sistematis:
* **Analisis Statistik:** Menguji normalitas data menggunakan Probability Plots.
* **Visualisasi Distribusi:** Identifikasi *skewness* dengan Histogram dan Boxplots.
* **Data Splitting:** Memisahkan data untuk validasi yang objektif (Train-Test Split).

## 📂 Dataset
Dataset yang digunakan adalah data perumahan di California yang mencakup variabel ekonomi dan geografis.
* **Fitur Utama:**
    * `MedInc`: Pendapatan median di blok tersebut.
    * `HouseAge`: Usia median rumah.
    * `AveRooms`: Rata-rata jumlah kamar.
    * `AveBedrms`: Rata-rata jumlah kamar tidur.
    * `AveOccup`: Rata-rata hunian rumah tangga.
* **Target:** `MedHouseVal` (Nilai rumah median).

## 🛠️ Methodology

### 1. Data Splitting
Data dibagi menjadi dua bagian menggunakan `train_test_split` dari Scikit-Learn untuk menghindari *data leakage*:
* **Train Set (80%):** Digunakan untuk analisis dan fit transformasi.
* **Test Set (20%):** Digunakan untuk evaluasi akhir.

### 2. Exploratory Data Analysis (EDA)
Kami melakukan inspeksi visual mendalam pada variabel kunci:
* **Histogram:** Untuk melihat kemiringan (*skewness*) data.
* **Boxplot:** Untuk mengidentifikasi titik-titik data ekstrem (*outliers*).
* **Probability Plot (Q-Q Plot):** Untuk membandingkan distribusi data dengan distribusi normal teoritis menggunakan `scipy.stats`.

### 3. Feature Scaling & Transformation
Untuk mempersiapkan data bagi algoritma machine learning, kami menyiapkan alat untuk:
* **StandardScaler:** Menghasilkan data dengan mean 0 dan standar deviasi 1.
* **MinMaxScaler:** Mengubah rentang data menjadi [0, 1].

## 📊 Summary of Features Analysis

| Feature | Visual Analysis | Statistical Tool | Purpose |
| :--- | :--- | :--- | :--- |
| **MedInc** | Histogram | Skewness Check | Identify income distribution |
| **AveRooms** | Boxplot | Outlier Detection | Filter extreme housing values |
| **HouseAge** | Probability Plot | Normality Test | Check for Gaussian distribution |

## 🚀 How to Run
1.  Clone repository ini:
    ```bash
    git clone [[https://github.com/username/california-housing-fe.git](https://github.com/username/california-housing-fe.git](https://github.com/RandiBro234/FeatureEngineering-MachineLearningOps-Randi-Nandika-Danendra))
    ```
2.  Install library yang dibutuhkan:
    ```bash
    pip install pandas numpy matplotlib scipy scikit-learn
    ```
3.  Jalankan notebook:
    ```bash
    jupyter notebook "3324600013_Feature_Engineering_(1)_Randi_Nandika_Danendra.ipynb"
    ```

## 🤝 Conclusion
Tahap *Feature Engineering* ini sangat krusial. Dengan menangani *outliers* dan memahami distribusi fitur melalui visualisasi statistik, data siap untuk diproses oleh algoritma regresi dengan hasil yang lebih stabil dan akurat.

---
*Created by [Randi Nandika Danendra]*
