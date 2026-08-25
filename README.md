<div align="center">

# 🗺️ Afyon Map Scraper & Business Insights Pipeline
### Automated Google Maps Data Harvesting, Cleaning & Intelligence Engine for Afyonkarahisar

> [!IMPORTANT]
> **📌 NOTE:** 
> The real-world dataset containing **592 unique businesses** extracted by this project has been added to the root directory as **`Afyon_Komple_Puanli_Final.xlsx`**. You can click to inspect or download it directly!

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![Python](https://img.shields.io/badge/python-3.x-blue.svg)]()
[![Selenium](https://img.shields.io/badge/automation-Selenium-orange.svg)]()
[![Pandas](https://img.shields.io/badge/data-Pandas-green.svg)]()
[![License](https://img.shields.io/badge/license-MIT-purple.svg)]()

*An industrial-grade, automated data pipeline engineered to extract, sanitize, and structure 500+ real-world commercial listings across all 12 districts of Afyonkarahisar—turning raw geospatial data into actionable market intelligence.*

</div>

---

## 💡 Why This Project?

In modern market research and local logistics, gathering clean geographical data at scale is a massive bottleneck. Manual collection is tedious, error-prone, and unsustainable. 

**Afyon Map Scraper & Insights** solves this problem by automating the entire intelligence lifecycle:
1. **Navigates** dynamic map interfaces across different districts autonomously.
2. **Bypasses** rendering hurdles by simulating human scrolling and handling complex DOM structures.
3. **Sanitizes** and deduplicates chaotic web data into a pristine, analysis-ready dataset.

Whether you are a market analyst looking to map regional business densities or a developer exploring robust web automation architectures, this tool delivers clean, verified data out of the box.

---

## 📊 Included Dataset (`Afyon_Komple_Puanli_Final.xlsx`)

Transparency and verification are key to great software. This repository includes a pre-compiled, real-world dataset extracted directly using this automation tool:
* **Total Verified Enterprises:** 592 unique businesses
* **Geographical Scope:** All 12 districts of Afyonkarahisar (Merkez, Sandıklı, Bolvadin, Dinar, Çay, Emirdağ, İscehisar, Şuhut, Sinanpaşa, Dazkırı, Bayat, Çobanlar)
* **Captured Attributes:** Business Name (`İşletme Adı`), Star Rating (`Yıldız Puanı`), District (`İlçe`), and City (`Şehir`).
* **Format:** Clean, structured Excel spreadsheet ready for BI tools (PowerBI, Tableau) or data science workflows.

---

## ⚙️ Key Technical Features

* **Multi-District Batch Processing:** Dynamically loops through regional parameters to ensure zero coverage gaps.
* **Robust Dynamic Scroll Engine:** Interacts with hidden feed containers (`div[role="feed"]`) to trigger lazy-loaded map elements seamlessly.
* **Smart Fallback Parsing:** Multi-layered exception handling (`try-except`) that extracts ratings reliably from both class selectors and complex `aria-label` DOM properties.
* **Automated Data Hygiene:** Integrated Pandas pipeline that filters out duplicates and normalizes string values for pristine reporting.

---

## 🛠️ Technology Stack

* **Core Language:** Python
* **Web Scraping & Automation:** Selenium WebDriver, WebDriver Manager
* **Data Manipulation & Cleaning:** Pandas
* **Output Format:** OpenXML Spreadsheet (.xlsx)
* **Version Control:** Git & GitHub

---

## 🚀 Quick Start & Installation

To run or test this pipeline on your local machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/e-uynk/Afyon-Map-Scraper-Insights.git](https://github.com/e-uynk/Afyon-Map-Scraper-Insights.git)

```

2. **Install dependencies:**
```bash
pip install pandas selenium webdriver-manager

```


3. **Execute the automation script:**
```bash
python main.py

```


4. **Access the output:** Check your project directory for the generated structured report (`Afyon_Komple_Puanli_Final.xlsx`).

---

## 👤 Author

**Esad UYANIK**

* Software Developer
* [GitHub Profile](https://www.google.com/search?q=https://github.com/e-uynk)

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

