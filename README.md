# Sandeep Singh - Academic Portfolio & Research Website

This repository contains the source code for the personal academic portfolio of **Sandeep Singh**, built with Jekyll and based on the [AcademicPages](https://academicpages.github.io/) template.

## Quick Setup & GitHub Pages Deployment

### 1. Repository Configuration
This website is configured to run on GitHub Pages. To publish:
1. Ensure the files in this folder are pushed to your GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initialize Sandeep Singh academic portfolio"
   git remote add origin https://github.com/SandeepSinghNk/SandeepSingh.github.io.git
   git branch -M main
   git push -u origin main
   ```
2. In your GitHub repository:
   * Go to **Settings** > **Pages**.
   * Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
   * Select branch `main` and folder `/ (root)`.
   * Click **Save**.

### 2. URL Customization
* If your repository is named `SandeepSinghNk.github.io` (matching your username), the site will serve at `https://sandeepsinghnk.github.io/`.
* If your repository remains `SandeepSingh.github.io`, set `baseurl: "/SandeepSingh.github.io"` inside `_config.yml`.

### 3. Local Development (Optional)
To test locally using Ruby:
```bash
bundle install
bundle exec jekyll serve
```
Open `http://localhost:4000` in your web browser.

---

## Research Projects Featured
* **Clinical ML Triage:** [Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Air Shed Ingestion:** Multi-state air quality and ERA5/FIRMS feature engineering across Northern India (126 CAAQMS stations).
