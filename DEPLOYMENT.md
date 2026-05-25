# Deployment Guide — PowerBI Stimulator Enterprise

This guide gives clear steps to deploy the unified enterprise edition using free static hosting.

The app is static. It does not require Node.js, Python, PHP, a paid database, or any AI API.

## Required Files

Deploy the complete `enterprise` folder. At minimum, these files must stay together:

```text
index.html
manifest.webmanifest
sw.js
assets/icon.svg
```

Recommended documentation files for GitHub:

```text
README.md
FEATURES.md
DEPLOYMENT.md
CHANGELOG.md
CONTRIBUTING.md
ABOUT_ADEWALE.md
ENTERPRISE_NOTES.md
SECURITY.md
PRIVACY.md
GOVERNANCE.md
LICENSE
```

## Cost and API Position

This platform does **not** use AI APIs because AI APIs are not cost-effective for this use case.

No OpenAI API.  
No Gemini API.  
No Claude API.  
No backend model endpoint.  
No paid Power BI Service dependency.  
No paid database.  

All insight generation is rule-based and local.

---

# Option 1 — Cloudflare Pages Recommended

Cloudflare Pages is recommended because Adewale already uses Cloudflare Pages for portfolio and HMG platforms.

## Steps

1. Create a GitHub repository. Suggested name:

   ```text
   powerbi-stimulator-enterprise
   ```

2. Upload all files from the `enterprise` folder to the root of the repository.

3. Confirm that this file is in the repository root:

   ```text
   index.html
   ```

4. Log in to Cloudflare Dashboard.
5. Go to **Workers & Pages**.
6. Click **Create application**.
7. Select **Pages**.
8. Select **Connect to Git**.
9. Choose the GitHub repository.
10. Configure build settings:

   ```text
   Framework preset: None
   Build command: leave blank
   Build output directory: /
   Root directory: /
   ```

11. Click **Save and Deploy**.
12. Wait for deployment to complete.
13. Open the generated URL, for example:

   ```text
   https://powerbi-stimulator-enterprise.pages.dev
   ```

14. Test the app:

   - Click **Sample**.
   - Click **Auto Report**.
   - Open **Enterprise Workspaces**.
   - Open **Semantic Model** and discover relationships.
   - Create an RLS role.
   - Run Refresh simulation.
   - Promote through Deployment Pipeline.
   - Publish App simulation.
   - Export Audit Log.
   - Backup project JSON.

15. On Android Chrome, open the browser menu and tap **Add to Home screen**.

---

# Option 2 — GitHub Pages

## Steps

1. Log in to GitHub.
2. Create a public repository named:

   ```text
   powerbi-stimulator-enterprise
   ```

3. Upload all files in the `enterprise` folder.
4. Open repository **Settings**.
5. Click **Pages**.
6. Under **Build and deployment**, choose:

   ```text
   Source: Deploy from a branch
   Branch: main
   Folder: / (root)
   ```

7. Click **Save**.
8. Wait for GitHub Pages to build the site.
9. Open the live URL. It will look like:

   ```text
   https://your-username.github.io/powerbi-stimulator-enterprise/
   ```

10. Test all major features.

## Optional GitHub Actions Deployment

A workflow is included at:

```text
.github/workflows/static-pages.yml
```

To use it:

1. Go to **Settings → Pages**.
2. Set Source to **GitHub Actions**.
3. Push to `main`.
4. Open the **Actions** tab and wait for deployment to finish.

---

# Option 3 — Netlify Drag-and-Drop

## Steps

1. Keep all enterprise files inside one folder.
2. Visit:

   ```text
   https://app.netlify.com/drop
   ```

3. Sign in or create a free account.
4. Drag the whole `enterprise` folder into Netlify Drop.
5. Wait for the generated site URL.
6. Open the URL and test the app.
7. Optional: go to **Site settings** and rename the site.

---

# Option 4 — Local Offline Use

## Steps

1. Copy the `enterprise` folder to your computer, phone or tablet.
2. Open `index.html` in Chrome, Edge or another modern browser.
3. Use CSV and JSON imports fully offline.
4. For XLSX import, open the hosted version online at least once so the browser can load the free SheetJS library, or convert Excel files to CSV.
5. Use **Backup** regularly to export your project JSON.

---

# PWA Installation

When deployed over HTTPS:

1. Open the live site in Chrome.
2. Click the browser menu.
3. Choose **Install app** or **Add to Home screen**.
4. The app will open like a mobile/desktop application.

---

# Verification Checklist

## Core BI

- Home page loads.
- Sample data loads.
- Data View previews datasets.
- Data Quality Auditor works.
- Auto Report creates report visuals.
- Pivot Matrix builds a matrix.
- Join Engine joins Sample Sales to Region Targets by `region`.
- Calculated Field creates `vat` using `round({{revenue}}*0.075,2)`.
- Backup downloads JSON.
- Restore imports JSON.

## Enterprise Features

- Workspaces page displays HMG Enterprise BI Workspace.
- Semantic Model detects relationship candidates.
- RLS role can be created and previewed.
- Lineage view shows Sources → Semantic Model → Reports → App → Consumers.
- Refresh Now adds audit activity.
- Deployment Pipeline promotes a package.
- App Publishing creates an enterprise app entry.
- Sharing adds a viewer.
- Admin Portal displays Adewale's profile and tenant settings.
- Audit CSV exports.
- Metric alert can be created and evaluated.
- Bookmark can save and restore a report state.
- Mobile layout preview renders report widgets.

---

# Security / Privacy

- Imported files are processed in the browser.
- The app does not upload user data to any server.
- Backups are downloaded by the user.
- Enterprise features are local simulations for governance training and demonstrations.
- No API key is required.

---

# Important Non-Affiliation Note

This is a Power BI-style enterprise simulator for educational and demonstration purposes. It is not an official Microsoft product and does not contain Microsoft proprietary source code.
