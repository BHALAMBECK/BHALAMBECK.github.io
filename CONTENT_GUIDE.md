# 📸 Content Upload Guide

Welcome! This guide shows you **exactly** how to add your images, resume, and documents to your portfolio website.

## 🚀 Quick Start (3 Steps)

### Step 1: Add Your Resume
1. Save your resume as: `Ben_Halambeck_Resume.pdf`
2. Drop it in the `resume/` folder
3. The "📄 Resume" button will automatically work!

### Step 2: Add Project Images
1. Go to the `images/projects/` folder
2. Add these 3 images (use exact filenames):
   - `supersonic.jpg` - Your supersonic experiment photo
   - `femap-api.jpg` - FEMAP screenshot or diagram
   - `pizza-drone.jpg` - Optimization plots or drone concept
3. The images will automatically appear on your website!

### Step 3: Add Optional Documents (Optional)
1. Go to the `docs/` folder
2. Add any technical reports or papers you want to share
3. Update the project links in `index.html` (see below)

---

## 📁 Folder Structure

```
BHALAMBECK.github.io/
├── index.html                    ← Main website file
├── images/
│   ├── ben.jpeg                  ← Your headshot (already there!)
│   └── projects/
│       ├── supersonic.jpg        ← ADD THIS
│       ├── femap-api.jpg         ← ADD THIS
│       └── pizza-drone.jpg       ← ADD THIS
├── resume/
│   └── Ben_Halambeck_Resume.pdf  ← ADD THIS
├── docs/                         ← ADD REPORTS HERE (optional)
└── CONTENT_GUIDE.md              ← You are here!
```

---

## 🎨 Image Guidelines

### Recommended Sizes
- **Project images**: 1200px × 800px (landscape)
- **Profile photo**: Already done! ✅
- **File format**: JPG or PNG
- **File size**: Keep under 500KB each

### Tips for Great Project Images
- **Supersonic project**: Photo of your test setup, schlieren imaging, or airfoil
- **FEMAP project**: Screenshot of the FEMAP interface with your scripts
- **Pizza-drone**: Your optimization charts, plots, or drone CAD model

---

## 🔗 Adding Project Links

Want to link to GitHub repos, papers, or demos? Here's how:

1. Open `index.html` in your code editor
2. Find the `siteData` object (around line 147)
3. Update the `links` section for each project:

```javascript
projects: [
  {
    title: "Supersonic Discrete-Normal Injection",
    // ... other fields ...
    links: { 
      demo: "#",                                    // ← Replace with video URL
      repo: "https://github.com/yourusername/...",  // ← Replace with GitHub
      paper: "docs/supersonic-report.pdf"           // ← Or local PDF
    }
  },
  // ... more projects
]
```

Replace `"#"` with actual URLs!

---

## 🎯 Common Tasks

### How to Update Your Contact Info
1. Open `index.html`
2. Find `siteData` (line ~147)
3. Update:
```javascript
email: "benjhalambeck@gmail.com",  // ← Your email
linkedin: "https://linkedin.com/in/benjaminhalambeck",  // ← Your LinkedIn
```

### How to Add a New Project
1. Open `index.html`
2. Find the `projects` array in `siteData`
3. Copy an existing project object and modify it:
```javascript
{
  title: "Your New Project",
  img: "images/projects/new-project.jpg",  // ← Add this image!
  alt: "Description of image",
  tags: ["Tag1", "Tag2"],
  blurb: "Short description...",
  details: [
    "Detail point 1",
    "Detail point 2"
  ],
  tech: ["Python", "MATLAB"],
  links: { repo: "#", demo: "#" }
}
```

### How to Update Skills
1. Open `index.html`
2. Find the `skills` array in `siteData`
3. Add/remove/edit skills:
```javascript
skills: [
  "Aerospace Design",
  "Your New Skill Here",  // ← Add here
  "Python"
]
```

---

## ✅ Checklist

Before you commit and push:

- [ ] Added resume: `resume/Ben_Halambeck_Resume.pdf`
- [ ] Added 3 project images to `images/projects/`
- [ ] Checked that image filenames match exactly
- [ ] Tested website locally (open `index.html` in browser)
- [ ] Updated any project links from `#` to real URLs
- [ ] (Optional) Added docs to `docs/` folder

---

## 🚀 Publishing Changes

Once you've added your files:

```bash
git add .
git commit -m "Add images, resume, and content updates"
git push origin main
```

Your site will update at: https://bhalambeck.github.io/

---

## 💡 Pro Tips

1. **Use descriptive alt text** - Good for accessibility and SEO
2. **Optimize images** - Use tools like TinyPNG to reduce file sizes
3. **Keep it updated** - Add new projects as you complete them
4. **Test locally first** - Open `index.html` in your browser before pushing

---

Need help? The code is well-commented in `index.html` - look for the `// ---------- Editable data ----------` section!

