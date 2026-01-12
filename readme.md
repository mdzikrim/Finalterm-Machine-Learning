# Machine Learning & Deep Learning: Final Term Projects

Repositori ini berisi kumpulan proyek tugas akhir (Final Term) yang mencakup berbagai teknik **Machine Learning** dan **Deep Learning**. Proyek ini mendemonstrasikan kemampuan dalam menangani masalah regresi, klasifikasi data tidak seimbang (*imbalanced data*), dan pengenalan citra (*computer vision*).

---

## Ringkasan Proyek

### 1. Song Release Year Prediction (Regression)
**File:** `Finalterm_Regresi.ipynb`

Analisis ini bertujuan untuk memprediksi tahun rilis sebuah lagu berdasarkan 90 fitur audio yang diekstrak dari dataset musik skala besar.

* **Dataset:** 515,345 baris data (Million Song Dataset subset).
* **Model yang Digunakan:** Linear Regression, Random Forest, dan XGBoost Regressor.
* **Key Highlights:** * Implementasi *feature scaling* dengan `StandardScaler`.
    * Evaluasi menggunakan MAE, R², dan MSE.
* **Hasil Terbaik:** | Metric | Skor (XGBoost) |
    | :--- | :--- |
    | **MAE** | ±6.16 Tahun |
    | **R² Score** | 34.45% |
    | **Akurasi (±10 thn)** | 82.01% |

---

### 2. Fraudulent Transaction Detection (Classification)
**File:** `Finalterm_Transaction.ipynb`

Membangun model klasifikasi untuk mendeteksi transaksi kartu kredit yang bersifat penipuan (*fraud*) pada dataset yang sangat tidak seimbang.

* **Masalah Utama:** *Class Imbalance* (Jumlah transaksi normal jauh lebih banyak dari penipuan).
* **Solusi:** Penggunaan **SMOTE** (*Synthetic Minority Over-sampling Technique*) untuk menyeimbangkan kelas.
* **Model:** Random Forest Classifier & XGBoost.
* **Metrik Evaluasi:** Difokuskan pada **ROC-AUC** dan **F1-Score** untuk meminimalkan *false negatives*.

---

### 3. Fish Species Classification (Deep Learning - CNN)
**File:** `Finalterm_CNN.ipynb`

Implementasi jaringan syaraf tiruan konvensional (CNN) untuk mengklasifikasikan 31 jenis spesies ikan yang berbeda melalui gambar.

* **Arsitektur Model:** * 3 Lapisan `Conv2D` + `MaxPooling2D`.
    * `GlobalAveragePooling2D` untuk reduksi parameter.
    * `Dropout (0.5)` untuk mencegah overfitting.
* **Preprocessing:** * Resizing citra.
    * *Data Augmentation* (Horizontal Flip, Rotation).
* **Framework:** TensorFlow & Keras.

---

## Tech Stack

| Kategori | Teknologi |
| :--- | :--- |
| **Bahasa** | Python 3.x |
| **Analisis Data** | Pandas, NumPy |
| **Visualisasi** | Matplotlib, Seaborn |
| **ML Framework** | Scikit-Learn, XGBoost, Imbalanced-learn |
| **DL Framework** | TensorFlow, Keras |
| **Environment** | Google Colab / Jupyter Notebook |

---
