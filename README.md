<div align="center">

# 🗺️ Afyon Map Scraper & Business Insights Pipeline
### Enterprise-Grade Google Maps Data Harvesting, Sanitization & Intelligence Engine

> **📌 NOTE:** 
> The real-world dataset containing **592 unique businesses** across all 12 districts extracted by this project has been pre-compiled and added to the root directory as **`Afyon_Komple_Puanli_Final.xlsx`**. You can inspect or download it directly!

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![Python](https://img.shields.io/badge/python-3.x-blue.svg)]()
[![Selenium](https://img.shields.io/badge/automation-Selenium-orange.svg)]()
[![Pandas](https://img.shields.io/badge/data-Pandas-green.svg)]()
[![License](https://img.shields.io/badge/license-MIT-purple.svg)]()

*An advanced, automated data pipeline engineered to extract, sanitize, and structure 500+ real-world commercial listings across all 12 districts of Afyonkarahisar—transforming chaotic geospatial web elements into pristine, analysis-ready market intelligence.*

</div>

---

## 🚀 Executive Summary

In modern market research, competitor analysis, and local logistics, acquiring clean geographical data at scale is a monumental bottleneck. Traditional manual collection is tedious, error-prone, and economically unsustainable. 

**Afyon Map Scraper & Insights** solves this challenge by automating the entire intelligence lifecycle. This repository doesn't just provide a script; it delivers a **verified, production-ready dataset** along with a robust automation architecture designed to bypass modern web rendering hurdles.

---

## 📊 Live Verified Dataset (`Afyon_Komple_Puanli_Final.xlsx`)

Transparency and empirical proof drive great engineering. This repository includes a pre-compiled dataset harvested directly through this pipeline:
* **Total Verified Enterprises:** 592 unique, deduplicated businesses.
* **Geographical Coverage:** 100% of Afyonkarahisar’s 12 districts (*Merkez, Sandıklı, Bolvadin, Dinar, Çay, Emirdağ, İscehisar, Şuhut, Sinanpaşa, Dazkırı, Bayat, Çobanlar*).
* **Granular Attributes:** Business Name (`İşletme Adı`), Star Rating (`Yıldız Puanı`), District (`İlçe`), and City (`Şehir`).
* **Format:** Clean OpenXML spreadsheet optimized for immediate integration into BI dashboards (PowerBI, Tableau) or machine learning models.

---

## 🏗️ Architecture & Technical Deep-Dive

The pipeline is structured around three core engineering pillars designed to handle the unpredictable nature of modern web scraping:

1. **Autonomous Multi-District Iteration:**
   * Programmatically cycles through an array of regional parameters, constructing targeted geographic query URLs to eliminate coverage gaps.
2. **Robust Dynamic Scroll Engine (Infinite Scroll Management):**
   * Interacts directly with hidden feed containers (`div[role="feed"]`) via JavaScript execution (`scrollTop = scrollHeight`) to trigger lazy-loaded DOM elements seamlessly without crashing.
3. **Smart Fallback Parsing & Exception Resilience:**
   * Web elements frequently change or drop attributes. The scraper utilizes multi-layered `try-except` blocks to extract star ratings reliably from both class selectors (`span.MW4T7d`) and complex DOM properties (`aria-label`).
4. **Automated Data Hygiene & Pipeline Sanitization:**
   * Raw scraped entries pass through an automated **Pandas** data hygiene filter that strips out whitespace anomalies, handles missing data points, and enforces strict deduplication (`drop_duplicates`).

---

## 🛠️ Technology Stack

* **Core Engine:** Python
* **Web Scraping & Browser Automation:** Selenium WebDriver, WebDriver Manager
* **Data Transformation & Cleansing:** Pandas
* **Output Specification:** OpenXML Spreadsheet (.xlsx)
* **Environment & Version Control:** Git, GitHub

---

## ⚙️ Quick Start & Installation

To run, test, or extend this data pipeline locally:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/e-uynk/Afyon-Map-Scraper-Insights.git](https://github.com/e-uynk/Afyon-Map-Scraper-Insights.git)

```

2. **Navigate to the project directory:**
```bash
cd Afyon-Map-Scraper-Insights

```


3. **Install required dependencies:**
```bash
pip install pandas selenium webdriver-manager

```


4. **Execute the automation pipeline:**
```bash
python main.py

```


5. **Inspect the output:** Locate the freshly generated `Afyon_Komple_Puanli_Final.xlsx` report right inside your root directory.

---

## 👤 Author

**Esad UYANIK**

* Software Developer
* [GitHub Profile](https://www.google.com/search?q=https://github.com/e-uynk)

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

```
