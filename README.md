# Sandeep Singh - Academic Portfolio & Research Website

This repository contains the source code for the personal academic portfolio of **Sandeep Singh** (`https://phdsandeepsingh.github.io`), built with Jekyll and based on the [AcademicPages](https://academicpages.github.io/) template.

## Quick Setup & GitHub Pages Deployment

### 1. Repository Configuration
This website is configured to run on GitHub Pages under `PhDSandeepSingh/PhDSandeepSingh.github.io`:
1. Push the committed files in this folder to your GitHub repository:
   ```bash
   git remote set-url origin https://github.com/PhDSandeepSingh/PhDSandeepSingh.github.io.git
   git branch -M main
   git push -u origin main
   ```
2. In your GitHub repository (`https://github.com/PhDSandeepSingh/PhDSandeepSingh.github.io`):
   * Go to **Settings** > **Pages**.
   * Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
   * Select branch `main` and folder `/ (root)`.
   * Click **Save**.

### 2. URL Configuration (`_config.yml`)
* **User Site (`PhDSandeepSingh/PhDSandeepSingh.github.io`):** Serves directly at `https://phdsandeepsingh.github.io/` with `baseurl: ""` (current default).
* **Project Site (if hosted under a different username, e.g., `SandeepSinghNk/PhDSandeepSingh.github.io`):** Change `baseurl` to `"/PhDSandeepSingh.github.io"` in `_config.yml`.

### 3. Skeleton Customization Checklist
When you are ready to personalize your details:
* **Profile Metadata & Social Links:** Edit the `author:` block in `_config.yml` (`employer`, `email`, `googlescholar`, `orcid`, `linkedin`, etc.).
* **Profile Headshot:** Add your photo to `images/profile.jpg` (and optionally `assets/images/profile.jpg`) and change `avatar: "profile.svg"` to `avatar: "profile.jpg"` in `_config.yml`.
* **Curriculum Vitae:** Edit the education, appointments, and awards placeholders in `_pages/cv.md`, and drop your PDF CV at `files/Sandeep_Singh_CV.pdf`.

### 4. Local Development (Optional)
To preview locally using Ruby:
```bash
bundle install
bundle exec jekyll serve
```
Open `http://localhost:4000` in your web browser.

---

## Research Projects Featured
* **Clinical ML Triage:** [Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Air Shed Ingestion:** Multi-state air quality and ERA5/FIRMS feature engineering across Northern India (126 CAAQMS stations).
