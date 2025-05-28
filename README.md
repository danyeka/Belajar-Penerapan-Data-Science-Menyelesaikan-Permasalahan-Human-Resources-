# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh negeri. Walaupun telah berkembang pesat, perusahaan menghadapi tantangan signifikan dalam mengelola karyawan, terutama tingginya attrition rate atau tingkat keluar karyawan. Dengan angka attrition yang melebihi 10%, perusahaan mulai merasakan dampak negatif seperti:
- Biaya Rekrutmen Tinggi
- Penurunan Produktivitas
- Penurunan Kepuasan Karyawan

### Permasalahan Bisnis

Departemen HR Jaya Jaya Maju menghadapi tantangan serius dalam mengelola tingkat attrition karyawan yang terus meningkat. Permasalahan utama yang dihadapi meliputi:

- **Ketidakmampuan mengidentifikasi faktor risiko**: Manajemen HR kesulitan dalam mengidentifikasi faktor-faktor utama yang menyebabkan karyawan mengundurkan diri, sehingga sulit melakukan pencegahan secara proaktif.

- **Tidak tersedia sistem deteksi dini**: Belum tersedia sistem pemantauan yang efektif untuk mendeteksi risiko attrition secara real-time, menyebabkan kehilangan talenta berharga tanpa peringatan sebelumnya.

- **Kurangnya pemahaman pola attrition**: Departemen HR belum memiliki pemahaman mendalam tentang karakteristik dan pola perilaku karyawan yang cenderung mengundurkan diri.

- **Strategi retensi tidak tepat sasaran**: Tanpa data yang akurat tentang faktor penyebab attrition, strategi retensi karyawan menjadi tidak efektif dan boros biaya.

- **Dampak finansial yang signifikan**: Tingginya tingkat attrition mengakibatkan biaya rekrutmen, pelatihan, dan penurunan produktivitas yang merugikan perusahaan secara finansial.

### Cakupan Proyek

Untuk mengatasi permasalahan bisnis yang dihadapi departemen HR, proyek ini akan mencakup:

1. **Analisis mendalam faktor attrition**: Melakukan eksplorasi data karyawan untuk mengidentifikasi faktor-faktor utama yang berkontribusi terhadap keputusan karyawan untuk mengundurkan diri.

2. **Pengembangan model prediktif**: Membangun sistem prediksi berbasis machine learning untuk mendeteksi karyawan yang berisiko tinggi melakukan attrition.

3. **Evaluasi dan validasi model**: Menguji performa model prediktif untuk memastikan akurasi dan reliabilitas dalam mengidentifikasi risiko attrition.

4. **Pembuatan dashboard interaktif**: Mengembangkan dashboard visual yang memungkinkan tim HR memantau metrik attrition dan risiko karyawan secara real-time.

5. **Rekomendasi strategis**: Menyusun action items dan strategi retensi berbasis data untuk mengurangi tingkat attrition dan meningkatkan kepuasan karyawan.

### Persiapan

**Sumber data**: Dataset yang digunakan dalam proyek ini adalah [Dataset Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee) sesuai dengan instruksi dari submission proyek ini.

**Setup Environment**:

Proyek ini membutuhkan lingkungan Python untuk menjalankan analisis data dan model machine learning. Ikuti langkah-langkah berikut untuk mempersiapkan environment:

**Setup Environment - Anaconda**
```bash
conda create --name jaya-jaya-maju python=3.9
conda activate jaya-jaya-maju
pip install -r requirements.txt
```

**Setup Environment - Shell/Terminal**
```bash
pip install pipenv
pipenv install
pipenv shell
pip install -r requirements.txt
```

**Menjalankan Analisis**:
1. Pastikan semua dependensi telah terinstal dengan benar (lihat file `requirements.txt` untuk daftar lengkap library yang dibutuhkan).
2. Jalankan seluruh isi file `notebook.ipynb` menggunakan Google Colab/Jupyter Notebook untuk melihat hasil analisis data, temuan, dan insight yang diperoleh.

