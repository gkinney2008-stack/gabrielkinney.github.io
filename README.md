# 🚀 Gabriel Kinney Engineering Portfolio - GitHub Pages Deployment Guide

## Overview

Your engineering portfolio is a modern, responsive HTML/CSS website that showcases your projects, experience, and skills. This guide walks you through publishing it on GitHub Pages so it's accessible via URL.

---

## 📋 What's Included

### Files in `portfolio-website/`
- **index.html** - Main portfolio homepage with all projects
- **safe-step-well.html** - Detailed project page for Safe Step Well
- **piano-sequencer.html** - Polyphonic Piano & Sequencer project details
- **mousetrap-car.html** - Mousetrap Car Design project details  
- **pill-crusher.html** - Pill Crusher Tool project details
- **README.md** - This file

### Features
✅ Fully responsive design (works on mobile, tablet, desktop)  
✅ Fast loading (pure HTML/CSS, no dependencies)  
✅ Professional styling with custom color scheme  
✅ Navigation between portfolio and project pages  
✅ Contact section with email and social links  
✅ SEO-friendly structure  

---

## 🔧 Setup Instructions

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Complete the registration process

### Step 2: Create a New Repository
1. Log into GitHub
2. Click the **+** icon in top right → **New repository**
3. Name it: `gabrielkinney.github.io`
   - (Replace "gabrielkinney" with YOUR GitHub username)
   - This exact naming is required for GitHub Pages
4. Choose **Public** (required for GitHub Pages)
5. Click **Create repository**

### Step 3: Upload Your Portfolio Files

**Option A: Via GitHub Web Interface (Easiest)**
1. Open your new repository on GitHub
2. Click **Add file** → **Upload files**
3. Drag and drop all HTML files from the `portfolio-website/` folder
4. Add a commit message: "Initial portfolio upload"
5. Click **Commit changes**

**Option B: Via Git Command Line (For advanced users)**
```bash
cd /path/to/portfolio-website
git init
git add .
git commit -m "Initial portfolio upload"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/gabrielkinney.github.io.git
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Scroll down to **Pages** section
4. Under "Source", select **main** branch
5. Folder should be **/(root)**
6. Click **Save**

### Step 5: Verify Your Portfolio is Live
Wait 2-3 minutes, then visit: `https://gabrielkinney.github.io`

Your portfolio is now published! 🎉

---

## 📝 Customization

### Update Your Information
Edit `index.html` and project pages to customize:

**In index.html:**
- Line ~160: Update email address in contact section
- Line ~165: Update LinkedIn URL
- Line ~170: Update GitHub URL
- Line ~175: Update phone number

**Contact Information:**
```html
<a href="mailto:your-email@example.com" class="contact-link">
    <div class="contact-link-icon">📧</div>
    <div>Email</div>
    <small>your-email@example.com</small>
</a>
```

### Add New Project Pages
1. Copy one of the existing project HTML files (e.g., `safe-step-well.html`)
2. Update the title, content, and details
3. Add link in `index.html` projects section
4. Upload the new file to GitHub

### Change Colors & Styling
The color scheme uses CSS variables (top of each HTML file):
```css
:root {
    --primary-color: #003366;      /* Royal Blue */
    --accent-color: #00BCD4;       /* Cyan/Teal */
    --text-dark: #333333;
    --text-light: #666666;
    --bg-light: #f5f5f5;
    --white: #ffffff;
}
```

Change these values to customize the entire website's appearance.

---

## 🔄 Making Updates

### To update your portfolio:
1. Edit the HTML files locally
2. Test in your browser (just open the HTML file)
3. Upload changed files to GitHub:
   - Via web interface: Click **Add file** → **Upload files** → select updated files
   - Via Git: `git add .` → `git commit -m "Update"` → `git push`
4. Wait 30 seconds - GitHub Pages auto-updates

### To add new projects:
1. Create a new HTML file (copy from template)
2. Update content with project details
3. Add link in `index.html` projects grid:
```html
<div class="project-card">
    <div class="project-image">📱</div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <div class="project-meta">Category • Date</div>
        <p class="project-description">Project description...</p>
        <div class="project-tags">
            <span class="tag">Skill1</span>
            <span class="tag">Skill2</span>
        </div>
        <div class="project-links">
            <a href="your-project.html">View Details</a>
            <a href="#">Documentation</a>
        </div>
    </div>
</div>
```

