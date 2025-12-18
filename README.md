# Telco Customer Churn Prediction

## 📌 Project Overview
Customer churn merupakan salah satu permasalahan utama pada industri telekomunikasi yang berbasis sistem langganan. Kehilangan pelanggan tidak hanya berdampak pada penurunan pendapatan, tetapi juga meningkatkan biaya akuisisi pelanggan baru.

Project ini bertujuan untuk membangun model machine learning yang dapat memprediksi customer churn sehingga perusahaan dapat melakukan tindakan preventif lebih awal terhadap pelanggan yang berisiko churn.

---

## 🎯 Business Problem
Perusahaan telekomunikasi kesulitan mengidentifikasi pelanggan yang berpotensi churn sebelum mereka benar-benar berhenti menggunakan layanan. Kesalahan yang paling merugikan adalah **False Negative**, yaitu pelanggan churn yang tidak terdeteksi oleh sistem, karena perusahaan kehilangan kesempatan untuk melakukan intervensi.

---

## 🧠 Objective
- Membangun model klasifikasi untuk memprediksi customer churn
- Meminimalkan False Negative
- Mendukung strategi retensi pelanggan melalui early warning system

---

## 📊 Dataset
Dataset berisi data pelanggan telekomunikasi yang mencakup:
- Informasi pelanggan (tenure, contract, layanan)
- Biaya bulanan dan total biaya
- Target variabel: **Churn (Yes / No)**

---

## 🔍 Exploratory Data Analysis (EDA)
Beberapa insight utama dari EDA:
- Distribusi target bersifat **imbalanced**, dengan pelanggan non-churn lebih banyak
- Pelanggan dengan **tenure rendah** memiliki kecenderungan churn lebih tinggi
- **Monthly charges tinggi** berasosiasi dengan peningkatan risiko churn

---

## 🧹 Data Preparation
Tahapan data preparation meliputi:
- Data cleaning dan handling missing values
- Encoding fitur kategorikal
- Feature preprocessing menggunakan pipeline
- Penanganan class imbalance

---

## 🤖 Modeling
- Problem type: **Binary Classification**
- Baseline model: **Logistic Regression**
- Alasan pemilihan:
  - Mudah diinterpretasikan
  - Cocok sebagai baseline model
  - Relevan untuk kebutuhan bisnis

---

## 📐 Evaluation Metric
Metric utama yang digunakan adalah **F2-score** karena:
- Memberikan bobot lebih besar pada **recall**
- Lebih sesuai dengan konteks bisnis di mana False Negative lebih merugikan daripada False Positive

---

## ⚙️ Hyperparameter Tuning
- Metode: **GridSearchCV**
- Objective: memaksimalkan **F2-score**
- Hasil tuning menunjukkan peningkatan performa model secara signifikan

---

## 📈 Model Performance
- F2-score meningkat dari **±0.56 (baseline)** menjadi **±0.72 (after tuning)**
- Recall untuk kelas churn meningkat
- Jumlah False Negative berhasil dikurangi

---

## 💼 Business Impact
Model ini dapat digunakan sebagai **early warning system** untuk:
- Mengidentifikasi pelanggan dengan risiko churn tinggi
- Mendukung program retensi seperti promo atau peningkatan layanan
- Mengurangi potensi kehilangan pendapatan

---

## 🚀 Deployment (Prototype)
Sebagai prototype, model ini di-deploy menggunakan **Streamlit** sehingga user dapat:
- Menginput data pelanggan
- Mendapatkan prediksi churn secara langsung

---

## 📝 Conclusion
Model machine learning yang dibangun berhasil meningkatkan kemampuan deteksi customer churn dengan fokus pada recall. Pendekatan ini selaras dengan kebutuhan bisnis yang ingin meminimalkan kehilangan pelanggan.

---

## 🔮 Recommendation
- Integrasi model ke sistem bisnis sebagai early warning system
- Penyesuaian threshold sesuai strategi bisnis
- Evaluasi dan retraining model secara berkala
- Penambahan fitur berbasis perilaku pelanggan

---

## 🛠️ Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn
- Streamlit
- Matplotlib & Seaborn

---

## 👩‍💻 Author
**Salma Almira Kuswihandono**  
Capstone Project – Machine Learning
