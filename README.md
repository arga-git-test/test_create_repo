# 📊 Superstore Retail Performance & Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-Business_Intelligence-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Suatu solusi dashboard interaktif dan analitis yang dirancang untuk menganalisis performa penjualan (*Sales*), profitabilitas (*Profit*), tren pemesanan (*Orders*), serta faktor-faktor kunci yang mempengaruhi pertumbuhan bisnis retail **Superstore Retail**.

---

## 📌 Dataset Overview

* **Source Dataset:** [Kaggle - Superstore Dataset Final](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
* **Deskripsi Data:** Dataset ini berisi catatan transaksi penjualan ritel yang mencakup detail pesanan (Order ID, Order Date, Ship Date, Ship Mode), demografi pelanggan (Customer ID, Customer Name, Segment, Location), hierarki produk (Category, Sub-Category, Product Name), serta metrik finansial (Sales, Quantity, Discount, Profit).

---

## 🚀 Fitur Utama & Struktur Dashboard

Dashboard ini dibagi menjadi beberapa halaman (*Pages*) yang dirancang secara khusus untuk memberikan sudut pandang komprehensif, mulai dari gambaran umum eksekutif, analisis wilayah, hingga analisis faktor pengaruh (AI / Key Influencers).

---

### 🟢 Page 1: Executive Overview & Performance Trends
Halaman ini memberikan ringkasan tingkat tinggi mengenai performa bisnis ritel secara keseluruhan beserta metrik pertumbuhan Year-over-Year (YoY).

#### **Fitur Utama & Visualisasi:**
1. **KPI Scorecards & YoY Growth:**
   * **Total Sales:** $608.5K (▲ +29.3% YoY)
   * **Total Order:** 1,310 (▲ +26.2% YoY)
   * **Total Profit:** $81.7K (▲ +32.6% YoY)
   * **Total Customer:** 637 (▲ +11.2% YoY)
   * **Total Qty:** 9,810 (▲ +22.9% YoY)
2. **Sales & Profit Trend (Line Chart):** Tren bulanan yang membandingkan Total Sales dan Total Profit sepanjang periode berjalan untuk mengidentifikasi pola musiman (*seasonality*).
3. **Total Order & Forecasting (Line Chart with Forecast):** Visualisasi histori jumlah pesanan lengkap dengan proyeksi/prediksi tren pesanan di masa depan.
4. **Sales Breakdown:**
   * **By Segment (Donut Chart):** Distribusi penjualan antar segmen (*Consumer* 48.69%, *Corporate* 34.01%, *Home Office* 17.29%).
   * **By Product Categories (Donut Chart):** Proporsi penjualan berdasarkan kategori produk (*Technology* 37.15%, *Office Supplies* 30.16%, *Furniture* 32.69%).
5. **Interactive Slicers:** Pengaturan *Trend Period* dan *Performance Period* untuk menyesuaikan rentang waktu analisis.

#### **💡 Analisis & Keputusan Bisnis yang Dapat Diambil:**
* **Evaluasi Kesehatan Bisnis:** Pertumbuhan Sales (+29.3%) dan Profit (+32.6%) yang melampaui pertumbuhan volume pesanan (+26.2%) mengindikasikan efisiensi margin yang membaik dan peningkatan nilai rata-rata transaksi per pelanggan (*Average Order Value*).
* **Perencanaan Inventaris & Stok:** Menggunakan grafik *Total Order Forecasting* untuk mempersiapkan jumlah pasokan barang di gudang sebelum terjadi lonjakan pesanan musiman di kuartal akhir.
* **Strategi Penjualan Segmen:** Segmen *Consumer* menyumbang hampir 50% dari total penjualan. Keputusan pemasaran dapat difokuskan untuk mempertahankan segmen *Consumer* sembari menyusun program promosi khusus (*B2B bulk discount*) untuk meningkatkan kontribusi dari segmen *Home Office*.

---

### 🟡 Page 2: Regional & Geography Performance Analysis
Halaman ini berfokus pada pemetaan geografis dan analisis detail performa ritel berdasarkan negara bagian (States) serta berbagai dimensi produk.

#### **Fitur Utama & Visualisasi:**
1. **Interactive Spatial Map (Bing Regional Performance):** Peta wilayah interaktif yang memperlihatkan intensitas penjualan di seluruh wilayah Amerika Serikat dengan *color-coding* visual.
2. **Comprehensive Regional Performance Table:** Tabel detail performa per *State* yang menampilkan:
   * **Total Order & YoY Order Growth**
   * **Total Sales & YoY Sales Growth**
   * **Total Profit & YoY Profit Growth**
3. **Multi-dimensional Slicers & Dynamic Metric Selection:**
   * Filter berdasarkan *Segment*, *Category*, *Sub Category*, *Ship Mode*, dan *Performance Period*.
   * Dropdown *Select Metric* untuk mengubah variabel utama analisis dengan cepat.

#### **💡 Analisis & Keputusan Bisnis yang Dapat Diambil:**
* **Identifikasi Top & Low Performing States:**
   * **Top Performers (misal: California & New York):** Memiliki kontribusi *Total Sales* dan *Profit* sangat tinggi. Keputusan: Mempertahankan infrastruktur logistik dan kampanye promosi yang agresif.
   * **Unprofitable / Loss-Making States (misal: Texas, Ohio, Pennsylvania, Illinois):** Walaupun penjualan terbilang cukup tinggi, wilayah ini mengalami **profit negatif/kerugian** (misal: Texas -$5,240, Ohio -$7,568).
* **Keputusan Strategi Operasional:**
   * **Evaluasi Diskon & Biaya Pengiriman:** Kerugian di negara bagian tertentu umumnya disebabkan oleh pemberian diskon yang terlalu tinggi atau biaya pengiriman yang membengkak. Manajemen perlu meninjau kembali kebijakan diskon regional dan mengevaluasi mitra logistik di wilayah teridentifikasi.

---

### 🔵 Page 3: Decomposition Tree & AI Key Influencers
Halaman ini memanfaatkan kemampuan *Advanced Analytics* & *Artificial Intelligence* (AI) untuk memahami faktor-faktor pendorong (*drivers*) utama yang mempengaruhi metrik bisnis.

#### **Fitur Utama & Visualisasi:**
1. **Decomposition Tree (Pohon Dekomposisi):**
   * Mengurai *Selected Metric* secara hirarkis dari segmen (*Consumer, Corporate, Home Office*) down-to kategori produk (*Furniture, Technology, Office Supplies*).
   * Memungkinkan pengguna melakukan *drill-down* eksploratif secara dinamis.
2. **Key Influencers Visual (AI Powered):**
   * Menjawab pertanyaan: *"What influences Selected Metric to Increase?"*
   * Menampilkan faktor utama beserta estimasi rata-rata kenaikan metrik (misal: Penjualan meningkat signifikan ketika *Sub Category is Tables* [+459.6] atau *Chairs* [+334.7]).
   * Membandingkan rata-rata nilai metrik antar sub-kategori (*Copiers, Machines, Tables, Bookcases, Chairs, dll.*).

#### **💡 Analisis & Keputusan Bisnis yang Dapat Diambil:**
* **Root Cause Analysis & Cross-Selling:** Mengidentifikasi sub-kategori bernilai tinggi (*Tables, Chairs, Copiers, Machines*). Keputusan: Menjadikan produk-produk ini sebagai produk utama dalam paket *bundling* atau penawaran *cross-selling* ke pelanggan segmen *Corporate*.
* **Optimasi Portofolio Produk:** Mengetahui sub-kategori mana yang menjadi pendorong terbesar peningkatan profit/sales sehingga perusahaan dapat mengalokasikan anggaran pemasaran secara presisi pada produk yang berpotensi menghasilkan return tertinggi.

---

## 🛠️ Tools & Teknologi Digunakan
* **Business Intelligence Tool:** Microsoft Power BI / Tableau
* **Dataset:** Kaggle Superstore Dataset
* **Teknik Analisis:** Time Series Forecasting, Geospatial Mapping, YoY Metric Calculations, AI-Driven Key Influencers analysis.

---

## 📝 Cara Menggunakan Dashboard
1. Gunakan filter **Performance Period** untuk memilih tahun analisis yang diinginkan.
2. Klik pada segmen atau wilayah tertentu di **Page 1** & **Page 2** untuk melakukan *cross-filtering* ke seluruh grafik.
3. Buka **Page 3** untuk melakukan analisis sebab-akibat dan melihat faktor yang paling mempengaruhi performa finansial.
