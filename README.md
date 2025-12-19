# HESCOR GitHub Quickstart

This guide describes the **minimal “publishable” research-code repository** for HESCOR (README + LICENSE + CITATION), and a set of **nice-to-haves** that improve reuse and discoverability.

---

## Minimal “publishable” repository (required)

### 1) README.md (required)
**Must-have (minimum)**
- **What does this repo do (and for whom)?**
  - 1–3 sentences are enough.

**Nice-to-have (recommended)**
- **What was it used for?** (paper/project, analysis goal, method context)
- **Quick start:** how to install/run it (or where the docs are)
- **Expected input/output** (for code/data)
- **Current status** (prototype / stable / archived, etc.)

---

### 2) LICENSE / LICENSE.md (required)
Add an explicit license so others know what is allowed.

**Minimum requirement**
- Add a file named `LICENSE` (or `LICENSE.md`)

Common choices depend on your intent (e.g., MIT for code, CC-BY-4.0 for text/data). If you’re unsure, ask for guidance.

---

### 3) CITATION.cff (required)
Add a `CITATION.cff` file to the **root** of your repo so GitHub shows a **“Cite this repository”** UI.

**Minimal example**
```yaml
cff-version: 1.2.0
message: "If you use this software, please cite it as below."
title: "YOUR PROJECT TITLE"
type: software
authors:
  - family-names: "LastName"
    given-names: "FirstName"
    orcid: "https://orcid.org/0000-0000-0000-0000"
version: 0.1.0
date-released: 2025-12-17
doi: 10.5281/zenodo.XXXXXXX
````

---

## Rule of thumb

If someone can **install, run one example, and cite it**, it is already a win.

---

## Nice-to-haves (recommended, not required)

### A) Releases + Zenodo DOI

* Create versioned releases (`v0.1`, `v1.0`, …)
* If connected to Zenodo, each GitHub Release is typically archived and can get a DOI

**Concept DOI vs Version DOI**

* **Version DOI** = one specific release
* **Concept DOI** = represents all versions (stable “software as a whole” DOI)

**Metadata note**
If you have both `.zenodo.json` and `CITATION.cff`, Zenodo will use `.zenodo.json` for its archiving metadata.

---

### B) Dependencies file

Include at least one:

* `requirements.txt`, `environment.yml`, `pyproject.toml`, `renv.lock`, etc.

---

### C) Data note

* What data is needed?
* Where to get it?
* Any access restrictions / ethics notes?

---

### D) Example config + tiny toy dataset

* A minimal runnable example is often more valuable than long prose.

---

### E) GitHub topics (include `hescor`)

Topics improve discoverability and grouping.

1. Open your repo on GitHub
2. Right sidebar → **About**
3. Gear icon → add topics (include **hescor**) → Save

**Nice-to-have minimum**

* `hescor`

**Suggested topics (pick what fits)**
Domains: `archaeology`, `paleoclimate`, `paleovegetation`, `remote-sensing`, `phenology`, `geospatial`, `machine-learning`
Languages: `python`, `r`, `julia`, …

---

### F) Add the HESCOR badge to your README

```md
[![GitHub Org](https://img.shields.io/badge/GitHub-HESCOR-blue?logo=github&logoColor=white)](https://github.com/HESCOR)
```

---

### G) Add your repo to the HESCOR org overview list

GitHub orgs only list **org-owned** repos in the Repositories tab. To also feature **member-owned** repos, we curate the org **Overview** page using:

* `HESCOR/.github` → `profile/README.md`

**How to add your repository**

1. Open a PR: `https://github.com/HESCOR/.github`
2. Edit: `profile/README.md`
3. Add a bullet under the right section (Research software / Infrastructure / Tools)
4. Include: repo link + 1–2 sentences + DOI (if applicable)

**Template bullet**

```md
- [OWNER/REPO](https://github.com/OWNER/REPO) — One-sentence description. (Language) (License) (DOI if available)
```

---

## Checklist

### Required

* [ ] `README.md` contains at least: **what the repo does**
* [ ] License file present (`LICENSE` or `LICENSE.md`)
* [ ] `CITATION.cff` present

### Nice-to-have

* [ ] README also includes: what it was used for + quick start + inputs/outputs + status
* [ ] Dependencies file present
* [ ] Data note present
* [ ] Example config + toy dataset
* [ ] Releases used; Zenodo connected (if DOI desired)
* [ ] Topics set (includes `hescor`)
* [ ] HESCOR badge added
* [ ] Repo listed on HESCOR org overview page
* [ ] Repo is public (if possible)

