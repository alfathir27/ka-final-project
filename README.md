# Deteksi Dini Pneumonia pada Citra X-Ray Paru

## Deskripsi Proyek

Proyek ini merupakan tugas akhir mata kuliah **Kecerdasan Artifisial** yang bertujuan untuk mendeteksi penyakit pneumonia pada citra X-Ray paru-paru menggunakan teknik **Hybrid Feature Extraction (HOG & LBP)** dengan analisis komparatif tiga model machine learning berbeda.

## Video Presentasi

[![Video Presentasi](https://img.youtube.com/vi/UZ1dce4G9y4/0.jpg)](https://youtu.be/UZ1dce4G9y4)

**Link:** https://youtu.be/UZ1dce4G9y4

## Tujuan

Mengembangkan sistem deteksi dini pneumonia yang akurat dengan membandingkan performa beberapa model klasifikasi:
- **Decision Tree**
- **Random Forest**
- **XGBoost**

## Fitur Utama

- Ekstraksi fitur menggunakan kombinasi **Histogram of Oriented Gradients (HOG)** dan **Local Binary Pattern (LBP)**
- Analisis komparatif antar model machine learning
- Visualisasi distribusi data dan hasil prediksi
- Preprocessing data menggunakan **SMOTE** untuk menangani imbalanced class
- Normalisasi fitur menggunakan **MinMaxScaler** dan **StandardScaler**

## Struktur Proyek

```
KA/
├── Datasets/
│   ├── train/
│   │   ├── NORMAL/
│   │   └── PNEUMONIA/
│   ├── val/
│   │   ├── NORMAL/
│   │   └── PNEUMONIA/
│   └── test/
│       ├── NORMAL/
│       └── PNEUMONIA/
├── [KA]_PROYEK_PNEUNOMIA_ASLI.ipynb
├── Video Presentasi Project.mp4
├── Presentasi Project.pptx
├── Laporan Project.docx
├── README.md
└── LICENSE
```

## Dataset

Dataset yang digunakan dalam proyek ini adalah citra X-Ray paru-paru dengan dua kelas:
- **NORMAL**: Citra paru-paru sehat
- **PNEUMONIA**: Citra paru-paru dengan pneumonia

### Distribusi Dataset:
| Split | NORMAL | PNEUMONIA |
|-------|--------|-----------|
| Train | 1,341  | 3,875     |
| Val   | 8      | 8         |
| Test  | 234    | 390       |

## Teknologi & Library

- **Python 3.x**
- **Matplotlib** & **Seaborn** - Visualisasi data
- **NumPy** & **Pandas** - Manipulasi data
- **scikit-learn** - Preprocessing dan model Machine Learning
- **XGBoost** - Gradient Boosting Classifier
- **imbalanced-learn (SMOTE)** - Oversampling untuk data tidak seimbang

## Cara Penggunaan

1. **Clone Repository**
   ```bash
   git clone https://github.com/alfathir27/ka-final-project
   cd KA
   ```

2. **Install Dependencies**
   ```bash
   pip install matplotlib seaborn numpy pandas scikit-learn xgboost imbalanced-learn joblib
   ```

3. **Jalankan Notebook**
   - Buka file `[KA]_PROYEK_PNEUNOMIA_ASLI.ipynb` menggunakan Jupyter Notebook atau Google Colab
   - Ikuti langkah-langkah dalam notebook untuk melakukan training dan evaluasi model

## Tim Pengembang

**Dosen Pengampu:**
- Kartika Chandra Dewi, S.Si., M.Si.

**Anggota Kelompok:**
- Muhammad Habib Nur Aiman (24031554152)
- Rabbani Yuki Arfiansyach (24031554131)
- M. Habiburrohman Al-Fathir (24031554145)
- Frendy Zahril Ramadhani (24031554187)

## Lisensi

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail.

## Acknowledgements

- Dataset X-Ray paru-paru yang digunakan dalam proyek ini
- Komunitas open-source untuk library dan framework yang digunakan
- Universitas dan dosen pembimbing atas dukungan dan bimbingannya
