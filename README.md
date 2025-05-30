# Decision3_UCI_Spam_Dataset 
Explorasi Data Analisis on UCI Spam Dataset - Tugas kelompok AI
# Decision3-UCI Spam Dataset
Analisis eksplorasi data untuk UCI Spam Dataset.

## Anggota Kelompok

-AHMAD JAZULI ROFI
-M YUZRIL FAIZIN

## Cara menjakankan
Buka file .ipynb di Google Colab/Jupyter.

# 📧 Spam Email Detection with Decision Tree

Deteksi apakah sebuah email merupakan spam atau bukan menggunakan algoritma *Decision Tree Classifier*.

## 🧠 Deskripsi Proyek

Proyek ini bertujuan untuk mengklasifikasikan email sebagai **spam** atau **bukan spam** (ham) menggunakan algoritma Decision Tree. Dataset yang digunakan adalah dataset publik dari UCI Spambase yang berisi fitur-fitur numerik hasil ekstraksi konten email.

## 🔍 Jenis Masalah

- **Tipe Masalah**: Klasifikasi Biner
- **Tujuan**: Memprediksi apakah email adalah spam (1) atau bukan spam (0)
- **Dataset**: [UCI Spambase Dataset](https://archive.ics.uci.edu/ml/datasets/Spambase)

## 📁 Struktur Dataset

Dataset memiliki 57 fitur numerik yang merepresentasikan:

- Frekuensi kata seperti "free", "money", dll.
- Frekuensi karakter khusus seperti `!`, `$`, dan `;`.
- Statistik huruf kapital dalam email.
- Label target: `1` = Spam, `0` = Not Spam

## ⚙️ Tahapan Penyelesaian

1. **Load dataset** dari UCI
2. **Preprocessing** dan pembagian data train/test
3. **Pelatihan model Decision Tree**
4. **Evaluasi model** menggunakan akurasi, precision, recall, dan confusion matrix
5. **Cross-validation**
6. **Tuning parameter model** menggunakan GridSearchCV
7. **Simpan model** dalam file `.pkl`
8. **Visualisasi pohon keputusan & confusion matrix**

## 🧪 Metrik Evaluasi

- **Accuracy**: Mengukur prediksi benar secara keseluruhan
- **Precision**: Seberapa tepat model dalam mendeteksi spam
- **Recall**: Seberapa banyak spam berhasil terdeteksi
- **F1-Score**: Harmonik rata-rata precision dan recall
- **Confusion Matrix**: Visualisasi prediksi vs label asli

## 📊 Hasil Akhir

- **Akurasi Awal**: ~93%
- **Best Cross-Validated Model**:
  - Akurasi: >94% (tergantung parameter GridSearch)
  - Precision & Recall tinggi untuk deteksi spam
- Model berhasil meminimalkan kesalahan klasifikasi spam & non-spam

## 🧠 Teknologi yang Digunakan

- Python 3
- Scikit-learn
- Pandas, NumPy
- Matplotlib & Seaborn
- Jupyter Notebook / Google Colab

## 💾 Simpan & Deploy Model

Model akhir disimpan ke file:

```bash
spam_classifier_decision_tree.pkl
