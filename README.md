# SPU IO Psychology — R for Statistics Knowledge Base

> **A shared archive of R code, analysis files, and project templates for graduate students in the Department of Industrial & Organizational Psychology at SPU.**

---

## 📖 How to Use This Repository

You do **not** need to know Git to use this repository. You can browse all files directly in your browser:

- Click any folder below to see what's inside
- Click any `.Rmd` file to read it in your browser
- Click the green **Code** button → **Download ZIP** to get everything at once

If you want to **contribute** files (add your project after dissertation defense), see the [Contributing Guide](CONTRIBUTING.md).

---

## 🖥️ Working Locally in RStudio

If you download the repository and want to run `.Rmd` files on your own computer, follow these two steps to make sure file paths work correctly.

**Step 1: Open the project file first.**
The repo includes an `.Rproj` file in its root folder. Always open this file in RStudio before opening any `.Rmd` — double-click it in your file browser, or use File → Open Project in RStudio. This sets the working directory to the repo root automatically.

**Step 2: Use `here()` for all file paths in your Rmd.**
All `.Rmd` files in this repo use the [`here` package](https://here.r-lib.org/) to handle file paths. Instead of hardcoded paths like `"C:/Users/YourName/Downloads/data.csv"`, paths are written like:

```r
library(here)
df <- read.csv(here("02_datasets", "your-data.csv"))
```

`here()` always builds paths relative to the repo root (where the `.Rproj` file lives), so the same code works on any computer regardless of where the repo is saved. If you open an `.Rmd` directly without opening the `.Rproj` first, `here()` may not anchor correctly and paths will break.

> **In short:** `.Rproj` first, then open your `.Rmd`.

---

## 📁 Repository Structure

```
/
├── io-psych-r4statistics.Rproj          # ← Open this first in RStudio
├── 00_stats-class-tutorials/     # Rmd files from first-year stats courses
├── 01_project-archive/           # Past student projects (anonymized)
│   ├── template/                 # Blank project submission template
│   └── [project folders]/        # One folder per contributed project
├── 02_datasets/                  # Shared/practice datasets (.csv, .sav)
├── 03_resources/                 # Cheat sheets, guides, helpful links
└── CONTRIBUTING.md               # How to add your own project
```

---

## 00 — Stats Class Tutorials

R Markdown files from the first-year statistics sequence. These are the canonical reference files for core statistical methods taught in the program.

| File | Topic |
|------|-------|
| *(Add your tutorial files here)* | |

---

## 01 — Project Archive

Anonymized Rmd files and datasets from past student research projects. Each project folder follows a standard structure:

```
01_project-archive/your-project-name/
├── README.md          # Brief description of the project & analysis
├── analysis.Rmd       # The main analysis file
├── data/              # Dataset(s) used (if shareable)
└── output/            # Rendered HTML or PDF output (optional)
```

### Contributed Projects

| Project | Primary Method | Contributor | Year |
|---------|---------------|-------------|------|
| *(Projects will appear here as students contribute)* | | | |

---

## 02 — Datasets

Shared datasets for practice or reuse across projects.

| Dataset | Description | Source |
|---------|-------------|--------|
| *(Datasets will be added here)* | | |

---

## 03 — Resources

| Resource | Description |
|----------|-------------|
| *(Cheat sheets, links, and guides will be added here)* | |

---

## 🔍 Finding What You Need

**"I need to remember how to run a specific test"** → Start in `00_stats-class-tutorials/`

**"Someone in my cohort did something similar to my dissertation"** → Browse `01_project-archive/`

**"I need a dataset to practice with"** → Check `02_datasets/`

**"I want to see how to structure my analysis file"** → See `01_project-archive/template/`

**"File paths in the Rmd aren't working"** → Make sure you opened `io-psych-r4statistics.Rproj` first, before the `.Rmd`

---

## ✏️ Contributing Your Project

After your dissertation defense, consider contributing your anonymized analysis files — your future cohort will thank you. See [CONTRIBUTING.md](CONTRIBUTING.md) for step-by-step instructions (no prior Git experience needed).

---

## Questions or Issues?

Open an [Issue](../../issues) on GitHub, or contact the repository maintainer.
