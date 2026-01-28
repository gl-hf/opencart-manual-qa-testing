# OpenCart Manual QA Testing Project

## Project Overview
This project demonstrates manual testing of the OpenCart demo e‑commerce application.  
The goal was to validate core user flows, identify functional and UX issues, and document defects using industry‑standard QA practices (checklists, test cases, bug reports, reproducible steps, severity/priority, screenshots).

## Application Under Test
- **URL:** https://demo.opencart.com  
- **Type:** Demo e‑commerce web application  

## Scope of Testing
- Homepage & navigation  
- Header elements (logo, currency switcher)  
- Catalog & category structure  
- Product pages  
- Cart functionality  
- Checkout flow (partially — limited by demo stock)  
- UI/UX validation  
- Negative testing (invalid inputs, edge cases)  
- Basic performance & SEO checks (Lighthouse)

## Out of Scope / Limitations
- Real payment processing  
- Admin panel  
- Backend/database testing  
- Security testing  

**Important note:**  
The demo environment contains many known issues and limitations.  
The goal of this project was not to test every possible scenario, but to demonstrate a structured QA approach and identify representative defects.  
Some flows (e.g., checkout, account pages) were partially blocked due to **Cloudflare Error 1015 (KAN‑4)** and demo restrictions.

---

## Test Environment
- **OS:** Windows 10  
- **Browser:** Google Chrome 122
- **Device:** Desktop  
- **Environment:** Demo  
- **Tools:** Jira, Excel, Chrome DevTools, Lighthouse  

---

## Test Artifacts
- **Checklist:** 44 test items  
- **Test Cases:** 21  
- **Bug Reports:** 15 issues created in Jira  
- **Bug Export:** `03_BugReports_Jira_Export.csv`  
- **Screenshots:** Evidence for each defect (`/screenshots`)  
- **Lighthouse Report:** SEO & performance audit  

## Repository Structure

---

```text
/OpenCart-QA-Project
│
├── README.md
│
├── 01_Checklist.xlsx
│
├── 02_TestCases.xlsx
│
├── 03_BugReports_Jira_Export.csv
│
├── /screenshots
│     ├── KAN-4.png
│     ├── KAN-15_1.png
│     ├── KAN-15_2.png
│     ├── KAN-17.png
│     └── ...
│
└── /lighthouse
      └── lighthouse-report.html
```

---

## Test Execution Summary
- Smoke, functional, negative and UX tests executed  
- Checkout partially blocked due to demo limitations  
- **15 defects reported:**  
  - **1 Blocker**  
  - **3 Critical**  
  - **7 Major**  
  - **4 Minor**  
- All defects documented with reproducible steps, AR/ER, environment, severity & priority  
- SEO issues identified via Lighthouse  

---

## Key Defects (Examples)
- **KAN‑4:** Cloudflare Error 1015 blocks users (Blocker)  
- **KAN‑15:** Out‑of‑stock products can be added to cart (Blocker)  
- **KAN‑17:** Quantity field accepts invalid values (Critical)  
- **KAN‑5:** Missing product image for Product 8 (Minor)  
- **KAN‑18:** Currency format inconsistent across currencies (Minor)  

---

## Project Purpose
This project was created to demonstrate practical manual QA skills, including:

- Test design  
- Exploratory testing  
- Defect reporting in Jira  
- UI/UX analysis  
- Negative testing  
- Basic SEO/performance checks  
- Documentation and structuring of QA artifacts  

It is intended as a portfolio project to showcase real QA workflow and testing methodology.

---

## Author


Andrii Snihur (2026)
