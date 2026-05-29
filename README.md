# 📂 Struktur Project & Penjelasan Berkas

Berikut struktur project beserta fungsi masing-masing folder dan file:

```bash
CAPSTONE/
│── data/
│   ├── coursera_courses.csv
│   ├── coursera_courses_clean.csv
│   ├── coursera_courses_dashboard.csv
│   ├── all_skills.json
│   └── data_dictionary.txt
│
│── notebook/
│   └── CAPSTONE_PROJECT.ipynb
│
│── report/
│   └── Laporan Komprehensif.pdf
│
│── dashboard.py
│── requirements.txt
│── url.txt
│── README.md
```

## 📁 Folder `data/`

Folder ini berisi dataset dan data hasil preprocessing yang digunakan pada proses analisis, recommendation system, dan dashboard.

### `coursera_courses.csv`

Dataset mentah (*raw dataset*) course Coursera sebelum dilakukan preprocessing.

### `coursera_courses_clean.csv`

Dataset hasil data cleaning dan preprocessing yang telah siap digunakan untuk:

* Exploratory Data Analysis (EDA)
* Recommendation System
* A/B Testing
* Dashboard Visualization

### `coursera_courses_dashboard.csv`

Dataset final yang telah disesuaikan untuk kebutuhan visualisasi dashboard Streamlit agar proses rendering lebih optimal.

### `all_skills.json`

File JSON yang berisi kumpulan skill hasil preprocessing untuk mendukung feature engineering pada recommendation system.

### `data_dictionary.txt`

Dokumentasi penjelasan setiap fitur/kolom dataset beserta tipe data dan deskripsinya sehingga mempermudah pemahaman struktur data.

---

## 📁 Folder `notebook/`

Folder ini berisi notebook utama project.

### `CAPSTONE_PROJECT.ipynb`

Notebook utama yang berisi seluruh proses end-to-end project, meliputi:

* Data Understanding
* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* TF-IDF Embedding
* Recommendation System
* Evaluation Analysis
* A/B Testing
* Visualization & Explanatory Analysis
* Conclusion

Notebook ini digunakan sebagai dokumentasi proses analisis data dan pengembangan recommendation system secara lengkap.

---

## 📁 Folder `report/`

Folder ini berisi dokumentasi laporan teknis project.

### `Laporan Komprehensif.pdf`

Laporan teknis komprehensif yang menjelaskan keseluruhan proses pengembangan project, mulai dari:

* Business Understanding
* Data Understanding
* Data Preparation
* Exploratory Data Analysis
* Recommendation Modeling
* Evaluation
* Insight Analysis
* Conclusion

Laporan ini digunakan sebagai dokumentasi formal hasil pengerjaan capstone project.

---

## 📄 `dashboard.py`

File utama aplikasi dashboard interaktif berbasis **Streamlit**.

Dashboard digunakan untuk:

* Menampilkan insight hasil EDA
* Menampilkan visualisasi business question
* Menjalankan demo recommendation system
* Menampilkan hasil A/B Testing
* Menampilkan kesimpulan project (*conclusion*)

Dashboard bersifat interaktif karena pengguna dapat melakukan filtering data dan mencoba recommendation system secara langsung.

---

## 📄 `requirements.txt`

Berisi daftar library (*dependencies*) yang dibutuhkan untuk menjalankan project.

Seluruh library dapat diinstall menggunakan command berikut:

```bash
pip install -r requirements.txt
```

### Library yang Digunakan

* streamlit
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* scipy

---

# 🚀 Cara Menjalankan Dashboard Secara Lokal

Reviewer atau pengguna dapat menjalankan dashboard pada laptop masing-masing dengan langkah berikut.

## 1. Clone Repository

Download repository terlebih dahulu:

```bash
git clone https://github.com/CodingCamp2026-EduAssist/edu-assist-data-scientist.git
```

Masuk ke folder project:

```bash
cd CAPSTONE
```

---

## 2. Install Dependencies

Install seluruh library yang dibutuhkan:

```bash
pip install -r requirements.txt
```

### Apabila Menggunakan Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

#### Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

---

## 3. Pastikan Struktur Folder Tidak Berubah

Pastikan seluruh file tersusun sesuai struktur project agar dataset dapat terbaca dengan benar oleh dashboard.

```bash
CAPSTONE/
│── data/
│── notebook/
│── report/
│── dashboard.py
│── requirements.txt
```

---

## 4. Jalankan Dashboard Streamlit

Gunakan command berikut:

```bash
streamlit run dashboard.py
```

---

## 5. Buka Dashboard pada Browser

Setelah berhasil dijalankan, dashboard dapat diakses melalui browser:

```text
http://localhost:****
```

Dashboard akan menampilkan:

* 🏠 Overview Dataset
* 📊 Business Insights (EDA)
* 🤖 Demo Recommendation System
* 🧪 A/B Testing Recommendation
* 📌 Conclusion

---

## 📄 `url.txt`

File ini berisi link deploy dashboard Streamlit yang dapat diakses secara online tanpa perlu menjalankan project secara lokal.

Pengguna dapat langsung membuka dashboard melalui URL yang tersedia pada file tersebut.

---
