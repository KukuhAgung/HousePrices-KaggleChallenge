# 🏠 House Price Prediction : Kaggle Challenge

Ini adalah repositori untuk proyek saya dalam kompetisi [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) di Kaggle. Notebook ini mengeksplorasi, membersihkan, dan memodelkan data perumahan untuk memprediksi harga jual akhir.

---

## 📊 Analisis Model

Saya membandingkan beberapa model regresi. Visualisasi di bawah ini menunjukkan perbandingan akurasi prediksi antara model `LinearRegression` sederhana dengan model `RandomForestRegressor` yang lebih kompleks.

### 📈 Linear Regression
![Visualisasi Linear Regression]("attachment/linearprediction.png")
* **Analisis:** Model ini menangkap tren linier umum dari data, namun terlihat jelas kesulitan. Model ini secara konsisten melakukan **under-predict** (prediksi terlalu rendah) pada rumah-rumah mahal (puncak) dan **over-predict** (prediksi terlalu tinggi) pada rumah-rumah murah (lembah), menunjukkan bahwa model ini terlalu sederhana untuk dataset ini.
* **RMSE Latihan (Train):** 17493.130233735763

### 🌲 Random Forest Regressor
![Visualisasi Random Forest Regression]("attachment/randomforestprediction.png")
* **Analisis:** Model Random Forest memberikan kecocokan (*fit*) yang jauh lebih baik dan akurat. Model ini berhasil menangkap **pola non-linier** yang kompleks dalam data, serta mengikuti puncak dan lembah harga asli (Original) dengan jauh lebih presisi.
* **RMSE Latihan (Train):** 8224.505021708035

---

## 🎯 Hasil Akhir

Setelah melalui proses *feature engineering*, seleksi model, dan *hyperparameter tuning*, model final `RandomForestRegressor` berhasil mencapai skor berikut di leaderboard resmi Kaggle.

![Hasil Leaderboard]("attachment/leaderboard.png")

* **Skor Submission Final (RMSE):** 0.18797
* **Peringkat:** 4384

---

## 🔗 Tautan
[![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/userpdf)
* **Tautan Kompetisi:** [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/leaderboard)
* **Lihat Notebook (Opsional):** [Klik di sini untuk melihat notebook lengkap](https://...link-ke-notebook-anda...)
