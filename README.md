# Sergei Mikhalishchev - Academic Website

A clean, static academic website ready for GitHub Pages.

## Quick Setup for GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click the **+** button → **New repository**
3. Name it: `yourusername.github.io` (for your main site) OR any name like `website`
4. Make it **Public**
5. Click **Create repository**

### Step 2: Upload These Files

**Option A: Using GitHub Web Interface (Easiest)**
1. In your new repository, click **"uploading an existing file"** or **Add file → Upload files**
2. Drag and drop ALL files from this folder
3. Click **Commit changes**

**Option B: Using Git Command Line**
```bash
cd path/to/this/folder
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/REPONAME.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**
6. Wait 1-2 minutes — your site will be live at `https://yourusername.github.io/`

### Step 4: (Optional) Custom Domain

To use `mikhalishchev.online`:

1. In GitHub Pages settings, enter `mikhalishchev.online` in "Custom domain"
2. Update your domain's DNS settings:
   - Add a **CNAME** record: `www` → `yourusername.github.io`
   - Add **A** records pointing to GitHub's IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
3. Check "Enforce HTTPS" once DNS propagates

---

## Files You Need to Add

### Required: Your Photo
- Save your headshot as `assets/photo.jpg`
- The homepage expects this file

### Required: Your Paper PDFs
Add these to `assets/papers/`:
- `inattentionsimplicityreluctance.pdf`
- `etf.pdf`
- `Quotas.pdf`

(Or update the links in `research.html` to point to external URLs like SSRN)

---

## File Structure

```
website/
├── index.html          # Homepage
├── research.html       # Research papers
├── cv.html             # CV page
├── teaching.html       # Teaching experience
├── contact.html        # Contact info
├── about.html          # About me
├── assets/
│   ├── style.css       # Stylesheet
│   ├── CV_SM.pdf       # Your CV
│   ├── photo.jpg       # ADD YOUR PHOTO
│   └── papers/         # ADD YOUR PAPER PDFs
└── README.md           # This file
```

---

## Customization

- **Colors**: Edit `assets/style.css` — look for `:root` variables at the top
- **Content**: Edit the HTML files directly — they're simple and readable
- **Add pages**: Copy any HTML file as a template, update nav in all files

---

## Questions?

The site is pure HTML/CSS — no build steps, no dependencies. Just upload and it works!
