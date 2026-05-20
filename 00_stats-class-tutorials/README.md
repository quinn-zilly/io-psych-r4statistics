# 00 — Stats Class Tutorials

R Markdown tutorial files from the first-year statistics sequence. These are the canonical reference files for core statistical methods taught in the program.

Folders are organized by academic year and instructor so it's easy to find the version you were taught from.

---

## Using These Tutorials

1. Download the repository (green **Code** button → **Download ZIP**) or clone it
2. Open `io-psych-r4statistics.Rproj` in RStudio first
3. Open any `.Rmd` file — all file paths use `here()` and will work correctly as long as you opened the `.Rproj` first

---

## Contents

### 2025–2026 (Dr. Fossum)

**Statistics 1**

| File | Topic |
|------|-------|
| `R Basics.Rmd` | R fundamentals: objects, vectors, data frames, basic operations |
| `Data Cleaning.Rmd` | Importing, inspecting, and cleaning data |
| `Descriptive Statistics.Rmd` | Means, SDs, distributions, visualizations |
| `One Sample Tests.Rmd` | One-sample t-test, chi-square goodness of fit |
| `t Tests.Rmd` | Independent samples and paired t-tests |
| `One-Way ANOVA.Rmd` | One-way ANOVA with post-hoc tests |
| `Simple Linear Regression.Rmd` | Bivariate regression, assumptions, diagnostics |

**Statistics 2**

| File | Topic |
|------|-------|
| `Multiple Linear Regression.Rmd` | Multiple regression, model comparison |
| `Categorical Predictors.Rmd` | Dummy coding, contrast coding |
| `Hierarchical Regression.Rmd` | Blocked entry regression, R² change |
| `Moderation (continuous).Rmd` | Continuous × continuous interactions |
| `Moderation (categorical).Rmd` | Continuous × categorical interactions |
| `Mediation and Bootstrapping.Rmd` | Mediation with bootstrapped indirect effects |
| `Process_Walkthrough.Rmd` | Hayes PROCESS macro walkthrough |

---

## Adding Tutorials from Other Years

If you have tutorial files from a different year or instructor, contribute them by adding a new subfolder following the same pattern:

```
00_stats-class-tutorials/
└── YYYY-YYYY (Dr. LastName)/
    ├── Statistics 1/
    │   ├── tutorial.Rmd
    │   └── data/
    └── Statistics 2/
        ├── tutorial.Rmd
        └── data/
```

See [CONTRIBUTING.md](../CONTRIBUTING.md) for how to submit files.
