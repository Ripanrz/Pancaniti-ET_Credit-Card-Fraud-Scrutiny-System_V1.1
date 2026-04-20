# 💳 Pancaniti ET: Credit Card Fraud Scrutiny System V1.1

<div align="center">
  
  [![Open In Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/12peErYzbbNVDRtiMl7kLFCQxeY4G30-0?usp=sharing)
  [![Hugging Face Model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Models-yellow?style=for-the-badge)](https://huggingface.co/Ripanrz/credit-card-fraud-et-v1.1)
  [![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
  [![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)

</div>

---

## 📝 Deskripsi Proyek
***Pancaniti ET: Credit Card Fraud Scrutiny System V1.1*** merupakan iterasi stabil dari sistem deteksi penipuan kartu kredit yang mengutamakan integritas data asli. 

Berbeda dengan versi sebelumnya, V1.1 **tidak menggunakan teknik Hybrid Resampling (SMOTE + Undersampling)**. Model dilatih langsung menggunakan distribusi data asli untuk memastikan bahwa pola yang dipelajari adalah representasi murni dari transaksi nyata. Dengan menggunakan algoritma **Extra Trees Classifier**, sistem ini terbukti sangat tangguh dalam menangani ketimpangan data tanpa terjebak dalam masalah *overfitting*.

---

## 🚀 Fitur Utama
* **Original Data Training**: Melatih model pada distribusi data asli untuk menghindari distorsi dari data sintetis.
* **Good Fit Performance**: Performa stabil di mana hasil evaluasi data latih dan data uji memiliki selisih yang sangat kecil (Aman dari Overfitting).
* **Robust Feature Scaling**: Menggunakan `RobustScaler` untuk menangani fitur `Time` dan `Amount` yang memiliki *outlier* ekstrem.
* **Cloud Integration**: Model dikemas dan dideploy secara otomatis ke **Hugging Face Hub** untuk aksesibilitas yang lebih luas.

---

## 🧠 Metodologi V1.1: Stabilitas adalah Kunci
Pada versi ini, fokus dialihkan dari "menyeimbangkan jumlah data" menjadi "mengoptimalkan pembelajaran algoritma". 

1. **Efisiensi Extra Trees**: Algoritma ini secara alami sangat baik dalam melakukan generalisasi pada data yang kompleks.
2. **Eliminasi Bias**: Tanpa SMOTE, model tidak berisiko menghafal data buatan, sehingga prediksi pada data dunia nyata menjadi lebih objektif.
3. **Validasi Ketat**: Menyertakan pengecekan otomatis selisih *F1-Score* antara fase *Train* dan *Test* untuk menjamin model tidak *overfit*.

---

## 🛠️ Tech Stack
| Komponen | Teknologi |
| :--- | :--- |
| **Bahasa** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| **Modeling** | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) |
| **Manipulasi Data** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/Numpy-013243?style=flat-square&logo=numpy&logoColor=white) |
| **Deployment** | ![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Repository-FFD21E?style=flat-square) |

---

## 📊 Hasil Evaluasi & Stabilitas
Model V1.1 menunjukkan karakteristik **Good Fit**. Hal ini dibuktikan dengan:
- **Akurasi & F1-Score**: Nilai yang konsisten tinggi baik pada data latih maupun data uji.
- **Confusion Matrix**: Kemampuan deteksi kelas *Fraud* yang tajam dengan tingkat *False Positive* yang sangat rendah.
- **Generalisasi**: Model siap digunakan untuk data transaksi baru karena tidak "menghafal" data latihan secara berlebihan.

<div align="center">
  <img src="hasil-evaluasi-credit-card-fraud-et-v1.1.png" alt="Hasil Evaluasi V1.1" width="800">
</div>

---

## 🌐 Akses Model
Model stabil versi 1.1 tersedia untuk publik di sini:
👉 **[Hugging Face Repository - V1.1](https://huggingface.co/Ripanrz/credit-card-fraud-et-v1.1)**

---
***Project dikembangkan sebagai bagian dari eksperimen sistem keamanan finansial berbasis AI yang aman dan stabil.***
