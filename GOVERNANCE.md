# Governance Guide

## Recommended Governance Workflow
1. Import only approved or anonymised data.
2. Open Data View and review the data dictionary.
3. Run the statistical profiler.
4. Add validation rules in Enterprise Center.
5. Save a workspace version before major changes.
6. Build the report.
7. Use RLS simulation to explain access boundaries.
8. Export the audit log and workspace backup when handing over.

## Suggested Validation Rules
- Required columns must be present.
- Missing values should be below a defined threshold.
- PII must be removed before classroom demos.
- Dataset source and owner must be known.
- Published report must include date and version.

## Production Disclaimer
This app is suitable for learning, demonstration, prototyping and lightweight local analysis. Production enterprise BI should use server-side authentication, governed data warehouses and formal compliance processes.
