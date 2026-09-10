# LexIP India — Unified IPR Search Console (Phase 1 Prototype)

A unified search interface across Indian Intellectual Property databases (Trademarks, Patents, Copyrights, and Geographical Indications).

## 🚀 Live Demo
- **Prototype Link:** https://talktovaishnavi25-hue.github.io/lexip-unified-ipr/
## 🎯 Problem Statement
Searching Indian IP currently requires navigating 4 separate government portals (InPASS for patents, TM Public Search for trademarks, Copyright Office, and GI Registry). Legal professionals face high friction, fragmented data structures, and lack of cross-record verification.

## 🛠️ Phase 1 Architecture
- **Unified Query Layer:** Debounced global search across Mark/Title, Applicant, and Application Number.
- **Faceted Categorization:** Segmented views isolating Nice Class (TM), IPC Class (Patents), Work Categories (Copyright), and Registered Territories (GI).
- **Compliance by Design (DPDP Act, 2023):** Redacts personal applicant addresses to align with upcoming digital personal data enforcement timelines.
- **Verification Layer Foundation:** Every record captures `source_url` and `retrieved_at` timestamps, staging one-click source verification for Phase 2 crawling pipelines.

## ⚖️ Legal & Operational Risk Mitigation
- **Phase 1 Approach:** Uses a curated, normalized static dataset to validate product-market fit before introducing automated crawling.
- **IT Act & Terms of Use Compliance:** Zero automated CAPTCHA bypassing. Respects manual human-portal boundaries while architecting data schemas for future licensed API/bulk-data pipelines.

## 💻 Tech Stack
- Frontend: Single-File React 18, Tailwind CSS, Lucide Icons, Babel Runtime.
- Deployment: Edge-hosted via Netlify / GitHub Pages.