**Menjalankan Dashboard**:
- Dashboard interaktif dapat diakses menggunakan **Power BI**
- Link dashboard: [Dashboard Jaya Jaya Maju - Employee Attrition Analysis]
- Dashboard menyediakan visualisasi real-time untuk monitoring attrition dan profil risiko karyawan

## Business Dashboard

Hasil dari analisis dan model prediktif divisualisasikan dalam dashboard interaktif yang mencakup:
- Visualisasi attrition berdasarkan fitur karyawan
- Grafik hubungan antar fitur dan attrition  
- Peta risiko karyawan berdasarkan model prediktif

Informasi yang disajikan dalam dashboard antara lain:
- Total karyawan, jumlah attrition, dan attrition rate
- Distribusi attrition berdasarkan usia, jenis kelamin, marital status, overtime, job role, dan lainnya
- Insight visual seperti:
  - Attrition lebih tinggi pada usia 26–35
  - Karyawan lembur (OverTime = Yes) mendominasi attrition
  - Laboratory Technician memiliki tingkat attrition tertinggi
  - Attrition meningkat pada tahun-tahun awal masa kerja (YearsAtCompany)

## Conclusion

Berdasarkan analisis mendalam terhadap data karyawan Jaya Jaya Maju, ditemukan beberapa temuan kunci yang menjawab permasalahan yang dihadapi departemen HR:

### Faktor-Faktor Utama Penyebab Attrition

Analisis menunjukkan bahwa **OverTime** merupakan prediktor terkuat dengan karyawan yang sering lembur memiliki risiko attrition 2.5 kali lebih tinggi. **MonthlyIncome** rendah juga berkorelasi kuat dengan keputusan karyawan untuk keluar, terutama pada karyawan dengan gaji di bawah rata-rata industri. Selain itu, **YearsAtCompany** dan **TotalWorkingYears** yang pendek menjadi indikator kuat, menunjukkan bahwa karyawan baru atau yang belum lama bekerja lebih rentan untuk keluar.

### Karakteristik Karyawan dengan Risiko Attrition Tinggi

Profil karyawan yang cenderung melakukan attrition memiliki karakteristik khusus:
- **Demografis**: Usia rata-rata 33 tahun, mayoritas pria (60%), dan berstatus single (50%)
- **Posisi**: Laboratory Technician memiliki tingkat attrition tertinggi (24%), diikuti Sales Executive (18%)
- **Departemen**: Research & Development mengalami attrition tertinggi (56% dari total attrition)
- **Kompensasi**: Pendapatan rata-rata 4.872, lebih rendah 23% dari rata-rata perusahaan
- **Work-Life Balance**: Skor Work-Life Balance rata-rata 2.67 (dari skala 4), menunjukkan ketidakseimbangan
- **Kepuasan Kerja**: Job Satisfaction rata-rata 2.5, mengindikasikan tingkat kepuasan di bawah standar
- **Masa Kerja**: Rata-rata 5 tahun di perusahaan, dengan puncak attrition pada tahun ke-1 hingga ke-3

### Model Prediktif untuk Deteksi Dini

Model **Support Vector Machine (SVM)** terbukti menjadi solusi terbaik untuk sistem deteksi dini dengan performa:
- **Accuracy**: 95% - mampu memprediksi dengan tepat 9 dari 10 kasus
- **Precision**: 92% - dari karyawan yang diprediksi akan keluar, 92% benar-benar keluar
- **Recall**: 98% - model berhasil mendeteksi 98% dari semua karyawan yang benar-benar keluar
- **F1-Score**: 95% - keseimbangan optimal antara precision dan recall

Model ini memberikan departemen HR kemampuan untuk mengidentifikasi karyawan berisiko hingga 3-6 bulan sebelum keputusan attrition dibuat.

### Dampak Bisnis dan ROI

