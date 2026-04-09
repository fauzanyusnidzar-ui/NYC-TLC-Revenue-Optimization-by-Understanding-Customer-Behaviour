# NYC-TLC-Revenue-Optimization-by-Understanding-Customer-Behaviour
# 🗽 NYC Taxi Revenue Optimization Analysis

## 1. Project Overview
Proyek ini menganalisis data transaksi **New York City Taxi (TLC)** periode Januari 2023 untuk mengekstrak wawasan perilaku penumpang, meningkatkan efisiensi operasional, dan mengidentifikasi peluang optimalisasi pendapatan. 

Fokus utamanya adalah bagaimana pemahaman terhadap pola perilaku customer dapat dimanfaatkan untuk mengoptimalkan alokasi supply dan meningkatkan pendapatan taksi secara efektif, terutama di tengah persaingan dengan layanan *ride-hailing* seperti Uber dan Lyft.

### 🎯 Key Objectives:
* **Objective 1:** Menganalisis pola permintaan berdasarkan waktu (jam sibuk vs jam sepi) dan lokasi (Manhattan vs Outer Borough).
* **Objective 2:** Mengidentifikasi karakteristik perjalanan, termasuk dominasi jarak tempuh dan jenis pemesanan (*Street-Hail*).
* **Objective 3:** Memberikan rekomendasi strategis untuk meningkatkan revenue melalui insentif driver, penyesuaian armada, dan strategi pemasaran.

---

## 2. Data Sources
* **Dataset 1 (NYC TLC Trip Record):** Data transaksi perjalanan taksi NYC periode Januari 2023 (waktu pickup/dropoff, lokasi zona, jarak tempuh, tarif, dan pembayaran).
* **Dataset 2 (NYC Borough Information):** Data pendukung mengenai populasi dan luas wilayah borough di New York City untuk memperkaya analisis diagnostik.

---

## 3. Technologies Used
* **Programming Language:** Python (Pandas, NumPy)
* **Visualization:** Matplotlib, Seaborn, Choropleth Analysis
* **Environment:** Jupyter Notebook

---

## 4. Project Structure
```text
📂 nyc-taxi-analysis
├── 📄 README.md (Summary & Temuan)
├── 📁 data
│   ├── 📥 raw (Dataset Asli)
│   └── 🧹 cleaned (Data Bersih)
├── 📓 notebooks (Proses EDA)
├── 📊 reports (Laporan PDF)
│   └── 🖼️ figures (Grafik/Map)
├── ⚙️ requirements.txt (Library)
└── 🐍 src (Script Python)
---
```
## 📊 5. Summary of Findings

### 💡 5.1 Business Insights
> **Note:** Analisis dilakukan berdasarkan data transaksi Januari 2023 dengan fokus pada perilaku komuter dan efisiensi pendapatan.

| Aspek | Temuan Utama | Dampak Bisnis |
| :--- | :--- | :--- |
| **Jarak Tempuh** | **Dominasi Jarak Pendek:** Mayoritas perjalanan terjadi internal di Manhattan. | Taksi berfungsi sebagai *last-mile connectivity* menuju halte transportasi publik. |
| **Metode Order** | **99% Street-Hail:** Penumpang lebih suka menyetop taksi langsung di jalan. | Efisien di Manhattan, namun kehilangan pasar di *Outer Borough* yang bergantung pada aplikasi. |
| **Waktu & Revenue** | **Scarcity di Jam Sepi:** Pendapatan per trip tertinggi ada pada pukul **04.00 - 06.00**. | Meskipun *peak hour* sore hari ramai, kelangkaan armada di subuh hari menciptakan peluang tarif lebih tinggi. |
| **Pola Lokasi** | **Zonasi Residensial:** Rute tersibuk ada di area seperti East Harlem. | Pergerakan bukan didominasi orang kantoran, melainkan aktivitas warga lokal antar wilayah residensial. |

---

### 🚀 5.2 Actionable Recommendations

#### 📈 Strategi Operasional
* **Optimalisasi Supply & Waktu:** * Penerapan *Early Bird Surcharge* untuk menarik driver beroperasi pada pukul 04.00 - 06.00.
    * Insentif khusus bagi driver yang bersedia mengambil penumpang di wilayah *Low-Supply* (Outer Borough).

#### 📱 Transformasi Digital & Layanan
* **Digitalisasi Layanan (E-Hail):** Kolaborasi dengan aplikasi pemesanan untuk mencakup wilayah di luar Manhattan yang tidak memiliki budaya *street-hail*.
* **Fixed Rate Strategy:** Memberlakukan tarif flat untuk perjalanan antar-borough guna bersaing harga dengan kompetitor *ride-hailing*.

#### 🤝 Customer Loyalty & Welfare
* **Subscription Model:** Menghadirkan paket langganan bulanan bagi penumpang rutin di Manhattan untuk mengunci loyalitas pelanggan.
* **Nudge Payment System:** Mengatur *default tip* sebesar 15-20% pada mesin EDC/pembayaran digital untuk meningkatkan kesejahteraan driver secara langsung.
* **Armada SUV:** Menambah alokasi mobil berkapasitas besar di zona residensial untuk menargetkan segmen keluarga/group.

---
