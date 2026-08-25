<div align="center">

# 🗺️ National-Maps-Scraper-Pipeline
### Dual-Scale Enterprise Architecture: From Regional Automated Harvesting to Nationwide Spatial Analytics

> [!IMPORTANT]
> **📌 NOTE / DATASETS AVAILABLE:** 
> This repository features a dual-scale data architecture containing two pre-compiled, real-world verified datasets located directly in the root directory:
> 1. **Regional Deep-Dive:** **`Afyon_Komple_Puanli_Final.xlsx`** (592 granular business listings across all 12 districts of Afyonkarahisar).
> 2. **Nationwide Scale:** **`TR Genel Esad Uyanık.xlsx`** (250,000+ verified commercial listings spanning across Turkey, equipped with spatial coordinates and review metrics).
> 
> *You can click and inspect or download both datasets directly from the file list above!*

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![Python](https://img.shields.io/badge/python-3.x-blue.svg)]()
[![Selenium](https://img.shields.io/badge/automation-Selenium-orange.svg)]()
[![Pandas](https://img.shields.io/badge/data-Pandas-green.svg)]()
[![License](https://img.shields.io/badge/license-MIT-purple.svg)]()

*An advanced, production-grade automated data pipeline engineered to transition seamlessly from targeted regional intelligence to massive nationwide spatial data harvesting—transforming chaotic geospatial web elements into pristine, analysis-ready business insights.*

</div>

---

## 🚀 Executive Summary & Architecture Evolution

In modern market research, competitor analysis, and location-based logistics, acquiring clean geographical data at scale is a monumental bottleneck. Traditional manual collection is tedious, error-prone, and economically unsustainable.

**National-Maps-Scraper-Pipeline** demonstrates a scalable engineering lifecycle:
* **Phase 1 (Regional Granularity):** Automated 100% coverage across Afyonkarahisar's 12 districts to build robust DOM traversal and fallback mechanisms.
* **Phase 2 (Nationwide Scaling):** Scaled the pipeline architecture to harvest, sanitize, and structure **250,000+ commercial listings nationwide**, complete with geographic coordinates (Latitude/Longitude) and engagement metrics (Review Counts).

---

## 📊 Included Datasets

Transparency and empirical scale drive great software engineering. This repository includes two distinct, production-ready datasets harvested directly via this automation pipeline:

### 1. Regional Dataset (`Afyon_Komple_Puanli_Final.xlsx`)
* **Total Records:** 592 unique enterprises.
* **Geographical Scope:** 12 districts of Afyonkarahisar (*Merkez, Sandıklı, Bolvadin, Dinar, Çay, Emirdağ, İscehisar, Şuhut, Sinanpaşa, Dazkırı, Bayat, Çobanlar*).
* **Attributes:** Business Name (`İşletme Adı`), Star Rating (`Yıldız Puanı`), District (`İlçe`), and City (`Şehir`).

### 2. Nationwide Spatial Dataset (`TR Genel Esad Uyanık.xlsx`)
* **Total Records:** 250,000+ unique, deduplicated businesses.
* **Geographical Scope:** Comprehensive multi-province and multi-city Turkish territorial coverage.
* **Granular Attributes:** Plate Code (`Plaka`), City (`İl`), District (`İlçe`), Business Name (`Restoran Adı`), Star Rating (`Yıldız`), Review Count (`Yorum Sayısı`), Latitude (`Enlem`), and Longitude (`Boylam`).
* **Format:** Clean OpenXML spreadsheets optimized for immediate integration into BI dashboards (PowerBI, Tableau), GIS tools, or spatial machine learning models.

---

## 🏗️ Core Engineering & Technical Deep-Dive

The underlying Python automation engine is built on robust engineering pillars to withstand unpredictable web scraping environments:

1. **Autonomous Multi-Region & District Iteration:**
   * Programmatically builds and executes targeted geographic query parameters, ensuring zero coverage gaps whether operating at a city or national level.
2. **Robust Dynamic Scroll Engine (Infinite Scroll Management):**
   * Interacts directly with hidden feed containers (`div[role="feed"]`) via JavaScript execution (`scrollTop = scrollHeight`) to trigger lazy-loaded DOM elements seamlessly across hundreds of thousands of entries without crashing.
3. **Smart Fallback Parsing & Exception Resilience:**
   * Web element structures frequently change. The scraper implements multi-layered `try-except` blocks to extract star ratings, review metrics, and coordinates reliably from complex DOM properties and `aria-label` attributes.
4. **Automated Data Hygiene & Pipeline Sanitization:**
   * Raw scraped entries pass through an automated **Pandas** data hygiene pipeline that strips out whitespace anomalies, handles missing data points, validates spatial coordinates, and enforces strict deduplication (`drop_duplicates`).

---

## 🛠️ Technology Stack

* **Core Engine:** Python
* **Web Scraping & Browser Automation:** Selenium WebDriver, WebDriver Manager
* **Data Transformation & Cleansing:** Pandas
* **Output Specification:** OpenXML Spreadsheets (.xlsx)
* **Environment & Version Control:** Git, GitHub (`.gitignore`, `.gitattributes` configured)

---

## ⚙️ Quick Start & Installation

To run, test, or extend this data pipeline locally:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/e-uynk/National-Maps-Scraper-Pipeline.git](https://github.com/e-uynk/National-Maps-Scraper-Pipeline.git)

```

2. **Navigate to the project directory:**
```bash
cd National-Maps-Scraper-Pipeline

```


3. **Install required dependencies:**
```bash
pip install pandas selenium webdriver-manager

```


4. **Execute the automation pipeline:**
```bash
python main.py

```


5. **Inspect the outputs:** Locate both the regional report and the massive nationwide spatial database (`TR Genel Esad Uyanık.xlsx`) right inside your root directory.

---

## 👤 Author

**Esad UYANIK**

* Software Developer
* [GitHub Profile](https://www.google.com/search?q=https://github.com/e-uynk)

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

```
