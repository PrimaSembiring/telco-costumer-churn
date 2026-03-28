# Customer Churn Prediction

## Deskripsi

Proyek ini bertujuan untuk membangun model machine learning dalam memprediksi kemungkinan pelanggan melakukan *churn* (berhenti berlangganan). Prediksi ini penting bagi perusahaan untuk mengidentifikasi pelanggan yang berisiko dan mengambil tindakan pencegahan guna meningkatkan retensi pelanggan.

---

## 📂 Dataset

link dataset : https://www.kaggle.com/code/bhartiprasad17/customer-churn-prediction
Dataset yang digunakan merupakan dataset *Customer Churn* yang berisi informasi terkait pelanggan, seperti:

* Data demografis pelanggan
* Jenis layanan yang digunakan
* Informasi kontrak
* Biaya layanan (monthly & total charges)
* Status churn (target)

Target variabel:

* `Churn` →

  * 0: Tidak churn
  * 1: Churn

---

## Tahapan Analisis

Proses analisis dalam proyek ini meliputi beberapa tahap utama:

### 1. Data Preprocessing

* Pembersihan data (missing value handling)
* Encoding variabel kategorikal
* Feature scaling menggunakan StandardScaler
* Penanganan data imbalance menggunakan SMOTE

---

### 2. Modeling

Beberapa algoritma machine learning yang digunakan:

* Logistic Regression
* Random Forest
* LightGBM
* XGBoost

---

### 3. Evaluasi Model

Model dievaluasi menggunakan metrik:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Fokus utama evaluasi adalah **recall pada kelas churn**, karena penting untuk mendeteksi pelanggan yang berpotensi berhenti.

---

## 📊 Hasil dan Insight

Hasil menunjukkan bahwa:

* Logistic Regression memiliki recall tertinggi dalam mendeteksi churn
* Random Forest memberikan performa yang cukup seimbang
* LightGBM menghasilkan performa terbaik secara keseluruhan
* XGBoost memiliki performa yang relatif lebih rendah dalam mendeteksi churn

---

## Kesimpulan

Pemilihan model terbaik bergantung pada tujuan bisnis:

* Jika fokus pada deteksi churn → Logistic Regression
* Jika fokus pada keseimbangan performa → LightGBM

Secara umum, **LightGBM dipilih sebagai model terbaik** karena memberikan kombinasi akurasi dan stabilitas yang optimal.

---


## Catatan

Model masih dapat ditingkatkan melalui:

* Hyperparameter tuning
* Feature engineering tambahan
* Eksplorasi metode balancing lainnya

