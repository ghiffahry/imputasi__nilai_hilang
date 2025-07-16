# 🧠 Studi Imputasi Data Hilang — Evaluasi Enam Metode dari Statistika hingga Reinforcement Learning

Selamat datang di repositori proyek simulasi ini!  
Studi ini mengevaluasi berbagai metode **imputasi data hilang** pada data akademik simulasi nilai mahasiswa. Kami membandingkan pendekatan dari **statistika dasar**, **pembelajaran mesin**, hingga **reinforcement learning (RL)**.

---

## 🎯 Tujuan Penelitian

Menilai efektivitas **enam metode imputasi** dalam mengembalikan nilai yang hilang secara acak (15% MCAR) pada data nilai 300 mahasiswa dari 9 mata kuliah. Data disimulasikan dengan sebaran berbeda (Normal, Gamma, Beta) untuk mencerminkan kompleksitas data dunia nyata.

---

## 🔬 Metode yang Digunakan

1. **Rataan (Mean)**
2. **Nilai Tengah (Median)**
3. **K-Nearest Neighbors (KNN)**
4. **Fuzzy K-Means Clustering**
5. **Isolation Forest**
6. **Reinforcement Learning (RL)**

---

## 📈 Hasil Utama

- **Statistika Dasar (Mean, Median):**  
  Cocok untuk data simetris, namun kurang akurat jika data multimodal atau memiliki pencilan.  
  *RMSE: 0.316–0.329*

- **Machine Learning (KNN, Fuzzy K-Means):**  
  Unggul pada struktur multivariat, dengan hasil terbaik pada Fuzzy K-Means (*RMSE: 0.316*).  
  Butuh normalisasi dan tuning parameter. Isolation Forest, bagus dalam deteksi pencilan,
  tapi kurang cocok untuk konteks imputasi data kompleks (*RMSE: 0.324*).

- **Reinforcement Learning (RL):**  
  Paling akurat dan mampu mempertahankan sebaran asli data dengan kebijakan berbasis reward.  
  *RMSE: 0.022, MAE: 0.015*

---

## 📌 Insight & Rekomendasi

- Gunakan **mean/median** untuk dataset kecil dan tidak terlalu banyak amatan hilang.
- Pilih **KNN atau Fuzzy** untuk data kompleks dan berkorelasi.
- Gunakan **RL** jika presisi tinggi dibutuhkan dan tersedia sumber daya komputasi.
- Hindari Isolation Forest jika data memiliki distribusi multimodal.
- Validasi sebaran pasca-imputasi sangat penting dalam studi akademik atau pendidikan.

---
