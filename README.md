# PowerBI Stimulator Enterprise 📊🏢
**By Adewale Samson Adeagbo**

![Version](https://img.shields.io/badge/version-2.0.0--enterprise-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg) ![Platform](https://img.shields.io/badge/platform-Static%20Browser%20App-orange.svg) ![AI API](https://img.shields.io/badge/AI%20API-Not%20Used-red.svg)

## Overview

**PowerBI Stimulator Enterprise** is a unified, additive, browser-based Business Intelligence simulation platform. It merges the original uploaded PowerBI Stimulator work with the enterprise enhancement layer already prepared in the workspace.

The result is a single cohesive static application for:

- Power BI-style learning,
- classroom demonstrations,
- portfolio showcase,
- lightweight local BI practice,
- enterprise governance simulation,
- offline/no-cost analytics training.

It is built with free web technologies and deliberately avoids AI APIs because paid model calls are not cost-effective for this use case.

## Important Positioning

This is a **Power BI-style enterprise simulator** for educational, demonstration and portfolio use. It is not affiliated with Microsoft and does not contain Microsoft proprietary source code. It recreates familiar BI concepts and workflows using HTML, CSS, JavaScript, browser storage and static hosting.

## Why This Exists

Adewale Samson Adeagbo's work shows that useful data tools can be built for learners and organisations without waiting for expensive infrastructure. This project supports people using low-resource devices, including tablets and entry-level laptops, by keeping computation inside the browser.

## Cost and API Statement

This project uses:

- No OpenAI API.
- No Gemini API.
- No Claude API.
- No paid model endpoint.
- No backend database.
- No paid server.
- No paid Power BI Service dependency.

All insight generation is deterministic and rule-based. Data parsing, profiling, joining, pivoting, calculations, dashboards, audit logs and backups run locally in the browser.

## Core BI Features Preserved

1. Home Dashboard
2. Data View
3. Data Quality Auditor
4. Report View / Canvas
5. Power Query-style Statistical Engine
6. Pivot Matrix
7. Themes & Formatting
8. Model View / Join Engine
9. DAX-style Measures / Calculated Fields
10. Report Scheduler Simulation
11. Heatmap Calendar
12. KPI Goal Tracker
13. Time Intelligence Compare
14. Rule-based Insight Studio
15. Project Backup / Restore
16. PWA support

## Enterprise Features Added

1. Enterprise Workspaces
2. Semantic Model Relationship Discovery
3. Row-Level Security Simulation
4. Data Lineage View
5. Refresh and Gateway Simulation
6. Deployment Pipeline Simulation
7. Apps, Sharing and Subscriptions Simulation
8. Tenant Admin Portal
9. Audit Logs
10. Metric Alerts
11. Bookmarks and Story Mode
12. Mobile Report Layout Preview
13. Sensitivity labels and endorsement simulation
14. Embedded HMG / Adewale identity

## About the Platform Owner

**Adewale Samson Adeagbo**  
Data Scientist · STEM Educator · AI-Augmented Solutions Developer · Founder, HMG Concepts

Adewale is an educator and builder with 15+ years of classroom experience in Nigeria. He is associated with HMG Concepts, HMG Academy, HMG Technologies and HMG Media.

- Portfolio: https://cssadewale.pages.dev
- HMG Concepts: https://hmgconcepts.pages.dev
- HMG Academy: https://hmgacademy.pages.dev
- GitHub: https://github.com/cssadewale
- LinkedIn: https://linkedin.com/in/adewalesamsonadeagbo
- WhatsApp / Hotline: +234 810 086 6322

See `ABOUT_ADEWALE.md` for the full embedded persona profile.

## Folder Structure

```text
enterprise/
├── index.html
├── manifest.webmanifest
├── sw.js
├── _headers
├── robots.txt
├── LICENSE
├── README.md
├── FEATURES.md
├── DEPLOYMENT.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── ABOUT_ADEWALE.md
├── ENTERPRISE_NOTES.md
├── SECURITY.md
├── PRIVACY.md
├── GOVERNANCE.md
├── sample_sales.csv
├── assets/icon.svg
├── data/sample_sales.csv
├── data/sample-sales.csv
├── docs/source-audit.md
└── docs/user-guide.md
```

## Quick Start

1. Open `index.html` in a modern browser.
2. Click **Sample** to generate sample datasets.
3. Click **Auto Report** to build report widgets.
4. Open **Data View** to inspect rows and run the Data Quality Auditor.
5. Open **Stats** to run the statistical engine.
6. Open **Workspace**, **Semantic Model**, **RLS**, **Lineage**, **Refresh**, **Pipeline**, **Sharing** and **Admin** to test enterprise simulations.
7. Use **Backup** to export the full project JSON.

## Deployment Summary

The app is static. Upload the contents of this folder to GitHub Pages, Cloudflare Pages, Netlify or any static host. No build command is needed.

See `DEPLOYMENT.md` for exact step-by-step instructions.
