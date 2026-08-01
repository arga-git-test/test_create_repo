# 📊 Superstore Retail Performance & Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-Business_Intelligence-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📌 Deskripsi Proyek
Dashboard **Superstore Retail Analytics** dirancang untuk memberikan wawasan mendalam mengenai performa penjualan (*sales*), profitabilitas (*profit*), serta tren pemesanan (*order trend*) dari bisnis ritel Superstore. Dashboard ini memungkinkan *stakeholder* untuk mengevaluasi pertumbuhan **Year-over-Year (YoY)**, menganalisis kontribusi antar segmen & kategori produk, memantau distribusi geografis (regional), hingga menganalisis faktor penentu (*Key Influencers*) yang mendorong peningkatan performa bisnis.

---

## 📈 Ringkasan Performa Utama (Key Metrics)

Berdasarkan periode analisis utama (2013):

* **Total Sales:** $608.5K (`+29.3% YoY`)[cite: 1]
* **Total Profit:** $81.7K (`+32.6% YoY`)[cite: 1]
* **Total Orders:** 1,310 Orders (`+26.2% YoY`)[cite: 1]
* **Total Customers:** 637 Customers (`+11.2% YoY`)[cite: 1]
* **Total Quantity Sold:** 9,810 Units[cite: 1]

---

## 🔍 Fitur Utama Dashboard

### 1. **Overview & Sales vs Profit Trend**
* **Tren Penjualan & Profit:** Visualisasi garis harian/bulanan yang membandingkan Total Sales dan Total Profit dari periode 2011 hingga 2013[cite: 1].
* **Forecasting Total Order:** Analisis tren pemesanan (*Total Order*) yang dilengkapi dengan fitur *forecasting* hingga tahun 2014[cite: 1].

### 2. **Segmentasi Pelanggan & Kategori Produk**
* **Sales by Segment:**
  * **Consumer:** 48.69% ($296.3K)[cite: 1]
  * **Corporate:** 34.01% ($206.9K)[cite: 1]
  * **Home Office:** 17.29% ($105.2K)[cite: 1]
* **Sales by Product Category:**
  * **Technology:** 37.15%[cite: 1]
  * **Office Supplies:** 32.69%[cite: 1]
  * **Furniture:** 30.16%[cite: 1]

### 3. **Regional & State Performance**
* **Peta Interaktif (Microsoft Bing):** Memvisualisasikan sebaran performa di berbagai negara bagian Amerika Serikat[cite: 1].
* **Tabel Performa Negara Bagian (State Breakdown):** Detail performa lengkap (Order, Sales, Profit, dan pertumbuhan YoY per negara bagian)[cite: 1].
  * *Top Performers:* California ($131.2K Sales), New York ($71.8K Sales), Virginia ($26.7K Sales)[cite: 1].

### 4. **Advanced Analytics & Decomposition Tree**
* **Decomposition Tree:** Membongkar kontribusi metrik berdasarkan hirarki Segmen (Consumer, Corporate, Home Office) dan Kategori Produk (Furniture, Technology, Office Supplies)[cite: 1].
* **Key Influencers (AI Analytics):** Menganalisis faktor utama penyebab peningkatan metrik:
  * Rata-rata *Selected Metric* meningkat paling tinggi ketika **Sub-category = Tables** (`+$459.6`), disusul oleh **Chairs** (`+$334.7`), **Technology** (`+$278.8`), dan **Phones** (`+$157.1`)[cite: 1].

---

## 🛠️ Teknologi & Tools yang Digunakan

* **Business Intelligence Tool:** Microsoft Power BI / Tableau / Looker Studio[cite: 1]
* **Map Service Integration:** Microsoft Bing Maps[cite: 1]
* **Data Sources:** Superstore Retail Dataset[cite: 1]
* **Key Analytics Features:** Time Series Forecasting, Key Influencer Visual, Decomposition Tree[cite: 1]

---

## 📂 Struktur Repositori

```text
.
├── assets/                  # Screenshot & gambar dashboard
│   ├── dashboard_overview.png
│   ├── regional_performance.png
│   └── key_influencers.png
├── data/                    # Dataset (jika bersifat publik)
│   └── superstore_dataset.csv
├── Superstore_Dashboard.pbix # File proyek Power BI / Workbook
└── README.md                # Dokumentasi proyek
