# HR Analytics Project with SQL in Jupyter Notebook

Selamat datang di proyek analisis data karyawan berbasis SQL yang dilakukan dalam lingkungan Jupyter Notebook menggunakan SQLite dan SQL Magic. Proyek ini bertujuan untuk membangun portfolio eksploratif dan analitis dari sebuah dataset sumber daya manusia (HRDataset), dan menyajikan insight penting yang berguna bagi pengambilan keputusan strategis perusahaan.

## Tujuan Proyek

Melalui pemanfaatan SQL secara intensif, proyek ini bertujuan untuk:
- Menganalisis karakteristik demografis tenaga kerja.
- Mengevaluasi struktur organisasi dan distribusi jabatan.
- Mengungkap disparitas gaji serta pola distribusinya.
- Mengukur kinerja dan produktivitas karyawan.
- Menelaah faktor-faktor turnover dan terminasi.
- Melacak tren masuk dan keluarnya karyawan dari tahun ke tahun.

## Dataset

Dataset yang digunakan adalah `HRDataset_v14.csv`, yang telah dikonversi ke database SQLite bernama `hr_database.db`. Dataset ini mencakup informasi penting seperti nama karyawan, jabatan, departemen, gaji, performa, status kerja, dan lainnya.

**Sumber dataset**:  
[Human Resources Data Set - Kaggle](https://www.kaggle.com/datasets/rhuebner/human-resources-data-set)


## Analisis dan SQL Query

### 1. Demografi Karyawan  
Tujuan: Memahami karakteristik dasar tenaga kerja.
- Jumlah karyawan berdasarkan jenis kelamin (`Sex`)
- Distribusi status pernikahan (`MaritalDesc`)
- Komposisi ras (`RaceDesc`)
- Jumlah karyawan berdasarkan kewarganegaraan (`CitizenDesc`)
- Persebaran berdasarkan negara bagian (`State`)

### 2. Struktur Organisasi  
Tujuan: Mengetahui penyebaran karyawan dalam organisasi.
- Jumlah karyawan per departemen (`Department`)
- Jumlah karyawan per posisi/jabatan (`Position`)
- Rata-rata gaji per posisi dan per departemen
- Jumlah bawahan tiap manajer (`ManagerName`)

### 3. Analisis Gaji  
Tujuan: Mengungkap distribusi dan ketimpangan gaji.
- Rata-rata, maksimum, dan minimum gaji
- Distribusi gaji berdasarkan jenis kelamin dan status pernikahan
- Karyawan dengan gaji tertinggi dan terendah

### 4. Kinerja dan Produktivitas  
Tujuan: Mengevaluasi performa dan keterlibatan karyawan.
- Rata-rata skor keterlibatan (`EngagementSurvey`) dan kepuasan (`EmpSatisfaction`)
- Total proyek khusus yang ditangani (`SpecialProjectsCount`)
- Korelasi antara skor performa dan jumlah absensi
- Total jumlah keterlambatan dalam 30 hari terakhir

### 5. Turnover dan Terminasi  
Tujuan: Memahami alasan dan pola karyawan keluar.
- Jumlah karyawan yang keluar (`Termd = 1`)
- Alasan terminasi utama (`TermReason`)
- Status kerja saat ini (`EmploymentStatus`)
- Perbandingan lama bekerja antara karyawan aktif dan nonaktif

### 6. Tren Tahunan Karyawan Masuk & Keluar  
Tujuan: Mengidentifikasi pola masuk dan keluarnya karyawan berdasarkan tahun.

## Teknologi yang Digunakan

- Python
- Pandas untuk manipulasi data
- SQLite untuk penyimpanan dan query data
- SQL Magic (`%%sql`) di Jupyter Notebook

## Struktur Proyek

```bash
📂 HR-Analytics-SQL
│
├── HRDataset_v14.csv
├── hr_database.db
├── HR_Analysis.ipynb
└── README.md
```
## Hasil dan Manfaat
Hasil analisis ini dapat membantu:
- Tim HR memahami demografi tenaga kerja
- Manajemen mengevaluasi efektivitas organisasi
- Pengambilan keputusan berbasis data terhadap gaji dan kinerja
- Menekan angka turnover dan memahami alasan terminasi