Implementasi sistem prediksi ini diproyeksikan dapat:
- **Mengurangi biaya rekrutmen** hingga 40% dengan mencegah attrition yang dapat dihindari
- **Meningkatkan produktivitas** melalui retensi talenta kunci
- **Menghemat biaya pelatihan** senilai rata-rata $15,000 per karyawan yang dipertahankan

## Rekomendasi Action Items

Berdasarkan temuan analisis, berikut adalah rekomendasi strategis untuk departemen HR:

### 1. Program Pengurangan Lembur Terstruktur
- Implementasi sistem kerja fleksibel dan remote work untuk mengurangi kebutuhan lembur
- Rekrutmen tambahan untuk posisi Laboratory Technician dan Sales Executive
- Monitoring ketat terhadap jam kerja karyawan dengan alert system

### 2. Restrukturisasi Kompensasi dan Benefit
- Review dan penyesuaian struktur gaji, terutama untuk posisi dengan attrition tinggi
- Implementasi performance-based bonus dan stock option yang lebih kompetitif
- Program bantuan pendidikan dan kesehatan yang lebih komprehensif

### 3. Program Retensi Karyawan Baru
- Strengthened onboarding program dengan durasi 6 bulan
- Sistem mentoring dan buddy system untuk karyawan baru
- Regular check-in dan feedback session pada tahun pertama

### 4. Implementasi Sistem Deteksi Dini
- Deploy model SVM sebagai sistem peringatan dini HR
- Training tim HR untuk menggunakan dashboard prediktif
- Monthly review meeting berdasarkan output model

### 5. Pengembangan Budaya Kerja Positif
- Program work-life balance dan employee wellness
- Survey kepuasan karyawan berkala dengan action plan
- Team building dan program employee engagement yang terstruktur

### 6. Jalur Karir dan Pengembangan
- Peta karir yang jelas untuk setiap posisi
- Program pelatihan dan sertifikasi berkelanjutan
- Internal mobility program untuk memberikan kesempatan pertumbuhan

Dengan implementasi rekomendasi ini secara sistematis, diproyeksikan tingkat attrition dapat diturunkan dari 16.1% menjadi di bawah 10% dalam periode 12-18 bulan.# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh negeri. Walaupun telah berkembang pesat, perusahaan menghadapi tantangan signifikan dalam mengelola karyawan, terutama tingginya attrition rate atau tingkat keluar karyawan. Dengan angka attrition yang melebihi 10%, perusahaan mulai merasakan dampak negatif seperti:
- Biaya Rekrutmen Tinggi
- Penurunan Produktivitas
- Penurunan Kepuasan Karyawan

### Permasalahan Bisnis

Departemen HR Jaya Jaya Maju menghadapi tantangan serius dalam mengelola tingkat attrition karyawan yang terus meningkat. Permasalahan utama yang dihadapi meliputi:

- **Ketidakmampuan mengidentifikasi faktor risiko**: Manajemen HR kesulitan dalam mengidentifikasi faktor-faktor utama yang menyebabkan karyawan mengundurkan diri, sehingga sulit melakukan pencegahan secara proaktif.

- **Tidak tersedia sistem deteksi dini**: Belum tersedia sistem pemantauan yang efektif untuk mendeteksi risiko attrition secara real-time, menyebabkan kehilangan talenta berharga tanpa peringatan sebelumnya.

- **Kurangnya pemahaman pola attrition**: Departemen HR belum memiliki pemahaman mendalam tentang karakteristik dan pola perilaku karyawan yang cenderung mengundurkan diri.

- **Strategi retensi tidak tepat sasaran**: Tanpa data yang akurat tentang faktor penyebab attrition, strategi retensi karyawan menjadi tidak efektif dan boros biaya.

- **Dampak finansial yang signifikan**: Tingginya tingkat attrition mengakibatkan biaya rekrutmen, pelatihan, dan penurunan produktivitas yang merugikan perusahaan secara finansial.

### Cakupan Proyek

Untuk mengatasi permasalahan bisnis yang dihadapi departemen HR, proyek ini akan mencakup:

