# Contributing to the R Statistics Knowledge Base

Thank you for contributing! This guide walks you through two options: a simple web-based upload (no Git needed) and a full Git workflow for those who want to learn it.

---

## What to Contribute

After completing your dissertation analysis, consider sharing:

- Your **main analysis `.Rmd` file** (anonymized — remove participant identifiers)
- Your **dataset** (only if your IRB approval permits sharing, even in anonymized form)
- A short **README** describing your project, research question, and main methods used

You do **not** need to share results, the written dissertation, or any identifiable data.

---

## Option A: Upload via GitHub Website (No Git Required)

This is the easiest option.

1. **Create a free GitHub account** at [github.com](https://github.com) if you don't have one
2. **Navigate to this repository** in your browser
3. Go to `01_project-archive/` → click **Add file** → **Upload files**
4. Create a folder for your project by typing `your-project-name/` before your filename in the file name field
5. Upload your `.Rmd`, data file, and README
6. Scroll down, add a short description (e.g., "Adding dissertation project — mediation analysis"), and click **Propose changes**
7. Click **Create pull request** — a maintainer will review and merge it

---

## Option B: Git Workflow (Recommended if You Want to Learn Git)

### One-Time Setup

```bash
# 1. Install Git: https://git-scm.com/downloads
# 2. Configure your identity
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# 3. Fork this repo on GitHub (click "Fork" in the top right)
# 4. Clone your fork to your computer
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME
```

### Adding Your Project

```bash
# 1. Create a branch for your contribution
git checkout -b add-my-dissertation-project

# 2. Create your project folder (copy the template)
cp -r 01_project-archive/template 01_project-archive/your-project-name

# 3. Add your files to that folder
# Edit the README.md inside your folder to describe your project

# 4. Stage and commit your files
git add 01_project-archive/your-project-name/
git commit -m "Add dissertation project: [brief description of your study]"

# 5. Push to your fork
git push origin add-my-dissertation-project

# 6. Go to GitHub and open a Pull Request from your fork to this repo
```

---

## Project Folder Template

Your contribution should follow this structure:

```
01_project-archive/your-project-name/
├── README.md          ← Required: describe your project (see template below)
├── analysis.Rmd       ← Required: your main analysis file
├── data/              ← Optional: dataset(s), only if IRB-permissible
│   └── your-data.csv
└── output/            ← Optional: rendered HTML/PDF of the analysis
```

### README.md Template

```markdown
# [Brief Project Title]

## Overview
[1-3 sentences: what was the research question?]

## Methods Used
- [e.g., Confirmatory Factor Analysis]
- [e.g., Structural Equation Modeling]
- [e.g., Multilevel Modeling]

## Key R Packages
- [e.g., lavaan, lme4, psych]

## Notes for Future Students
[Anything you wish you'd known — tricky data issues, helpful resources, etc.]

## Year Completed
[e.g., 2024]
```

---

## Before You Submit: Anonymization Checklist

- [ ] Removed all participant names, IDs, or other direct identifiers from data files
- [ ] Removed or masked any file paths that reveal personal information (e.g., `C:/Users/YourName/...`)
- [ ] Confirmed your IRB approval permits data sharing (even anonymized)
- [ ] Replaced your name in the Rmd author field with something generic (e.g., "IO Psychology PhD Student") or removed it

---

## Questions?

Open an [Issue](../../issues) on GitHub and tag it `question`.
