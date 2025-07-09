# 🛒 Prediksi Penjualan Harian dan Target Penjualan Toko

Proyek ini bertujuan untuk memprediksi **penjualan harian toko** (regresi) dan **klasifikasi target penjualan** (klasifikasi biner), berdasarkan data historis dan atribut toko. Proyek ini dibuat dalam rangka UAS Data Mining.

---

## 📦 Dataset

Dataset terdiri dari dua file:
- `train.csv`: Data penjualan harian tiap toko.
- `store.csv`: Informasi atribut tiap toko.

---

## ⚙️ Alur Proyek

1. **Data Preprocessing**
   - Merge dua dataset (`train` dan `store`)
   - Handle missing values & duplikasi
   - Feature engineering dari kolom tanggal
   - Encoding variabel kategorikal

2. **Task 1: Prediksi Penjualan (Regresi)**
   - 🎯 Tujuan: Prediksi jumlah penjualan (`Sales`)
   - Model yang digunakan:
     - Linear Regression
     - Random Forest Regressor

3. **Task 2: Klasifikasi Target Penjualan**
   - 🎯 Tujuan: Klasifikasi apakah penjualan di atas rata-rata (target tercapai)
   - Model yang digunakan:
     - SVM
     - Decision Tree
     - K-Nearest Neighbors (KNN)

4. **Evaluasi Model**
   - Regresi: RMSE, R²
   - Klasifikasi: Accuracy, F1 Score, Training Time

---

## 🧠 Hasil Evaluasi Model

### 🔢 Task 1: Regresi – Prediksi Sales Harian

| Model                  | RMSE     | R² Score |
|------------------------|----------|----------|
| Linear Regression      | 2173.77  | 0.614    |
| Random Forest Regressor| **985.36**   | **0.921**  |

### 🔠 Task 2: Klasifikasi – Target Penjualan

| Model         | Accuracy | F1 Score | Training Time |
|---------------|----------|----------|----------------|
| SVM           | 0.657    | 0.648    | 73.21 sec      |
| Decision Tree | 0.898    | 0.899    | 1.29 sec       |
| KNN           | **0.909**| **0.911**| 0.01 sec       |

---

## 📌 Insight

- **Random Forest** jauh lebih akurat daripada Linear Regression untuk prediksi penjualan harian.
- Untuk klasifikasi, **KNN** memberikan hasil terbaik dengan akurasi 91%.
- Fitur seperti promosi, jenis toko, dan waktu (bulan/hari) sangat mempengaruhi hasil prediksi.

---

## 📚 Tools & Library

- Python 3
- Pandas, NumPy
- Scikit-Learn
- Matplotlib, Seaborn
- Jupyter Notebook