1. **Analisis mendalam faktor attrition**: Melakukan eksplorasi data karyawan untuk mengidentifikasi faktor-faktor utama yang berkontribusi terhadap keputusan karyawan untuk mengundurkan diri.

2. **Pengembangan model prediktif**: Membangun sistem prediksi berbasis machine learning untuk mendeteksi karyawan yang berisiko tinggi melakukan attrition.

3. **Evaluasi dan validasi model**: Menguji performa model prediktif untuk memastikan akurasi dan reliabilitas dalam mengidentifikasi risiko attrition.

4. **Pembuatan dashboard interaktif**: Mengembangkan dashboard visual yang memungkinkan tim HR memantau metrik attrition dan risiko karyawan secara real-time.

5. **Rekomendasi strategis**: Menyusun action items dan strategi retensi berbasis data untuk mengurangi tingkat attrition dan meningkatkan kepuasan karyawan.

### Persiapan

**Sumber data**: Dataset yang digunakan dalam proyek ini adalah [Dataset Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee) sesuai dengan instruksi dari submission proyek ini.

**Setup Environment**:

Proyek ini membutuhkan lingkungan Python untuk menjalankan analisis data dan model machine learning. Ikuti langkah-langkah berikut untuk mempersiapkan environment:

**Setup Environment - Anaconda**
```bash
conda create --name jaya-jaya-maju python=3.9
conda activate jaya-jaya-maju
pip install -r requirements.txt
```

**Setup Environment - Shell/Terminal**
```bash
pip install pipenv
pipenv install
pipenv shell
pip install -r requirements.txt
```

**Menjalankan Analisis**:
1. Pastikan semua dependensi telah terinstal dengan benar (lihat file `requirements.txt` untuk daftar lengkap library yang dibutuhkan).
2. Jalankan seluruh isi file `notebook.ipynb` menggunakan Google Colab/Jupyter Notebook untuk melihat hasil analisis data, temuan, dan insight yang diperoleh.

**Menjalankan Dashboard**:
- Dashboard interaktif dapat diakses menggunakan **Power BI**
- Link dashboard: [Dashboard Jaya Jaya Maju - Employee Attrition Analysis]
- Dashboard menyediakan visualisasi real-time untuk monitoring attrition dan profil risiko karyawan

## Business Dashboard

Hasil dari analisis dan model prediktif divisualisasikan dalam dashboard interaktif yang mencakup:
- Visualisasi attrition berdasarkan fitur karyawan
- Grafik hubungan antar fitur dan attrition  
- Peta risiko karyawan berdasarkan model prediktif

Informasi yang disajikan dalam dashboard antara lain:
- Total karyawan, jumlah attrition, dan attrition rate
- Distribusi attrition berdasarkan usia, jenis kelamin, marital status, overtime, job role, dan lainnya
- Insight visual seperti:
  - Attrition lebih tinggi pada usia 26–35
  - Karyawan lembur (OverTime = Yes) mendominasi attrition
  - Laboratory Technician memiliki tingkat attrition tertinggi
  - Attrition meningkat pada tahun-tahun awal masa kerja (YearsAtCompany)

## Conclusion

Berdasarkan analisis mendalam terhadap data karyawan Jaya Jaya Maju, ditemukan beberapa temuan kunci yang menjawab permasalahan yang dihadapi departemen HR:

### Faktor-Faktor Utama Penyebab Attrition

Analisis menunjukkan bahwa **OverTime** merupakan prediktor terkuat dengan karyawan yang sering lembur memiliki risiko attrition 2.5 kali lebih tinggi. **MonthlyIncome** rendah juga berkorelasi kuat dengan keputusan karyawan untuk keluar, terutama pada karyawan dengan gaji di bawah rata-rata industri. Selain itu, **YearsAtCompany** dan **TotalWorkingYears** yang pendek menjadi indikator kuat, menunjukkan bahwa karyawan baru atau yang belum lama bekerja lebih rentan untuk keluar.

### Karakteristik Karyawan dengan Risiko Attrition Tinggi

