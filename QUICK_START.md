# 🚀 Quick Start Guide

## Your Website is Ready!

Your portfolio website has been enhanced with professional features and is ready for your content. Here's what's been added:

### ✨ New Features

1. **📸 Smart Image Handling**
   - Automatic fallback to placeholder SVGs until you add real images
   - Just drop your JPG images in `images/projects/` and they'll work instantly!

2. **📄 Working Resume Button**
   - Add `Ben_Halambeck_Resume.pdf` to the `resume/` folder
   - The button will automatically link to it

3. **🎨 Categorized Skills**
   - Skills are now grouped by: Aerospace & Engineering, Programming & Tools, Analytics & Optimization
   - Easy to customize in the `siteData` object

4. **✉️ Contact Form**
   - Functional contact form that opens email client
   - Option to upgrade to Formspree for direct submissions

5. **⏱️ Visual Timeline**
   - Your experience section now has a beautiful timeline with dots and gradient line

6. **🔍 SEO & Social Sharing**
   - Proper meta tags for social media previews
   - Optimized for search engines

---

## 🎯 Next Steps (3 Easy Tasks)

### Task 1: Add Your Images (5 minutes)
1. Navigate to `images/projects/` folder
2. Add these 3 images with **exact filenames**:
   ```
   supersonic.jpg       (your supersonic experiment photo)
   femap-api.jpg        (FEMAP screenshot or diagram)
   pizza-drone.jpg      (optimization plots or drone design)
   ```
3. That's it! The website will automatically use them.

**Image Tips:**
- Size: ~1200x800px (landscape orientation)
- Format: JPG or PNG
- Keep under 500KB each
- Use [TinyPNG](https://tinypng.com/) to compress if needed

---

### Task 2: Add Your Resume (1 minute)
1. Save your resume as exactly: `Ben_Halambeck_Resume.pdf`
2. Drop it in the `resume/` folder
3. The "📄 Resume" button will now work!

---

### Task 3: Update Project Links (5 minutes)
Open `index.html` and find the `siteData` section (around line 170). Update the `#` placeholders with real URLs:

```javascript
projects: [
  {
    title: "Supersonic Discrete-Normal Injection",
    // ...
    links: { 
      demo: "https://youtube.com/...",           // Video demo
      repo: "https://github.com/...",            // GitHub repo
      paper: "docs/supersonic-report.pdf"        // Or upload PDF to docs/
    }
  },
  // ... do the same for other projects
]
```

---

## 🧪 Test Your Website Locally

1. **Open in Browser**: Just double-click `index.html`
2. **Check Everything**:
   - ✅ Do your images show up?
   - ✅ Does the resume button download your PDF?
   - ✅ Do project links work?
   - ✅ Does the contact form open your email?

---

## 📤 Publish Your Changes

Once everything looks good:

```bash
# Make sure you're in the right directory
cd BHALAMBECK.github.io

# Add all your new files
git add .

# Commit with a descriptive message
git commit -m "Add images, resume, and professional enhancements"

# Push to GitHub
git push origin main
```

Your site will update at: **https://bhalambeck.github.io/** in ~1 minute!

---

## 🎨 Optional Customizations

### Add a New Project
Copy an existing project object in `siteData.projects` and modify:

```javascript
{
  title: "Your New Project",
  img: "images/projects/new-project.jpg",  // Add this image!
  alt: "Description",
  tags: ["Tag1", "Tag2"],
  blurb: "Brief description",
  details: [
    "Detail 1",
    "Detail 2"
  ],
  tech: ["Python", "MATLAB"],
  links: { repo: "#", demo: "#" }
}
```

### Update Skills
Edit the `skillCategories` in `siteData`:

```javascript
skillCategories: {
  "Aerospace & Engineering": ["Your", "Skills", "Here"],
  "Programming & Tools": ["Python", "MATLAB", "..."],
  "Analytics & Optimization": ["Data Viz", "ML", "..."]
}
```

### Change Colors
Find the `:root` variables in the `<style>` section (~line 13):

```css
:root{ 
  --brand:#c04a00;   /* Main brand color */
  --accent:#f4a261;  /* Accent/link color */
  /* ... more colors */
}
```

### Enable Formspree (Advanced)
For a real contact form without email client:
1. Sign up at [Formspree.io](https://formspree.io/) (free tier available)
2. Get your form endpoint
3. Uncomment the Formspree code in the contact form handler (~line 407)
4. Replace `YOUR_FORM_ID` with your actual ID

---

## 📂 Folder Structure

```
BHALAMBECK.github.io/
├── index.html              ← Main website (edit siteData here)
├── QUICK_START.md          ← You are here!
├── CONTENT_GUIDE.md        ← Detailed content guide
├── README.md               ← Original repo readme
│
├── images/
│   ├── ben.jpeg            ← Your headshot ✅
│   └── projects/
│       ├── supersonic.jpg  ← ADD THIS
│       ├── supersonic.svg  ← Placeholder (will auto-hide)
│       ├── femap-api.jpg   ← ADD THIS
│       ├── femap-api.svg   ← Placeholder (will auto-hide)
│       ├── pizza-drone.jpg ← ADD THIS
│       └── pizza-drone.svg ← Placeholder (will auto-hide)
│
├── resume/
│   └── Ben_Halambeck_Resume.pdf  ← ADD THIS
│
└── docs/                   ← Optional: technical reports
```

---

## 💡 Pro Tips

1. **Test Locally First**: Always open `index.html` in your browser before pushing
2. **Optimize Images**: Use tools like TinyPNG to reduce file sizes
3. **Keep It Updated**: Add new projects as you complete them
4. **Use Exact Filenames**: The website looks for specific filenames, so match them exactly
5. **Check Mobile**: Test how it looks on your phone too!

---

## ❓ Common Questions

**Q: The images don't show up on the live site**  
A: Make sure you committed and pushed them to GitHub. Check that filenames match exactly.

**Q: Resume button shows "disabled" style**  
A: The PDF filename must be exactly `Ben_Halambeck_Resume.pdf` in the `resume/` folder.

**Q: Can I use PNG instead of JPG?**  
A: Yes! The auto-fallback works with both `.jpg` and `.png` files.

**Q: How do I add more than 3 projects?**  
A: Copy a project object in `siteData.projects`, add your new project info, and add the corresponding image.

---

## 🎉 You're All Set!

Your portfolio is now:
- ✅ Professional and modern
- ✅ Easy to update (just drop images in folders)
- ✅ SEO optimized
- ✅ Mobile responsive
- ✅ Dark/light theme enabled
- ✅ Contact form ready

**Just add your 3 images and resume PDF, and you're ready to go!**

Need help? Check `CONTENT_GUIDE.md` for more detailed instructions.

