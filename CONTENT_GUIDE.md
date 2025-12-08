# 📸 Content Upload Guide

This guide tracks the content status for your portfolio website.

## ✅ Current Status: READY TO PUBLISH

**All core content has been added!** You can now publish your changes.

---

## 🚀 Quick Start (Completed)

### Step 1: Add Your Resume ✅
- [x] Saved resume as: `resume/Ben_Halambeck_Resume.pdf`
- [x] The "📄 Resume" button is active.

### Step 2: Add Project Images ✅
- [x] `supersonic.png` (Supersonic experiment)
- [x] `femap-api.png` (FEMAP API)
- [x] `pizza-drone.jpg` (Pizza drone optimization)
- **Note:** The code handles both `.jpg` and `.png` extensions automatically, but `index.html` is currently set to use the files above.

### Step 3: Add Documents ✅
- [x] `docs/` folder populated with reports and code samples.
- [x] Project links in `index.html` updated to point to these docs.

---

## 📁 Current Folder Structure

```
BHALAMBECK.github.io/
├── index.html                    ← Main website file (Updated with links)
├── images/
│   ├── ben.jpeg                  ← Profile photo
│   └── projects/
│       ├── supersonic.png        ✅ Added
│       ├── femap-api.png         ✅ Added
│       └── pizza-drone.jpg       ✅ Added
├── resume/
│   └── Ben_Halambeck_Resume.pdf  ✅ Added
├── docs/                         
│   ├── Experimental_...pdf       ✅ Added
│   ├── final report.pdf          ✅ Added
│   ├── matlab code 1.pdf         ✅ Added
│   └── matlab code 2.pdf         ✅ Added
└── CONTENT_GUIDE.md              ← You are here!
```

---

## 🎨 Image Guidelines

### Recommended Sizes
- **Project images**: 1200px × 800px (landscape)
- **File format**: JPG or PNG (Currently using a mix)
- **File size**: Keep under 500KB each

---

## 🔗 Project Links Configuration

Your `index.html` is currently configured with these links:

1. **Supersonic Project**
   - Demo: YouTube Video
   - Paper: `docs/Experimental_Investigation_of_Discrete_Normal_Injection_for_Supersonic_Wing_Circulation_Control.pdf`

2. **FEMAP API**
   - (No external links configured currently - consider adding GitHub repo if public)

3. **Pizza-Drone Optimization**
   - Report: `docs/final report.pdf`
   - Code: `docs/matlab code 1.pdf` & `2.pdf`

---

## 🎯 Maintenance Tasks

### How to Update Your Contact Info
1. Open `index.html`
2. Find `siteData` (line ~187)
3. Update `email` or `linkedin` fields.

### How to Add a New Project
1. Open `index.html`
2. Find the `projects` array in `siteData`
3. Copy an existing project object and modify it.

### How to Update Skills
1. Open `index.html`
2. Find `skillCategories` in `siteData`
3. Add/remove/edit skills in the lists.

---

## ✅ Final Checklist

Before you push changes:

- [x] Added resume: `resume/Ben_Halambeck_Resume.pdf`
- [x] Added 3 project images to `images/projects/`
- [x] Checked that image filenames match `index.html`
- [x] Tested website locally (open `index.html` in browser)
- [x] Updated project links to point to `docs/`
- [x] Added reports to `docs/` folder

---

## 🚀 Publishing Changes

You are ready to go! Run these commands in your terminal:

```bash
git add .
git commit -m "Update content guide and verify assets"
git push origin main
```

Your site will update at: https://bhalambeck.github.io/
