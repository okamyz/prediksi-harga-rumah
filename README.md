# Prediksi Harga Rumah Jakarta Selatan

Project data science pertama saya: memprediksi harga rumah di Jakarta Selatan
dari luas tanah, luas bangunan, jumlah kamar, dan kapasitas garasi.

## Dataset
Daftar Harga Rumah (Kaggle, wisnuanggara), sekitar 1.000 data listing.
Sumber: https://www.kaggle.com/datasets/wisnuanggara/daftar-harga-rumah 

## Langkah yang dikerjakan
1. Data cleaning (menghapus duplikat dan data harga janggal)
2. Exploratory Data Analysis
3. Pemodelan: Linear Regression dan Random Forest
4. Evaluasi dengan MAE, R², dan 5-fold cross-validation

## Hasil
| Model | MAE (miliar Rp) | R² |
|---|---|---|
| Tebakan rata-rata | 5,42 | -0,01 |
| Linear Regression | 2,35 | 0,74 |
| Random Forest | 1,73 | 0,83 |

Luas tanah adalah faktor paling berpengaruh terhadap harga (±77%).

## Keterbatasan
Data hanya sekitar seribu baris dan didominasi kawasan Tebet, sehingga model
kurang akurat untuk rumah berharga sangat tinggi.

## Cara menjalankan
pip install -r requirements.txt
Lalu buka notebooks/01_harga_rumah.ipynb