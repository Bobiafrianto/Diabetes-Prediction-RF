# Proyek Klasifikasi Diabetes dengan Random Forest

Proyek ini bertujuan untuk membangun model machine learning menggunakan algoritma **Random Forest** untuk mengkalisifikasikan diabetes atau tidak diabetes berdasarkan data diagnostik.

### Bahasa & Environment
![Python](https://img.shields.io/badge/Python-3.13.1-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter&logoColor=white)

### Tools & Library
![Pandas](https://img.shields.io/badge/Pandas-2.2.2-teal?logo=pandas&logoColor=white)
![Numpy](https://img.shields.io/badge/Numpy-2.0.0-purple?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.9.2-red?logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13.2-lightblue?logo=plotly&logoColor=white)
![ImbalancedLearn](https://img.shields.io/badge/Imbalanced--Learn-0.12.3-yellow?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.5.0-green?logo=scikitlearn&logoColor=white)
![Joblib](https://img.shields.io/badge/Joblib-1.4.2-darkblue?logo=python&logoColor=white)


### Model
![RandomForest](https://img.shields.io/badge/Model-RandomForest-yellowgreen)


---

## Deskripsi Proyek

Dalam proyek ini, saya melakukan beberapa langkah penting untuk memastikan kualitas data dan performa model. Pertama, saya mengecek fitur-fitur yang seharusnya tidak bernilai *NaN*. Hasil pengecekan menunjukkan bahwa memang tidak ada nilai *NaN*, namun terdapat nilai `0` pada fitur tertentu yang tidak valid secara medis. Untuk mengatasi hal ini, nilai `0` pada masing-masing fitur tersebut saya ganti dengan nilai median dari fitur yang bersangkutan. Setelah data dibersihkan, saya melakukan pemeriksaan keseimbangan kelas pada variabel target `Outcome` dan menemukan adanya ketidakseimbangan, di mana jumlah data pasien tidak diabetes jauh lebih banyak dibandingkan pasien dengan diabetes. Agar model tidak bias terhadap kelas mayoritas, saya menerapkan teknik **SMOTE (Synthetic Minority Oversampling Technique)** yang menghasilkan data tambahan untuk kelas minoritas sehingga distribusi kelas menjadi lebih seimbang. Dengan data yang telah bersih dan seimbang, saya kemudian membangun dan melatih model **Random Forest Classifier** untuk melakukan prediksi terhadap kemungkinan seorang pasien menderita diabetes.
