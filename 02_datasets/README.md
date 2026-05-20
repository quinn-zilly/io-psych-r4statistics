# 02 — Shared Datasets

This folder contains datasets that are reusable across multiple projects — practice data, publicly available data, or datasets referenced in more than one analysis.

**Tutorial-specific datasets** (used only by one tutorial file) live alongside their tutorial in `00_stats-class-tutorials/`, not here. This folder is for anything you'd reach for across different projects.

---

## What Belongs Here

- Practice datasets useful for teaching or exploring methods
- Datasets referenced by more than one project or tutorial
- Publicly available datasets relevant to IO psychology research

## What Does Not Belong Here

- Data tied to a single tutorial (those live in `00_stats-class-tutorials/.../data/`)
- Identified or potentially re-identifiable participant data
- Raw data that hasn't been checked for sharing permissions

---

## Using These Datasets

Load any file here from an `.Rmd` using `here()`:

```r
library(here)
df <- read.csv(here("02_datasets", "your-file.csv"))
```

Make sure you've opened `io-psych-r4statistics.Rproj` first so `here()` anchors to the repo root.

---

## Datasets

| File | Description | Source |
|------|-------------|--------|
| *(Datasets will be added here)* | | |
