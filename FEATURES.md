# PowerBI Stimulator Enterprise — Complete Feature Guide

This document explains the unified additive system. It combines the original PowerBI Stimulator features with the enterprise BI simulation features.

## 1. Home Dashboard
The Home Dashboard displays dataset count, row count, column count, report visual count, feature map, recent data preview and the embedded Adewale / HMG identity card.

**Purpose:** Give users an immediate overview of the current BI workspace and reinforce ownership/branding.

## 2. Data View
Data View manages local datasets. Users can import CSV, TSV, JSON and XLSX/XLS when the free SheetJS browser library is available.

Capabilities:
- Dataset preview.
- Automatic column detection.
- Type inference.
- CSV export.
- Local browser storage.
- Backup and restore.

**Privacy:** Data is processed inside the browser.

## 3. Data Quality Auditor
Checks a selected dataset for:
- Missing values.
- Duplicate rows.
- Column data type.
- Unique value count.
- Potential data quality issues.

It also includes a safe cleanup action that trims string values and removes exact duplicate rows.

## 4. Report View
Recreates a Power BI-style canvas using free browser rendering.

Supported visuals:
- Bar chart.
- Line chart.
- Donut chart.
- KPI card.
- Table visual.
- Text box.

Users can create visuals manually or use **Auto Report**.

## 5. Power Query Editor / Statistical Engine
Profiles every column with:
- Count.
- Nulls.
- Unique values.
- Minimum.
- Maximum.
- Mean.
- Median.
- Mode.
- Standard deviation.
- Variance.
- Q1.
- Q3.
- IQR.
- Coefficient of variation.
- Outlier count.

## 6. Pivot Matrix
Builds cross-tab summaries.

Users choose:
- Dataset.
- Row field.
- Column field.
- Value field.
- Aggregation.

Aggregations:
- SUM.
- AVERAGE.
- COUNT.
- MIN.
- MAX.
- COUNT DISTINCT.

## 7. Themes & Formatting
Includes reusable palettes and live preview.

Included palette ideas:
- PowerBI.
- Lagos.
- Classroom.
- Executive.
- Accessible.

Themes can be exported and imported as JSON.

## 8. Model View / Data Join Engine
Simulates model building by combining two datasets with key columns.

Supported joins:
- INNER JOIN.
- LEFT JOIN.
- RIGHT JOIN.
- OUTER JOIN.

The joined result can be saved as a new dataset.

## 9. DAX-style Measures / Calculated Fields
Creates derived columns using local JavaScript/math expressions.

Examples:

```text
quantity * unit_price
round({{revenue}} * 0.075, 2)
({{revenue}} - {{cost}}) / {{revenue}}
```

It is not full Microsoft DAX. It is a free local training simulation.

## 10. Report Scheduler
Simulates report subscriptions while the browser tab is open.

Supported local exports:
- Project JSON.
- Report HTML.
- First dataset CSV.

Email uses `mailto:` drafts. No paid email API is used.

## 11. Heatmap Calendar
Creates a GitHub-style activity chart from a date field.

It can:
- Count records per day.
- Sum a numeric value per day.
- Filter by year.
- Display daily intensity.

## 12. KPI Goal Tracker
Creates local enterprise goals with:
- Name.
- Current value.
- Target value.
- Completion percentage.
- Ring gauge.
- Progress bar.

## 13. Time Intelligence Compare
Compares two period filters against a numeric metric.

It calculates:
- Period A total.
- Period B total.
- Absolute delta.
- Percentage change.
- Visual comparison chart.

## 14. Rule-based Insight Studio
A no-AI insight feature that generates deterministic observations from local data.

It checks:
- Dataset size.
- Missing values.
- Numeric minimum, maximum and average.
- Top category value.

It does not call OpenAI, Gemini, Claude or any model endpoint.

# Enterprise Features

## 15. Enterprise Workspaces
Simulates Power BI Service workspaces.

A workspace contains:
- Reports.
- Datasets / semantic models.
- Members.
- Sensitivity labels.
- Endorsement status.
- Owner details.

Default workspace: **HMG Enterprise BI Workspace** owned by **Adewale Samson Adeagbo**.

## 16. Semantic Model Relationship Discovery
Scans loaded datasets and finds matching column names.

It displays:
- Dataset cards.
- Columns.
- Data types.
- Relationship candidates.
- Cardinality estimate.
- Match count.
- Certified model badge.

## 17. Row-Level Security Simulation
Lets users create security roles such as:

```text
Role: Lagos Viewer
Rule: region = Lagos
```

It previews rows visible to that role and stores the role locally.

**Important:** This is a training simulation. Production RLS requires server-side identity enforcement.

## 18. Data Lineage View
Shows movement of data across the BI lifecycle:

```text
Sources → Semantic Model → Reports → Enterprise App → Consumers
```

It also produces an impact table.

## 19. Refresh & Gateway Simulator
Simulates:
- Gateway status.
- Refresh schedules.
- Manual refresh.
- Refresh history through audit logs.

Because the app is static, cloud background jobs are not used.

## 20. Deployment Pipelines
Simulates enterprise Application Lifecycle Management.

Stages:
- Development.
- Test.
- Production.

Promotions are logged in the audit trail.

## 21. Apps, Sharing & Subscriptions
Simulates organisational app distribution.

Supports:
- Publish app simulation.
- Viewer access list.
- Role assignment.
- Sensitivity label.
- Internal/external sharing documentation.

## 22. Tenant Admin Portal
Simulates tenant governance.

Includes:
- Export data setting.
- External sharing setting.
- Publish to web setting.
- Sensitivity label setting.
- Audit setting.
- Owner profile.
- Audit log table.

## 23. Audit Logs
Audit logs record key actions such as:
- Workspace creation.
- RLS role creation.
- Refresh schedule creation.
- Manual refresh.
- Pipeline promotion.
- App publishing.
- Viewer addition.
- Alert creation.
- Bookmark save/restore.
- Tenant setting changes.

Logs can be exported as CSV.

## 24. Metric Alerts
Creates local threshold rules.

Example:

```text
Total revenue > 100000
```

Status values:
- Triggered.
- OK.
- Not evaluated.

## 25. Bookmarks & Story Mode
Bookmarks save report canvas states for presentation story points.

Users can:
- Save a bookmark.
- Restore a bookmark.
- Use bookmarks for report storytelling.

## 26. Mobile Layout Preview
Creates a phone-sized report preview.

Useful for mobile-first stakeholders such as school owners, administrators, teachers and partners.

## 27. Project Backup / Restore
Backup exports complete project state to JSON:
- Datasets.
- Reports.
- Goals.
- Enterprise settings.
- Workspaces.
- RLS roles.
- Audit logs.
- Alerts.
- Bookmarks.

Restore imports that JSON back into the browser.

## 28. PWA Support
Includes:
- `manifest.webmanifest`.
- `sw.js`.

When deployed over HTTPS, users can install it using **Add to Home Screen**.

## 29. Embedded HMG / Adewale Identity
The platform embeds:
- Adewale Samson Adeagbo's name.
- Professional title.
- HMG Concepts.
- HMG Academy.
- HMG Technologies.
- Portfolio link.
- GitHub link.
- LinkedIn link.
- WhatsApp number.
- Email contacts.
