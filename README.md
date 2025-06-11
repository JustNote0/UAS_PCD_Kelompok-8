
# 🍇 Klasifikasi Daun Anggur Menggunakan Metode LBP, GLCM, dan SVM

## 📌 Deskripsi Singkat Proyek

Proyek ini bertujuan untuk mengembangkan model klasifikasi daun anggur berdasarkan fitur tekstur citra menggunakan metode ekstraksi **Local Binary Pattern (LBP)** dan **Gray Level Co-occurrence Matrix (GLCM)**, serta diklasifikasikan dengan algoritma **Support Vector Machine (SVM)**. Data yang digunakan berasal dari _Grapevine Leaves Image Dataset_ di Kaggle.

---

## 👩‍💻 Anggota Kelompok

Kelompok 8 - Mata Kuliah Pengolahan Citra Digital:

- Nurus Shobah Hidayati (163)
- Ananda Sakinah (060)
- Permata Witjaksana P. (098)

---

## 📂 Struktur Proyek

```
.
├── Poster PCD_Kelompok 8.png         # Ringkasan hasil proyek dalam bentuk visual poster
├── Progres1_PCD_Kelompok_8.ipynb     # Notebook lengkap berisi langkah-langkah EDA, preprocessing, dan modelling
├── README.md                         # File ini
```

---

## 📊 Dataset

- **Sumber**: [Grapevine Leaves Image Dataset (Kaggle)](https://www.kaggle.com/datasets/muratkokludataset/grapevine-leaves-image-dataset)
- **Kelas**: 5 Jenis daun anggur (`Ak`, `Ala_Idris`, `Dimnit`, `Nazli`, `Burgundy`)

---

## 🧪 Metodologi

1. **Exploratory Data Analysis (EDA)**  
   - Menampilkan contoh gambar dari setiap kelas
   - Melihat distribusi kelas
   - Visualisasi sampel gambar
   - Cek ukuran, duplikasi, dan kualitas gambar

2. **Preprocessing Data**
   - Resize gambar untuk keseragaman ukuran
   - Konversi gambar ke grayscale
   - Enhancement Menggunakan CLAHE

4. **Ekstraksi Fitur**  
   - **Local Binary Pattern (LBP)**: untuk mendeskripsikan tekstur lokal
   - **Gray Level Co-occurrence Matrix (GLCM)**: untuk mengekstrak fitur statistik dari tekstur (contrast, correlation, energy, dll.)
   - Penggabungan kedua macam ekstraksi fitur (**LBP & GLCM**)

5. **Model Training & Evaluasi**
   - Algoritma klasifikasi: **Support Vector Machine (SVM)**
   - Evaluasi menggunakan:
     - Confusion Matrix
     - Classification Report (Precision, Recall, F1-Score, Accuracy)

---

## 🧾 Hasil

- **Akurasi**: ~18%
- **F1-Score Tertinggi**: Ala_Idris (0.26)
- **Kesimpulan**: Model dengan fitur LBP dan GLCM serta SVM masih belum mampu membedakan antar kelas dengan baik. Diperlukan:
  - Fitur yang lebih representatif
  - Preprocessing lanjutan
  - Parameter tuning

---

## 💡 Insight & Analisis

- Kelas tertentu seperti `Dimnit` dan `Nazli` tidak terklasifikasi sama sekali → menunjukkan kebutuhan akan representasi fitur yang lebih baik
- Kinerja rendah dari SVM bisa disebabkan karena overlap karakteristik antar daun atau ketidakseimbangan data

---

## 🚀 Cara Menjalankan Proyek

1. Clone repository ini:

```bash
git clone https://github.com/username/klasifikasi-daun-anggur.git
cd klasifikasi-daun-anggur
```

2. Buka file `.ipynb` menggunakan Google Colab atau Jupyter Notebook.

3. Pastikan kamu memiliki `kaggle.json` untuk mengakses dataset.

4. Jalankan setiap sel secara berurutan untuk melihat hasilnya.

---

## 🛠️ Alat yang Digunakan

- Python
- Google Colab
- OpenCV
- Scikit-learn
- NumPy
- Matplotlib
- Kaggle API

---

## 📌 Catatan

Poster proyek ini dapat dilihat pada file [`Poster PCD_Kelompok 8.png`](./Poster%20PCD_Kelompok%208.png) sebagai ringkasan visual dari seluruh eksperimen.

---


