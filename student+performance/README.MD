# Evaluasi Model Machine Learning & Perintah Git

Dokumen ini berisi penjelasan mengenai metrik evaluasi model regresi (MAE, RAE, MSE, RMSE, R² Score) serta daftar perintah Git yang digunakan untuk mengunggah proyek ke GitHub.

---

## 1. Analisis Metrik Evaluasi Regresi

Dalam pemodelan *Machine Learning* untuk kasus regresi, metrik evaluasi digunakan untuk mengukur seberapa akurat nilai prediksi model dibandingkan dengan nilai sebenarnya.

### **Apakah Nilai Metrik Harus Mendekati 1 atau 0?**

* **$R^2$ Score (Coefficient of Determination)**
  * **Target Ideal:** **Mendekati 1 (atau 100%)**
  * **Penjelasan:** Metrik ini mengukur seberapa baik variasi data dapat dijelaskan oleh model. Nilai $1$ menunjukkan bahwa prediksi model sempurna tanpa ada kesalahan.

* **MAE (Mean Absolute Error)**
  * **Target Ideal:** **Mendekati 0**
  * **Penjelasan:** Mengukur rata-rata selisih mutlak antara nilai asli dan nilai prediksi. Semakin kecil nilainya (mendekati 0), semakin kecil tingkat kesalahan model.

* **MSE (Mean Squared Error)**
  * **Target Ideal:** **Mendekati 0**
  * **Penjelasan:** Rata-rata dari kuadrat kesalahan. Nilai yang makin mendekati 0 menunjukkan performa model yang semakin baik.

* **RMSE (Root Mean Squared Error)**
  * **Target Ideal:** **Mendekati 0**
  * **Penjelasan:** Akar kuadrat dari MSE untuk mengembalikan skala kesalahan ke satuan data asli. Nilai mendekati 0 menunjukkan tingkat kesalahan yang sangat rendah.

* **RAE (Relative Absolute Error)**
  * **Target Ideal:** **Mendekati 0 (atau 0%)**
  * **Penjelasan:** Rasio perbandingan antara kesalahan model dibanding kesalahan model dasar (*baseline*). Nilai mendekati 0 berarti model jauh lebih baik dibanding hanya menebak nilai rata-rata.

---

## 2. Ringkasan Target Metrik Evaluasi

| Metrik Evaluasi | Target Nilai Ideal | Keterangan |
| :--- | :--- | :--- |
| **MAE** | Mendekati 0 | Mengukur besarnya error rata-rata |
| **MSE** | Mendekati 0 | Memberikan penalti pada error besar |
| **RMSE** | Mendekati 0 | Skala error disesuaikan ke satuan data asli |
| **RAE** | Mendekati 0 (0%) | Rasio kesalahan dibanding model *baseline* |
| **$R^2$ Score** | **Mendekati 1 (100%)** | Mengukur sejauh mana model menjelaskan variasi data |

---

