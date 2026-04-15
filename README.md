# 🌍 Berita Kebencanaan Dashboard

Dashboard monitoring **berita kebencanaan nasional** yang melakukan **web scraping otomatis dari berbagai portal berita** dan menyajikannya dalam bentuk **dataset, detail berita, serta tabel kejadian bencana**.

Dashboard ini dibangun menggunakan **Python dan Streamlit** untuk membantu memantau informasi bencana secara cepat dari berbagai sumber media online.

---

# 📸 Tampilan Dashboard

## 📰 Dataset Berita
Dashboard menampilkan seluruh berita hasil scraping yang telah dikumpulkan dari berbagai portal berita.

![Dataset](docs/dashboard_dataset.png)

---

## 📖 Detail Berita
Pengguna dapat melihat **ringkasan isi berita**, tanggal, tag, serta link menuju sumber berita asli.

![Detail](docs/dashboard_detail.png)

---

## 📊 Tabel Kejadian Bencana
Dashboard juga mengekstrak informasi kejadian bencana seperti:

- Jenis bencana
- Waktu kejadian
- Provinsi
- Dampak kejadian
- Korban terdampak

![Tabel Bencana](docs/dashboard_bencana.png)

---

# 🚀 Fitur Utama

## 🔎 Multi Source Scraping
Mengambil berita dari berbagai portal berita seperti:

- Detik
- Kompas
- MetroTV

---

## 🔑 Keyword Filtering
Scraping dilakukan berdasarkan keyword tertentu seperti:

- Bencana
- Banjir
- Tanah Longsor
- Gempa Bumi

---

## 📅 Filter Tanggal
Pengguna dapat menentukan rentang waktu scraping berita.

---

## 📊 Dashboard Monitoring
Menampilkan statistik seperti:

- Total berita
- Jumlah sumber berita
- Status scraping

---

## 📰 Detail Artikel
Menampilkan:

- Judul berita
- Isi berita
- Tanggal publikasi
- Tag
- Link sumber

---

## 📑 Ekstraksi Informasi Kejadian
Sistem mencoba mengekstrak informasi penting dari isi berita seperti:

- Provinsi
- Jenis bencana
- Jumlah korban
- Jumlah pengungsi

---

# 🛠️ Tech Stack

Project ini dibangun menggunakan:

- Python
- Streamlit
- BeautifulSoup
- Requests
- Pandas

---

# 📦 Instalasi

Clone repository:

```bash
git clone https://github.com/username/berita-kebencanaan-dashboard.git
cd berita-kebencanaan-dashboard
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Contoh isi `requirements.txt`:

```txt
streamlit
requests
beautifulsoup4
pandas
lxml
```

---

# ▶️ Menjalankan Aplikasi

Jalankan Streamlit:

```bash
streamlit run app.py
```

Kemudian buka di browser:

```
http://localhost:8501
```

---

# 📂 Struktur Project

```
berita-kebencanaan-dashboard
│
├── app.py
├── scraper.py
├── requirements.txt
│
├── data
│   └── berita.csv
│
├── images
│   └── logo.png
│
└── docs
    ├── dashboard_dataset.png
    ├── dashboard_detail.png
    └── dashboard_bencana.png
```

---

# ⚙️ Cara Kerja Sistem

1. User memilih:
   - sumber berita
   - keyword
   - rentang tanggal

2. Sistem melakukan scraping berita dari website.

3. Data yang diambil:

- Judul
- Tanggal
- Isi berita
- Link berita

4. Sistem melakukan **ekstraksi informasi kejadian bencana** dari isi berita.

5. Hasil ditampilkan pada dashboard Streamlit.

---

# 📊 Contoh Output Dataset

| No | Judul | Tanggal | Website | Tag |
|----|------|------|------|------|
| 1 | Banjir Rendam Bekasi | 15 April 2026 | Detik | banjir, bekasi |
| 2 | Gempa M4.5 Guncang Sumba | 12 April 2026 | Kompas | gempa, sumba |

---

# 📌 Use Case

Dashboard ini dapat digunakan untuk:

- Monitoring berita kebencanaan
- Analisis kejadian bencana berbasis berita
- Early information monitoring
- Pengumpulan dataset penelitian

---

# ⚠️ Disclaimer

Data diperoleh dari hasil scraping portal berita dan hanya digunakan untuk tujuan:

- penelitian
- analisis data
- monitoring informasi publik

---

# 👨‍💻 Author

Developed by **Andrew Putra**
