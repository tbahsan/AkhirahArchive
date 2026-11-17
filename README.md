# AkhirahArchive: Islamic Eschatology Digital Library (1900–2026)

[![Version](https://img.shields.io/badge/version-6.0%20International-0F5C44?style=flat-square)](#)
[![Languages](https://img.shields.io/badge/UI%20%26%20Catalog-EN%20%C2%B7%20BN%20%C2%B7%20AR%20%C2%B7%20UR-1D4A78?style=flat-square)](#4-language-interface--auto-detection)
[![Books](https://img.shields.io/badge/verified%20books-140-9A7432?style=flat-square)](#catalog-overview)
[![Issues](https://img.shields.io/github/issues/tbahsan/AkhirahArchive?style=flat-square&color=144D40)](https://github.com/tbahsan/AkhirahArchive/issues)
[![License: MIT](https://img.shields.io/badge/license-MIT-555555?style=flat-square)](LICENSE)

An open-source, zero-dependency, offline-first multilingual digital library and scholarly reference hub on **Islamic Eschatology** (*Ashrat al-Sa'ah*, *Fitan*, *Barzakh*, and *Akhirah*). Designed to run directly from a single standalone `index.html` file on **GitHub Pages** ([tbahsan.github.io/AkhirahArchive](https://tbahsan.github.io/AkhirahArchive/)) or completely offline in any modern browser.

---

## Table of Contents

- [Overview](#overview)
- [3-Tier Evidentiary Framework](#3-tier-evidentiary-framework)
- [Key Features](#key-features)
- [4-Language Interface & Auto-Detection](#4-language-interface--auto-detection)
- [Catalog Overview](#catalog-overview)
- [Quick Start & Deployment](#quick-start--deployment)
- [Repository Structure](#repository-structure)
- [Multilingual Subject Index & Keywords](#multilingual-subject-index--keywords)
- [Contributing](#contributing)
- [Credits & Maintenance](#credits--maintenance)
- [License](#license)

---

## Overview

Discussions around the Signs of the Hour (*Ashrat al-Sa'ah*) and End-Times narrations frequently mix authentic revelation, unverified popular traditions, and modern geopolitical speculation. This project addresses that gap by organizing **140 verified books (1900–2026)** and classical commentaries across **English, Bengali, Arabic, and Urdu** under a strict evidentiary classification, paired with primary scripture links, an offline eschatology map, practical du'as, scholarly FAQs, and interactive study tools.

---

## 3-Tier Evidentiary Framework

Every source in the library is transparently classified into one of three evidentiary tiers:

| Tier | Category | Description & Usage Guidance |
| :--- | :--- | :--- |
| **Tier 1** | **Primary Revelation** | The Noble Qur'an and authentic *Sahih*/*Hasan* Sunnah (linked directly via Quran.com, Sunnah.com, and Dorar.net). Forms the sole binding foundation of belief. |
| **Tier 2** | **Scholarly Research & Classical Commentaries** | Peer-reviewed academic editions, classical hadith commentaries (*Fath al-Bari*, *Sharh Sahih Muslim*, *Sharh al-Aqidah al-Tahawiyyah*), and verified modern monographs. Historical compilations containing mixed chains are explicitly flagged with **Isnad Caution**. |
| **Tier 3** | **Contemporary / Speculative Analysis** | Modern geopolitical essays and personal authorial readings of current events. Included for critical awareness and explicitly separated from binding creed. |

---

## Key Features

- **140 Verified Multilingual Books (`#1–#140`):** Searchable and filterable by language, evidentiary tier, access type (free PDF/online read, Archive.org, catalog info), topic, classical status, and reading progress, with a collapsible filter drawer, compact pagination (`12 / 24 / 48 / All`), and card/table views.
- **Built-in GitHub Issues Feedback Hub:** Visitors can suggest verified books, report broken links (pre-filled directly from any book modal), submit translation fixes, and browse live open issues from [`tbahsan/AkhirahArchive`](https://github.com/tbahsan/AkhirahArchive/issues) directly inside the app, with graceful offline fallback.
- **Interactive Offline SVG Geography Map:** 10 clickable authentic hadith locations (Makkah & al-Bayda, Madinah & Hijaz, Damascus Eastern Minaret, Bab Ludd, Bayt al-Maqdis & Mount Tur, Dabiq & A'maq, Constantinople, River Euphrates, Isfahan & Khorasan, and Aden/Yemen) with direct hadith references and related books.
- **Signs & Afterlife Timeline:** 14 Minor Signs (categorized as fulfilled, ongoing, and future), all 10 Major Signs, and the 12-stage journey of the Afterlife from death and *Barzakh* to Paradise and Hellfire.
- **Practical Action, Protection Du'as & 25 FAQs:** 6 authentic protection du'as (with Arabic script, transliteration, translation, and one-click copy), a persistent daily preparation checklist, and 25 searchable scholarly Q&As.
- **Verification & Active Study Tools:**
  - **Ijma vs. Ikhtilaf:** Clear separation between Sunni consensus and legitimate scholarly differences.
  - **Myth-Buster & Comparative Table:** Fact-checking common viral eschatological misconceptions.
  - **3-Deck 3D Flip Flashcards:** Glossary terms, 10 Major Signs, and 12 core authentic hadiths.
  - **12-Question Self-Assessment Quiz:** Instant explanations aligned with authentic sources.
- **Scholar Profiles, Edition Guides & Extra Sources:** 16 classical and modern scholar bios, 6 critical-edition buying/reading guides, a 4-stage study roadmap, 6 academic theses, and 4 verified lecture series.
- **Local-First Personal Workspace:** Bookmarks, reading status tracker, personal notes, 3-book side-by-side comparison, custom book additions, CSV/Markdown exports, printable study sheets, JSON backup/restore, and Light/Dark themes, stored strictly in browser `localStorage` with zero user tracking.

---

## 4-Language Interface & Auto-Detection

The entire interface, book summaries, map labels, du'as, FAQs, flashcards, and quizzes are available in four languages with automatic **LTR / RTL layout mirroring**:

- **English (`en`):** LTR
- **বাংলা / Bengali (`bn`):** LTR
- **العربية / Arabic (`ar`):** Full RTL (`dir="rtl"`)
- **اردو / Urdu (`ur`):** Full RTL (`dir="rtl"`)

### Automatic Default Language Selection
On first visit, the app automatically selects the best language using a privacy-friendly cascade:
1. **URL Parameter (`?lang=en|bn|ar|ur`)** or saved manual user preference (`localStorage`).
2. **Instant Offline Timezone Detection (`Intl`):** e.g., `Asia/Dhaka` → Bengali, `Asia/Karachi` → Urdu, Arab world timezones → Arabic, otherwise browser locale (`navigator.languages`) or English.
3. **Optional Non-Blocking IP Country Lookup:** When hosted online (e.g., GitHub Pages), a lightweight background country lookup (`get.geojs.io`) refines the default language if no manual preference has been set. Fails silently when offline.

Visitors can switch languages at any time from the header switcher.

---

## Catalog Overview

| Language | Books | Highlights |
| :--- | :---: | :--- |
| **English (`en`)** | 40 | Al-Ashqar, Ibn Kathir, Al-Ghazali (Winter ed.), Al-Albani, Brill *Roads to Paradise*, critical methodologies |
| **Arabic (`ar`)** | 35 | *Fath al-Bari* (Vol. 13), *Sharh Sahih Muslim* (Vol. 18), *Sharh al-Tahawiyyah*, Al-Wabil, Al-Muqaddim, Al-Bayhaqi |
| **Urdu (`ur`)** | 35 | Anwar Shah Kashmiri, Mufti Muhammad Shafi, Maulana Yusuf Ludhianvi, Kitabosunnat verified editions |
| **Bengali (`bn`)** | 30 | Dr. Abdullah Jahangir, IslamHouse verified translations, classical & contemporary studies |
| **Total** | **140** | **94 direct free reads/PDFs · 33 classical works & commentaries** |

---

## Quick Start & Deployment

### Option 1: Use Offline Immediately
Download `index.html` and open it directly in any modern web browser (Chrome, Firefox, Safari, Edge). No server, build step, or internet connection is required for browsing, searching, reading notes, map exploration, flashcards, or quizzes.

### Option 2: Deploy Free on GitHub Pages
1. Fork or push this repository to your GitHub account.
2. Go to **Repository Settings → Pages**.
3. Under **Build and deployment → Source**:
   - Select **GitHub Actions** (uses the included `.github/workflows/pages.yml` automatically), **or**
   - Select **Deploy from a branch** → `main` → `/ (root)` and click **Save**.
4. Your site will be live within ~60 seconds at:
   `https://tbahsan.github.io/AkhirahArchive/`

### Option 3: Local Preview Server
```bash
python3 -m http.server 8080
# Open http://localhost:8080 in your browser
```

---

## Repository Structure

```text
.
├── index.html                                    # Standalone v6.0 International web app (zero dependencies, SEO + JSON-LD)
├── og-preview.png                                # 1200x630 Open Graph / Twitter social preview banner
├── robots.txt                                    # Search crawler directives
├── sitemap.xml                                   # Multilingual XML sitemap (EN, BN, AR, UR hreflang)
├── data/
│   └── books.json                                # Structured JSON dataset of all 140 verified books (4-language summaries)
├── catalog/
│   └── End_Times_Digital_Library_1900-2026_v5.md # Full scholarly Markdown catalog (§§A–I)
├── .github/
│   ├── ISSUE_TEMPLATE/                           # Structured GitHub Issue forms (books, broken links, feedback)
│   └── workflows/
│       └── pages.yml                             # Automated GitHub Pages deployment workflow
├── .nojekyll                                     # Prevents Jekyll processing on GitHub Pages
├── CONTRIBUTING.md                               # Verification standards & contribution guide
├── LICENSE                                       # MIT License
└── README.md                                     # Project documentation
```

---

## Multilingual Subject Index & Keywords

To aid global searchability and research discovery across English, Bengali, Arabic, and Urdu, **AkhirahArchive** covers the following core topics and classical references:

- **English:** Islamic eschatology, Signs of the Hour (*Ashrat al-Sa'ah*), Minor Signs, 10 Major Signs of Qiyamah, *Fitan* and *Malahim*, *al-Masih al-Dajjal*, *Imam al-Mahdi*, Descent of *Isa ibn Maryam* (Jesus in Islam), Gog and Magog (*Ya'juj* and *Ma'juj*), *Barzakh* and the life of the grave, Day of Judgment (*Yawm al-Qiyamah*), *Akhirah*, *Jannah* and *Jahannam*, Sahih Bukhari *Kitab al-Fitan*, Sahih Muslim Book 54, *Fath al-Bari*, *Sharh al-Aqidah al-Tahawiyyah*, Hadith verification (*Tahqiq*), Islamic digital library, open-source Islamic reference.
- **বাংলা (Bengali):** কিয়ামতের আলামত, কিয়ামতের ছোট ও বড় নিদর্শন, আখিরী জামানা, দাজ্জাল, ইমাম মাহদী, ঈসা (আ.)-এর অবতরণ, ইয়াজুজ মাজুজ, ফিতান ও মালাহিম, কবর ও বারযাখ, আখিরাত, জান্নাত ও জাহান্নাম, সহীহ হাদিসভিত্তিক বই, ইসলামিক ডিজিটাল লাইব্রেরি, ড. আব্দুল্লাহ জাহাঙ্গীর, ইবনে কাসীর, আলবানী।
- **العربية (Arabic):** أشراط الساعة الصغرى والكبرى، علامات يوم القيامة، الفتن والملاحم، المسيح الدجال، المهدي، نزول عيسى عليه السلام، يأجوج ومأجوج، عذاب القبر وعالم البرزخ، البعث والحشر والجنة والنار، فقه أشراط الساعة، فتح الباري، شرح صحيح مسلم، شرح العقيدة الطحاوية، مكتبة إسلامية رقمية.
- **اردو (Urdu):** علاماتِ قیامت صغریٰ و کبریٰ، قیامت کی نشانیاں، آخری زمانے کے فتن و ملاحم، فتنۂ مسیحِ دجال، امام مہدی، نزولِ عیسیٰ علیہ السلام، یاجوج و ماجوج، عذابِ قبر اور عالمِ برزخ، حشر و آخرت، جنت و جہنم، اسلامی ڈیجیٹل لائبریری، صحیح احادیث، علامہ انور شاہ کشمیری، مفتی محمد شفیع، دکتور یوسف الوابل۔

---

## Contributing

Contributions (such as newly verified scholarly editions, broken-link fixes, translation refinements, or UI accessibility enhancements) are warmly welcome. Please review [`CONTRIBUTING.md`](CONTRIBUTING.md) before submitting a Pull Request.

---

## Credits & Maintenance

> **This project was created with Artificial Intelligence under the direction and maintenance of [Tasneem Bin Ahsan](https://github.com/tbahsan). Users are encouraged to verify references directly against primary texts.**

- **Maintainer:** Tasneem Bin Ahsan ([github.com/tbahsan](https://github.com/tbahsan))
- **Built With:** Artificial Intelligence (catalog curation, 4-language localization, scholarly structure, and zero-dependency single-file web architecture)

---

## License

This project is open source and licensed under the [MIT License](LICENSE).

All third-party books, translations, and primary texts linked within the catalog remain the intellectual property of their respective authors, publishers, and open Islamic digital archives (IslamHouse, Shamela.ws, Kitabosunnat, Internet Archive, Sunnah.com, Quran.com, and Dorar.net).
