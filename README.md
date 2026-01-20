\# Prediksi Harga Rumah Menggunakan KNN



\## Deskripsi

Proyek ini berisi implementasi Machine Learning regresi untuk memprediksi harga rumah berdasarkan beberapa karakteristik fisik dan lokasi.  

Model dibangun menggunakan algoritma K-Nearest Neighbors (KNN) dengan Python dan scikit-learn.



Tujuan utama proyek ini adalah untuk memahami penerapan KNN pada kasus regresi, termasuk preprocessing data dan evaluasi performa model.



---



\## Dataset

Dataset berisi data rumah di beberapa wilayah dengan fitur berikut:

\- `lokasi` – Lokasi rumah (contoh: Jember, Banyuwangi)

\- `luas_tanah_m2` – Luas tanah (m²)

\- `luas_bangunan_m2` – Luas bangunan (m²)

\- `jumlah_kamar` – Jumlah kamar

\- `jarak_ke_pusat_kota_km` – Jarak ke pusat kota (km)

\- `usia_bangunan_tahun` – Usia bangunan (tahun)

\- `harga_rumah_juta` – Harga rumah (dalam juta rupiah)



---



\## Alur Pengerjaan

1\. Membaca dan meninjau dataset

2\. Memisahkan fitur dan target

3\. Encoding data kategorikal (`lokasi`)

4\. Membagi data menjadi data latih dan data uji

5\. Melatih model KNN Regressor

6\. Evaluasi model tanpa scaling

7\. Standardisasi fitur menggunakan `StandardScaler`

8\. Evaluasi ulang model setelah scaling



---



\## Model

\- Algoritma: K-Nearest Neighbors Regressor

\- Jumlah tetangga (`k`) = 3

\- Pembagian data: 70% data latih, 30% data uji



---



\## Evaluasi

Model dievaluasi menggunakan:

\- R-Squared (R²)

\- Mean Absolute Error (MAE)

\- Mean Squared Error (MSE)



\### Hasil

\- Tanpa scaling: performa model masih kurang optimal

\- Dengan scaling: performa meningkat secara signifikan  

&nbsp; - R² mencapai sekitar 0.77

&nbsp; - Error prediksi (MAE dan MSE) menjadi lebih kecil



Hal ini menunjukkan bahwa standardisasi fitur sangat berpengaruh pada performa KNN.



---



\## Tools \& Library

\- Python

\- Jupyter Notebook

\- Pandas

\- NumPy

\- Scikit-learn



---



\## Struktur Folder

Prediksi-Harga-Rumah-KNN/

├── Prediksi_Harga_Rumah_Menggunakan_KNN.ipynb

├── data_harga_rumah_bwi_jbr.csv

└── README.md



---



\## Catatan Pengembangan

Beberapa pengembangan yang dapat dilakukan:

\- Mencoba nilai `k` yang berbeda

\- Menambahkan validasi silang

\- Mencoba algoritma regresi lain (Linear Regression, Random Forest)

\- Visualisasi perbandingan harga asli dan prediksi

