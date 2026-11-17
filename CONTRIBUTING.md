# Contributing to End Times Digital Library (1900–2026)

Thank you for helping preserve and expand this open-source scholarly resource!

## Strict Quality & Verification Standards

Every Pull Request adding books, hadith references, FAQs, or translations MUST follow these rules:

1. **Preserve Existing Book IDs (`#1–#140`):** Never renumber existing entries, user bookmarks and personal notes stored in `localStorage` rely on stable IDs. Append new books starting at `#141+`.
2. **Respect the 3-Tier Evidentiary Framework:**
   - **Tier 1:** Only direct Qur'an verses or authentic (*sahih* / *hasan*) hadiths with exact collection & number (verified on `Sunnah.com` or `Dorar.net`).
   - **Tier 2:** Scholarly monographs, classical commentaries, or vetted compilations. Mark as `tier2_caution` if the work mixes weak (*da'if*) or *Isra'iliyyat* reports without rigorous authentication.
   - **Tier 3:** Contemporary geopolitical or speculative books must be clearly tagged `tier3` and never presented as definitive prophecy.
3. **100% Verified Direct URLs Only:** Every link must resolve to an authentic legal open-access host (IslamHouse, Shamela.ws, Waqfeya, Kitabosunnat, Internet Archive, publisher/WorldCat catalog)، never link to pirated sites or unverified shorteners.
4. **Zero-Dependency Architecture:** Keep `index.html` self-contained without mandatory external JS/CSS CDNs so it works reliably offline and on static GitHub Pages hosting.
5. **Update Both Data & Catalog:** When adding a book, update `data/books.json`, `catalog/End_Times_Digital_Library_1900-2026_v5.md`, and `index.html`.

## How to Submit a Contribution
1. Fork this repository and create a feature branch (`git checkout -b add-book-example`).
2. Make your edits and test `index.html` locally (`python3 -m http.server 8080`).
3. Verify zero JavaScript console errors and valid JSON in `data/books.json`.
4. Open a Pull Request describing the source verification for every new entry or citation.
