# Security Policy

## Security Model
PowerBI Stimulator Enterprise is a client-side static application. It does not send imported data to a backend server.

## What Is Protected
- Data is processed locally in the browser.
- Static security headers are included for compatible hosts.
- No API keys are required.
- No AI API calls are made.

## Limitations
- Client-side RBAC/RLS is a simulation, not production-grade enforcement.
- Anyone with access to the browser storage or exported workspace JSON can inspect local data.
- Public demos should use anonymised or sample data only.

## Recommended Use
- Use sample data for teaching.
- Anonymise sensitive records before import.
- Clear browser storage on shared devices.
- Use private repositories when storing non-public documentation.