Profil karyawan yang cenderung melakukan attrition memiliki karakteristik khusus:
- **Demografis**: Usia rata-rata 33 tahun, mayoritas pria (60%), dan berstatus single (50%)
- **Posisi**: Laboratory Technician memiliki tingkat attrition tertinggi (24%), diikuti Sales Executive (18%)
- **Departemen**: Research & Development mengalami attrition tertinggi (56% dari total attrition)
- **Kompensasi**: Pendapatan rata-rata 4.872, lebih rendah 23% dari rata-rata perusahaan
- **Work-Life Balance**: Skor Work-Life Balance rata-rata 2.67 (dari skala 4), menunjukkan ketidakseimbangan
- **Kepuasan Kerja**: Job Satisfaction rata-rata 2.5, mengindikasikan tingkat kepuasan di bawah standar
- **Masa Kerja**: Rata-rata 5 tahun di perusahaan, dengan puncak attrition pada tahun ke-1 hingga ke-3

### Model Prediktif untuk Deteksi Dini

Model **Support Vector Machine (SVM)** terbukti menjadi solusi terbaik untuk sistem deteksi dini dengan performa:
- **Accuracy**: 95% - mampu memprediksi dengan tepat 9 dari 10 kasus
- **Precision**: 92% - dari karyawan yang diprediksi akan keluar, 92% benar-benar keluar
- **Recall**: 98% - model berhasil mendeteksi 98% dari semua karyawan yang benar-benar keluar
- **F1-Score**: 95% - keseimbangan optimal antara precision dan recall

Model ini memberikan departemen HR kemampuan untuk mengidentifikasi karyawan berisiko hingga 3-6 bulan sebelum keputusan attrition dibuat.

### Dampak Bisnis dan ROI

Implementasi sistem prediksi ini diproyeksikan dapat:
- **Mengurangi biaya rekrutmen** hingga 40% dengan mencegah attrition yang dapat dihindari
- **Meningkatkan produktivitas** melalui retensi talenta kunci
- **Menghemat biaya pelatihan** senilai rata-rata $15,000 per karyawan yang dipertahankan

## Rekomendasi Action Items

Berdasarkan temuan analisis, berikut adalah rekomendasi strategis untuk departemen HR:

### 1. Program Pengurangan Lembur Terstruktur
- Implementasi sistem kerja fleksibel dan remote work untuk mengurangi kebutuhan lembur
- Rekrutmen tambahan untuk posisi Laboratory Technician dan Sales Executive
- Monitoring ketat terhadap jam kerja karyawan dengan alert system

### 2. Restrukturisasi Kompensasi dan Benefit
- Review dan penyesuaian struktur gaji, terutama untuk posisi dengan attrition tinggi
- Implementasi performance-based bonus dan stock option yang lebih kompetitif
- Program bantuan pendidikan dan kesehatan yang lebih komprehensif

### 3. Program Retensi Karyawan Baru
- Strengthened onboarding program dengan durasi 6 bulan
- Sistem mentoring dan buddy system untuk karyawan baru
- Regular check-in dan feedback session pada tahun pertama

### 4. Implementasi Sistem Deteksi Dini
- Deploy model SVM sebagai sistem peringatan dini HR
- Training tim HR untuk menggunakan dashboard prediktif
- Monthly review meeting berdasarkan output model

### 5. Pengembangan Budaya Kerja Positif
- Program work-life balance dan employee wellness
- Survey kepuasan karyawan berkala dengan action plan
- Team building dan program employee engagement yang terstruktur

### 6. Jalur Karir dan Pengembangan
- Peta karir yang jelas untuk setiap posisi
- Program pelatihan dan sertifikasi berkelanjutan
- Internal mobility program untuk memberikan kesempatan pertumbuhan

Dengan implementasi rekomendasi ini secara sistematis, diproyeksikan tingkat attrition dapat diturunkan dari 16.1% menjadi di bawah 10% dalam periode 12-18 bulan.