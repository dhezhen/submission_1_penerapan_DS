# Submission #1 Penerapan Data Analisi

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh negeri. Walaupun telah berkembang pesat, perusahaan menghadapi tantangan signifikan dalam mengelola karyawan, terutama tingginya **attrition rate** atau tingkat keluar karyawan. Dengan angka attrition yang melebihi **10%**, perusahaan mulai merasakan dampak negatif seperti:
- **Biaya Rekrutmen Tinggi**: Berdasarkan karakteristik perusahaan yang memiliki lebih dari 1.000 karyawan, biaya yang dikeluarkan untuk proses rekrutmen dan pelatihan karyawan baru meningkat seiring tingginya angka pergantian karyawan. Hal ini mencakup biaya iklan lowongan kerja, seleksi, onboarding, dan pelatihan.
- **Penurunan Produktivitas**: Tingginya pergantian karyawan menyebabkan hilangnya pengalaman dan keterampilan yang dibutuhkan untuk mencapai target bisnis. Data dalam dataset seperti **YearsAtCompany** dan **YearsWithCurrManager** dapat membantu mengukur kontribusi pengalaman terhadap produktivitas.
- **Penurunan Kepuasan Karyawan**: Indikator kepuasan seperti **Job Satisfaction**, **Work-Life Balance**, dan **Environment Satisfaction** dalam dataset menunjukkan pentingnya mengidentifikasi ketidakpuasan lebih awal untuk mencegah gelombang keluar karyawan.

Manajemen HR di Jaya Jaya Maju menyadari pentingnya memahami faktor-faktor penyebab attrition agar dapat menyusun strategi yang tepat untuk **meningkatkan retensi karyawan** dan **mengurangi attrition rate** secara signifikan.

### Permasalahan Bisnis
Permasalahan bisnis yang akan diselesaikan melalui proyek ini adalah:
1. **Mengidentifikasi faktor-faktor utama yang mempengaruhi attrition rate** di perusahaan, baik dari segi demografis, kepuasan kerja, maupun metrik finansial.
2. **Mengukur tingkat kepuasan karyawan** berdasarkan parameter seperti **Job Satisfaction**, **Work-Life Balance**, dan **Environment Satisfaction**.
3. **Menentukan pola perilaku karyawan yang cenderung keluar**, seperti pengaruh jarak rumah ke kantor, lembur berlebihan (OverTime), dan pendapatan karyawan.
4. **Menyediakan alat bantu berupa business dashboard** yang memudahkan manajemen HR memantau dan menganalisis faktor-faktor penyebab attrition secara berkala.

Dengan menyelesaikan permasalahan ini, perusahaan diharapkan dapat:
- Mengurangi **attrition rate** dengan mengambil langkah pencegahan yang tepat.
- Menyusun program retensi yang lebih efektif.
- Meningkatkan kepuasan kerja dan produktivitas karyawan.

### Cakupan Proyek
Proyek ini mencakup:
1. **Eksplorasi dan Pemahaman Data**: Analisis dataset `employee_data.csv` untuk memahami karakteristik karyawan dan distribusi attrition.
2. **Data Preparation**: Membersihkan dan memproses data agar siap digunakan untuk analisis lebih lanjut.
3. **Analisis Faktor Penyebab Attrition**:
   - Analisis korelasi antara variabel seperti pendapatan, lembur, tingkat kepuasan, dan jarak rumah.
   - Visualisasi tren dan pola attrition di berbagai departemen, level pekerjaan, dan usia karyawan.
4. **Pembuatan Business Dashboard**: Visualisasi data dalam bentuk dashboard yang mudah dipahami untuk memantau faktor penyebab attrition.
5. **Kesimpulan dan Rekomendasi**: Menarik kesimpulan dari hasil analisis dan memberikan rekomendasi praktis untuk mengurangi attrition.

### Persiapan
**Sumber data**: Dataset yang digunakan dalam proyek ini adalah [Dataset Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee) sesuai dengan instruksi dari submission proyek ini.
**Setup environment**:
1. setup environment - Anaconda
```
conda create --name data_analisys python=3.10
conda activate data_analisys
pip install -r requirements.txt
```
2. setup environment - Shell/terminal
```
pip install pipenv
pipenv install
pipenv shell
pip install -r requirements.txt
```

4. setup environment - Notebook Google Collab (jika menggunakan google colab)
- Pastikan semua dependensi, paket, dan pustaka yang diperlukan telah tersedia (terdapat file requirements.txt).
- Kemudian, jalankan seluruh sel dalam file submission_1.ipynb menggunakan Google Colab atau Jupyter Notebook untuk menampilkan hasil analisis data, temuan yang diidentifikasi, serta insight yang diperoleh
2.  Menjalankan Dashboard
- untuk menjalankan dashboard, silakan klik

Proyek ini membutuhkan lingkungan sederhana untuk menjalankan analisis data dan dashboard. Berikut langkah-langkah untuk mempersiapkan environment:
1. Menjalankan `notebook.ipynb`
   - Pastikan dependensi, packages, library yang dibutuhkan sudah tersedia (lihat file `requirements.txt` untuk melihat dependensi yang dibutuhkan).
   - Jalankan seluruh isi file `notebook.ipynb` menggunakan Google Colab/Jupyter Notebook untuk melihat hasil analisis data, temuan, dan insight yang diperoleh.
2. **Dashboard Analisis**:
   - Dashboard dibangun dengan menggunakan google looker studio dan bisa Anda lihat pada link berikut ini: 
    https://lookerstudio.google.com/reporting/3a8e7744-09f3-4893-88a5-032d876c26ea/page/OpsKF



## Business Dashboard
Hasil dari analisis dan model prediktif dapat divisualisasikan dalam bentuk dashboard untuk membantu tim HR memantau dan memahami attrition secara real-time. Berikut adalah elemen-elemen yang dapat disertakan dalam dashboard:
1. **Tren Attrition**:
   - Distribusi attrition berdasarkan fitur seperti **OverTime**, **MonthlyIncome**, dan **YearsAtCompany**.
2. **Feature Importance**:
   - Visualisasi kontribusi fitur utama seperti **OverTime_Yes** dan **MonthlyIncome** terhadap risiko attrition.

3. **Model tertinggi**:
   - Berdasarkan hasil dari pengujian dengan 4 algoritma yang berbeda Random Forest memiliki tingkat akurasi tertinggi yaitu 95.5%
   .


## Conclusion
Proyek ini berhasil mencapai tujuan utama yaitu:
1. **Mengidentifikasi faktor utama penyebab attrition**:
   - Faktor terpenting adalah lembur berlebihan (**OverTime**), pendapatan rendah (**MonthlyIncome**), dan masa kerja pendek.
2. **Membangun model prediktif yang akurat**:
   - Model Random Forest memberikan performa terbaik dengan **accuracy 95.55%** dan metrik lainnya yang tinggi.
3. **Memberikan rekomendasi actionable**:
   - Tim HR dapat mengimplementasikan kebijakan untuk mengurangi lembur, menyesuaikan skala gaji, dan memperkuat retensi karyawan baru.

### Rekomendasi Action Items untuk Perusahaan
Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.
1. **Kurangi Lembur Berlebihan**:
   - Berikan program kerja fleksibel untuk meningkatkan keseimbangan kerja-hidup.
2. **Kaji Skala Gaji**:
   - Sesuaikan gaji karyawan agar kompetitif di pasar dan berikan insentif tambahan.
3. **Perkuat Retensi Karyawan Baru**:
   - Implementasikan program onboarding dan mentoring untuk karyawan dengan masa kerja pendek.