---

## 📱 Mobile Responsiveness

The portfolio is fully responsive and looks great on:
- ✅ Desktop (1200px+)
- ✅ Tablet (768px-1199px)
- ✅ Mobile (320px-767px)

Test on your phone by visiting: `https://gabrielkinney.github.io`

---

## 🎯 Portfolio Structure

```
gabrielkinney.github.io/
│
├── index.html                    (Main portfolio page)
├── safe-step-well.html          (Project: Safe Step Well)
├── piano-sequencer.html         (Project: Polyphonic Piano)
├── mousetrap-car.html           (Project: Mousetrap Car)
├── pill-crusher.html            (Project: Pill Crusher)
└── README.md                    (This file)
```

---

## ✨ Features Included

### Homepage
- Hero section with CTA buttons
- About section with skills grid
- Featured projects grid (6 projects)
- Experience and leadership section
- Contact section with social links
- Footer with copyright

### Project Pages
- Project overview and hero section
- Technical specifications
- Design details and methodology
- Testing and validation results
- Learning outcomes
- Future work suggestions

---

## 🔐 Privacy & Security

- ✅ No backend server (100% static site)
- ✅ No database needed
- ✅ All data stored on GitHub (encrypted)
- ✅ GitHub Pages SSL certificate (HTTPS)
- ✅ No analytics tracking (unless you add it)

---

## 📊 Adding Analytics (Optional)

To track portfolio visits, add Google Analytics:

1. Create Google Analytics account at [google.com/analytics](https://google.com/analytics)
2. Get your Measurement ID (looks like: G-XXXXXXXXXX)
3. Add this to the `<head>` section of index.html (and other pages):
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🤝 Sharing Your Portfolio

Once live, share your portfolio URL:
- **Email:** Include link in resume footer
- **LinkedIn:** Add to profile URL
- **Social Media:** Tweet your portfolio launch
- **Job Applications:** Paste link in cover letters
- **Networking:** Share in professional networks

**Your Portfolio URL:** `https://gabrielkinney.github.io`

---

## 🐛 Troubleshooting

### Portfolio not showing after upload?
- Wait 2-3 minutes for GitHub Pages to build
- Hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac)
- Check Settings → Pages is enabled
- Ensure index.html is in root folder

### Links not working?
- Check file names are exact (case-sensitive)
- Ensure all HTML files are in same folder
- Test locally first by opening files in browser

### Styling looks off?
- Clear browser cache (Settings → Privacy)
- Try different browser
- Check CSS color values are valid hex codes

### Need to unpublish?
- Go to repository Settings → Pages → Source → Disable
- GitHub will keep your repo but won't serve the site

---

## 📚 Helpful Resources

- **GitHub Pages Docs:** [pages.github.com](https://pages.github.com)
- **HTML Reference:** [mdn.org/html](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **CSS Reference:** [mdn.org/css](https://developer.mozilla.org/en-US/docs/Web/CSS)
- **GitHub Desktop:** [desktop.github.com](https://desktop.github.com) (easier than command line)

---

## ✅ Quick Checklist

Before launching:
- [ ] All HTML files are in portfolio-website/ folder
- [ ] index.html opens correctly in browser
- [ ] All links work (test locally first)
- [ ] Contact email is correct
- [ ] GitHub repository is public
- [ ] GitHub Pages is enabled in Settings
- [ ] Repository is named `gabrielkinney.github.io`

---

## 🎉 You're Done!

Your professional engineering portfolio is now live on the internet! 

**Next Steps:**
1. Share your portfolio URL with potential employers
2. Add to your resume
3. Continue adding projects as you complete them
4. Update experience and skills as they grow

---

**Questions?** Refer to GitHub Pages documentation or reach out to GitHub Support.

**Happy sharing!** Your engineering work deserves to be seen by the world. 🚀

---

*Portfolio Created:* June 17, 2026  
*Last Updated:* June 17, 2026  
*Version:* 1.0
