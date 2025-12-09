# Employee Attrition Analysis & Key Retention Strategy

---

## Overview
Proyek ini bertujuan memahami pola attrition (karyawan keluar) dan faktor-faktor yang memengaruhinya, seperti departemen, usia, masa kerja, gaji, lembur, kepuasan kerja, hingga job role. Analisis dilakukan untuk membantu perusahaan mengidentifikasi kelompok karyawan berisiko tinggi resign dan menyusun strategi retensi yang lebih tepat. Hasil analisis digunakan untuk memberikan rekomendasi retensi yang berdampak langsung pada stabilitas operasional perusahaan.

---

## File Description
- employee.csv : Dataset HR dari Kaggle (IBM HR Analytics).
- employee_clean.csv : Dataset bersih, siap untuk analisis.
- hr_attrition_analysis.ipynb : Notebook Python berisi proses EDA, visualisasi, uji statistik, dan insight bisnis.
- Tableau Dashboard : Visualisasi interaktif attrition berdasarkan job role, usia, gaji, dan kepuasan kerja.

---

## Steps
1. Memahami Dataset
- Dataset berisi 1470 karyawan dan 35 variabel tanpa missing value.
- Variabel penting: Department, JobRole, MonthlyIncome, Age, OverTime, EducationField, JobSatisfaction, dan Attrition.
- Nilai kategori pada kolom kepuasan (1–4) diubah menjadi label agar mudah dianalisis.

2. Data Preparation
- Konversi kolom Yes/No → 1/0.
- Membuat kelompok usia (18–25, 26–35, dst).
- Mengecek tipe data dan duplikasi.
- Menyimpan ulang dataset yang siap dipakai.

3. Analisis Utama
- Pola Attrition berdasarkan department, job role, tenure, dan age group.
- Pengaruh gaji terhadap attrition menggunakan statistik deskriptif dan boxplot.
- Hubungan faktor pekerjaan (department, job role, overtime, education field, marital status) menggunakan Chi-Square.
- Pengaruh kepuasan kerja (environment, job satisfaction, job involvement) terhadap risiko resign.
- Identifikasi kelompok risiko tinggi seperti sales representative, usia 18–25, dan karyawan dengan job involvement rendah.

---

## Insights
- Departemen paling rentan: Sales memiliki attrition tertinggi, terutama Sales Representative (~40%).
- Usia: Karyawan muda 18–25 tahun paling sering resign.
- Gaji: Karyawan dengan gaji rendah lebih banyak keluar dibanding yang bergaji lebih tinggi.
- Overtime: Karyawan yang sering lembur memiliki peluang resign lebih besar.
- Kepuasan & Keterlibatan: Attrition tertinggi terjadi pada karyawan dengan kepuasan dan keterlibatan kerja rendah (hingga 34%).

---

## Conclusion
Attrition perusahaan banyak dipengaruhi oleh faktor internal: job role, gaji, overtime, dan kepuasan kerja. Kombinasi beban kerja berat, gaji rendah, dan keterlibatan kerja yang minim menjadi pemicu utama karyawan resign. Perusahaan perlu fokus pada role risiko tinggi dan meningkatkan program retensi untuk karyawan muda dan kelompok berpenghasilan rendah.

---

## Recommendation & Action Plan
1.	Prioritaskan Departemen Sales
- Perbaiki workload & berikan dukungan role-based training.
2.	Retensi Karyawan Muda
- Optimalkan onboarding dan mentorship 6 bulan pertama.
3.	Evaluasi Struktur Gaji
- Berikan adjustment untuk segmen gaji rendah dan penalti lembur berlebih.
4.	Atur Lembur
- Redistribusikan pekerjaan atau tambah tenaga untuk role kritis.
5.	Tingkatkan Kepuasan & Engagement
- Terapkan employee recognition, survei berkala, dan pengembangan karier.

---

## Business Impact
- Potensi penurunan attrition rate 10–20% dalam satu tahun.
- Efisiensi besar pada biaya rekrutmen & pelatihan.
- Produktivitas tim meningkat karena turnover menurun.
- Stabilitas operasional lebih terjaga, terutama pada posisi yang berhubungan langsung dengan revenue.

---

## Visualization

Tableau Dashboard: https://public.tableau.com/app/profile/rifqi.nadhir.aziz/viz/attrition_dashboard/Dashboard1?publish=yes


---

## Tools & Libraries
- Python – Pandas, Matplotlib, Seaborn, SciPy (Chi-Square Test)
- Tableau – Dashboard interaktif attrition
- Jupyter Notebook – EDA & analisis statistik

---

## 👤 Author
Rifqi Nadhir Aziz