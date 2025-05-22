# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh negeri. Walaupun telah berkembang pesat, perusahaan menghadapi tantangan signifikan dalam mengelola karyawan, terutama tingginya attrition rate atau tingkat keluar karyawan. Dengan angka attrition yang melebihi 10%, perusahaan mulai merasakan dampak negatif seperti:
 - Biaya Rekrutmen Tinggi
 - Penurunan Produktivitas
 - Penurunan Kepuasan Karyawan

### Permasalahan Bisnis

1. Apa saja faktor utama yang menyebabkan attrition karyawan?

2. Bagaimana MonthlyIncome bervariasi di berbagai departemen dan JobRole?

3. Apakah ada korelasi antara YearsAtCompany dan Attrition?

4. Bagaimana distribusi StockOption berdasarkan JobRole?

5. Apa dampak Lembur terhadap kinerja karyawan (PerformanceRating)?

6. Apakah ada pola attrition berdasarkan frekuensi BusinessTravel?

7. Jabatan mana yang memiliki rata-rata YearsAtCompany tertinggi?

8. Apakah ada hubungan antara EducationField dan Pendapatan Bulanan?

9. Bagaimana DistanceFromHome memengaruhi attrition?

10. Bagaimana Usia mempengaruhi attrition?

### Cakupan Proyek

1. Analisis eksploratif terhadap fitur-fitur karyawan.

2. Identifikasi faktor-faktor yang memengaruhi attrition.

3. Membangun model prediktif untuk memprediksi risiko attrition.

4. Evaluasi model

5. Memberikan rekomendasi berbasis data.

### Persiapan
**Sumber data**: Dataset yang digunakan dalam proyek ini adalah [Dataset Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee) sesuai dengan instruksi dari submission proyek ini.
**Setup environment**:
Proyek ini membutuhkan lingkungan sederhana untuk menjalankan analisis data dan dashboard. Berikut langkah-langkah untuk mempersiapkan environment:
1. Menjalankan `notebook.ipynb`
   - Pastikan dependensi, packages, library yang dibutuhkan sudah tersedia (lihat file `requirements.txt` untuk melihat dependensi yang dibutuhkan).
   - Jalankan seluruh isi file `notebook.ipynb` menggunakan Google Colab/Jupyter Notebook untuk melihat hasil analisis data, temuan, dan insight yang diperoleh.
2. **Menjalankan Dashboard**:
   Untuk melihat isi dashboard secara langsung, dapat menggunakan **Power BI** 

## Business Dashboard
Hasil dari analisis dan model prediktif divisualisasikan dalam dashboard interaktif yang mencakup:
 - Visualisasi attrition berdasarkan fitur karyawan.
 - Grafik hubungan antar fitur dan attrition.
 - Peta risiko karyawan berdasarkan model prediktif.

Informasi yang disajikan dalam dashboard antara lain:
 - Total karyawan, jumlah attrition, dan attrition rate.
 - Distribusi attrition berdasarkan usia, jenis kelamin, marital status, overtime, job role, dan lainnya.
 - Insight visual seperti:
   - Attrition lebih tinggi pada usia 26–35.
   - Karyawan lembur (OverTime = Yes) mendominasi attrition.
   - Laboratorium Technician memiliki tingkat attrition tertinggi.
   - Attrition meningkat pada tahun-tahun awal masa kerja (YearsAtCompany).


## Conclusion

Faktor-Faktor Penyebab Attrition
 - OverTime adalah prediktor terkuat — lembur berlebihan meningkatkan risiko attrition.
 - MonthlyIncome rendah berkorelasi dengan tingkat keluar yang lebih tinggi.
 - YearsAtCompany dan TotalWorkingYears yang pendek adalah indikator risiko keluar.
 - DistanceFromHome dan Age juga memiliki kontribusi kecil namun relevan.

## Model Prediktif Terbaik

Model terbaik adalah SVM, dengan performa:
 - Accuracy: 95%
 - Precision: 92%
 - Recall: 98%
 - F1-Score: 95%

SVM menunjukkan performa superior dibanding Logistic Regression dan XGBoost.

## Jawaban terhadap Pertanyaan Bisnis
 - Attrition tinggi terjadi pada karyawan yang lembur, berpendapatan rendah, dan masa kerja pendek.
 - MonthlyIncome bervariasi menurut JobRole, dengan Manager dan Director memiliki gaji lebih tinggi.
 - YearsAtCompany menunjukkan pola non-linear terhadap attrition.
 - StockOption lebih tinggi pada posisi direktur dan manajerial.
 - OverTime tidak memengaruhi PerformanceRating secara signifikan.
 - Frekuensi BusinessTravel tinggi berkorelasi dengan attrition.
 - Manager memiliki rata-rata YearsAtCompany tertinggi.
 - EducationField berpengaruh terhadap pendapatan, terutama HR dan Marketing.
 - DistanceFromHome tidak signifikan terhadap attrition.
 - Usia muda (20–35) lebih rentan terhadap attrition.

## Karakteristik Umum Karyawan yang Melakukan Attrition
 - Usia rata-rata: 33 tahun
 - Jenis kelamin dominan: Pria
 - Status: Mayoritas Single
 - JobRole tertinggi attrition: Laboratory Technician
 - Departemen tertinggi attrition: Research & Development
 - Pendapatan rata-rata: 4,872
 - OverTime: Tinggi
 - JobSatisfaction: 2.5
 - WorkLifeBalance: 2.67
 - YearsAtCompany rata-rata: 5 tahun

## Rekomendasi Action Items
 - Kurangi Lembur: Terapkan sistem kerja fleksibel.
 - Kaji Struktur Gaji: Sesuaikan agar kompetitif.
 - Retensi Karyawan Baru: Onboarding dan mentoring.
 - Bangun Budaya Positif: Lingkungan kerja suportif.
 - Gunakan Model SVM: Untuk sistem peringatan dini HR.
 - Pengembangan Karier: Program pelatihan dan jalur karier jelas.
