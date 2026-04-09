# NYC-TLC-Revenue-Optimization-by-Understanding-Customer-Behaviour
1. Project Overview

Proyek ini menganalisis data transaksi New York City Taxi (TLC) periode Januari 2023 untuk mengekstrak wawasan perilaku     penumpang, meningkatkan efisiensi operasional, dan mengidentifikasi peluang optimalisasi pendapatan. Fokus utamanya adalah bagaimana pemahaman terhadap pola perilaku customer dapat dimanfaatkan untuk mengoptimalkan alokasi supply dan meningkatkan pendapatan taksi secara efektif, terutama di tengah persaingan dengan layanan ride-hailing seperti Uber dan Lyft.

Key Objectives:

Objective 1: Menganalisis pola permintaan berdasarkan waktu (jam sibuk vs jam sepi) dan lokasi (Manhattan vs Outer Borough).
Objective 2: Mengidentifikasi karakteristik perjalanan, termasuk dominasi jarak tempuh dan jenis pemesanan (Street-Hail).
Objective 3: Memberikan rekomendasi strategis untuk meningkatkan revenue melalui insentif driver, penyesuaian armada, dan strategi pemasaran.

2. Data Sources

Dataset 1 (NYC TLC Trip Record) – Data transaksi perjalanan taksi NYC periode Januari 2023 yang mencakup informasi waktu pickup/dropoff, lokasi zona, jarak tempuh, hingga detail tarif dan pembayaran.

Dataset 2 (NYC Borough Information) – Data pendukung mengenai populasi dan luas wilayah borough di New York City untuk memperkaya analisis diagnostik.

3. Technologies Used

Programming Language: Python (Pandas, NumPy)

Visualization: Matplotlib, Seaborn, Choropleth Analysis

Others: Jupyter Notebook

4. Project Structure
Plaintext

├── README.md          <- Ringkasan proyek dan temuan utama.
├── data
│   ├── raw            <- Dataset asli dari NYC TLC Januari 2023.
│   └── cleaned        <- Data yang telah dibersihkan (menghapus outlier, data kosong, & tahun anomali).
├── notebooks          <- Jupyter notebooks berisi proses cleaning, EDA, dan Analisis Diagnostik.
├── reports            <- Laporan PDF: "Revenue Optimization by Understanding Customer Behaviour".
│   └── figures        <- Heatmap, Barplot, dan Choropleth map.
├── requirements.txt   <- Daftar library Python yang dibutuhkan.
└── src                <- Script python untuk pengolahan data.

5. Summary of Finding
    5.1 Business Insight

Dominasi Perjalanan Pendek: Mayoritas perjalanan terjadi di internal Manhattan dengan jarak pendek hingga moderat,     berfungsi sebagai transportasi pelengkap ke halte transportasi publik.

Metode Pemesanan: 99% pemesanan dilakukan melalui Street-Hail (setop di jalan), yang sangat efisien di Manhattan namun membuat taksi kalah saing dengan aplikasi di Outer Borough.

Scarcity di Jam Sepi: Meskipun peak hour terjadi pukul 14.00 - 20.00, pendapatan per perjalanan (fare per trip) justru lebih tinggi pada pukul 04.00 - 06.00 karena kelangkaan armada.

Pola Lokasi: Rute paling ramai didominasi oleh pergerakan antar zona residensial (seperti East Harlem), bukan area perkantoran.

5.2 Actionable Recommendation

Optimalisasi Supply & Waktu: Memberikan insentif bagi driver (misal: kenaikan fare per km atau surcharge) untuk mengambil trip di luar jam sibuk atau di wilayah dengan demand tinggi yang sepi armada.

Digitalisasi Layanan: Meningkatkan layanan pesan online melalui kerjasama dengan platform E-Hail dan memberlakukan fixed rate serta promo khusus di luar Manhattan untuk bersaing dengan layanan aplikasi.

Strategi Pemasaran & Armada: Menerapkan sistem subscription untuk pelanggan rutin di Manhattan dan mulai menyediakan armada SUV untuk menargetkan kelompok penumpang lebih dari satu orang.

Mendorong Tip: Menampilkan sugesti tip (15-20%) pada sistem pembayaran kartu kredit dan memasang stiker standar tip pada armada untuk meningkatkan kesejahteraan driver.
