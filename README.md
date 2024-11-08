# House Price Prediction

Repository ini berisi implementasi model prediksi harga rumah menggunakan algoritma Regresi Linear. Model ini memprediksi harga rumah berdasarkan fitur Ukuran Rumah (sqft) yang terdapat dalam dataset.

## Latar Belakang

Kenaikan harga properti sering menjadi perhatian, baik bagi individu maupun investor. Menggunakan algoritma regresi linear, model ini mencoba menemukan pola dalam data historis yang dapat membantu memprediksi harga rumah berdasarkan ukuran. Model ini diharapkan dapat memberikan prediksi yang mendekati akurat dengan memperhitungkan ukuran sebagai fitur utama.

## Teknologi yang Digunakan

- Python: Bahasa pemrograman yang digunakan untuk implementasi
- NumPy: Library untuk komputasi ilmiah
- Pandas: Library untuk manipulasi data
- scikit-learn: Library untuk algoritma pembelajaran mesin
- Matplotlib: Library untuk visualisasi data

## Fitur

1. Eksplorasi Data: Visualisasi data menggunakan scatter plot untuk melihat hubungan antara ukuran rumah dan harga.
2. Pembagian Data: Data dipecah menjadi data pelatihan dan pengujian untuk mengevaluasi performa model.
3. Pembuatan Model: Menggunakan regresi linear untuk membuat model prediksi.
4. Evaluasi Model: Mengukur performa model menggunakan Mean Squared Error (MSE) dan R^2 Score.
5. Prediksi Harga: Fitur untuk memprediksi harga rumah berdasarkan ukuran yang ditentukan pengguna.

## Instalasi

1. Clone repository ini:
  ```bash
    git clone https://github.com/username/house-price-prediction.git
  ```

2. Install dependensi yang diperlukan:
```bash
    pip install -r requirements.txt
```

## Cara Penggunaan

1. Pastikan file CSV dataset (_Synthetic House pricing dataset - Sheet1.csv) ada dalam folder yang sama dengan script.
2. Jalankan script untuk melatih dan menguji model:
```bash
  python main.py
```
3. Prediksi harga untuk ukuran rumah tertentu dapat dilakukan dengan memanggil fungsi predict_house_price(size) pada akhir script.

## Struktur Project

```bash
house-price-prediction/
├── _Synthetic House pricing dataset - Sheet1.csv  # Dataset harga rumah
├── main.py                                       # Script utama untuk menjalankan model
└── README.md                                     # Dokumentasi repository
```

## Contoh Penggunaan

Untuk memprediksi harga rumah dengan ukuran tertentu, bisa memanfaatkan fungsi predict_house_price. Contohnya, untuk rumah berukuran 1800 sqft:
```bash
print("Prediksi harga untuk rumah berukuran 1800 sqft:", predict_house_price(1800))
```

## Hasil Evaluasi

Model ini dievaluasi menggunakan Mean Squared Error (MSE) dan R^2 Score:
- MSE: Mengukur rata-rata kuadrat kesalahan antara nilai prediksi dan nilai sebenarnya.
- R^2 Score: Mengukur seberapa baik model menjelaskan variabilitas data.
