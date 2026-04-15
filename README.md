# 📚 CourseVault — Personal Course Organizer

A beautifully designed, multi-page personal academic organizer built with pure HTML & CSS. Deployed on GitHub Pages.

## 🌐 Live Demo

**https://YOUR-USERNAME.github.io/course-organizer/**

---

## 📁 Project Structure

```
course-organizer/
├── index.html              ← Home page
├── css/
│   └── styles.css          ← Single external stylesheet (all styling)
├── pages/
│   ├── my-courses.html     ← Course table with 7 sample entries
│   ├── add-course.html     ← Add course form
│   └── contact.html        ← Contact Us page with FAQ
└── README.md
```

## 🚀 Deploy to GitHub Pages (Step-by-Step)

### Method 1 — GitHub Web Interface (Easiest)

1. **Create a new GitHub repository**
   - Go to [github.com/new](https://github.com/new)
   - Name it: `course-organizer`
   - Set to **Public**
   - Click **Create repository**

2. **Upload your files**
   - On the new repo page, click **"uploading an existing file"**
   - Drag and drop ALL files/folders from this project
   - Make sure to preserve the folder structure (`css/`, `pages/`)
   - Commit with message: `Initial commit: CourseVault launch 🎓`

3. **Enable GitHub Pages**
   - Go to your repo → **Settings** tab
   - Scroll to **Pages** in the left sidebar
   - Under **Source**, select **Deploy from a branch**
   - Branch: `main` · Folder: `/ (root)`
   - Click **Save**

4. **Your site is live!** ✅
   - Wait ~60 seconds, then visit:
   - `https://YOUR-USERNAME.github.io/course-organizer/`

---

### Method 2 — GitHub CLI (Terminal)

```bash
# 1. Initialize git in this folder
git init
git add .
git commit -m "Initial commit: CourseVault 🎓"

# 2. Create repo on GitHub and push
gh repo create course-organizer --public --push --source=.

# 3. Enable Pages via CLI
gh api repos/:owner/course-organizer/pages \
  --method POST \
  -f source[branch]=main \
  -f source[path]=/

# 4. Your site will be live at:
echo "https://$(gh api user --jq .login).github.io/course-organizer/"
```

---

### Method 3 — Git Commands (Manual)

```bash
git init
git add .
git commit -m "feat: CourseVault personal course organizer"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/course-organizer.git
git push -u origin main
```
Then enable Pages in Settings → Pages → Source: `main` branch.

---

## ✨ Features

| Feature | Details |
|--------|---------|
| **4 Pages** | Home, My Courses, Add Course, Contact Us |
| **Semantic HTML** | `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>` |
| **External CSS only** | Single `css/styles.css` file |
| **Course Table** | 7 sample entries with filtering & search |
| **Full Form** | Course Name, Instructor, Credits, Notes + validation |
| **Responsive** | Mobile hamburger menu, fluid grid layout |
| **Hover Effects** | Cards lift, nav highlights, table row hover |
| **Transitions** | Smooth CSS transitions throughout |
| **Color Theme** | Academic Noir with Amber accents (`#e8a020`) |
| **Toast Notifications** | Form submit feedback |
| **Live Search/Filter** | Filter courses by name, status, department |
| **FAQ Accordion** | Interactive expand/collapse on Contact page |
| **GPA Ring** | SVG progress ring on Home page |
| **Progress Bar** | Form completion tracker on Add Course |

## 🎨 Design Tokens

```css
--accent:     #e8a020   /* Amber gold */
--bg-base:    #0f0f0f   /* Deep black */
--bg-card:    #1f1f1f   /* Card surface */
--text-primary: #f0ede8 /* Warm white */
--font-display: 'DM Serif Display'
--font-body:    'DM Sans'
```

## 📄 License

MIT — free to use, modify, and distribute.

---

*Built with ❤️ for students who want to own their academic journey.*
