# HESCOR GitHub Quickstart

This guide explains how we keep the **repository list** on the HESCOR GitHub organization page up to date without transferring ownership of individual repos, and what you should add to your own repo to improve visibility and citability.

---

## 1) How the “repo list” on https://github.com/HESCOR works

GitHub organizations only show org-owned repositories in the built-in **Repositories** tab.

To also feature **member-owned repositories** (personal/group repos), we maintain a curated list on the organization **Overview** page via an **organization profile README**:

- The list lives in: `HESCOR/.github` → `profile/README.md`

That README is rendered on the organization’s Overview page and acts as our “project landing page”.

### Add your repository to the HESCOR list
1. Open a PR against: `https://github.com/HESCOR/.github`
2. Edit: `profile/README.md`
3. Add a new bullet under the right section (Research software / Infrastructure / Tools).
4. Include:
   - Repo link
   - 1–2 sentence description (what it does, for whom)
   - DOI (if applicable)

**Template bullet:**
```md
- [OWNER/REPO](https://github.com/OWNER/REPO) — One-sentence description. (Language) (License) (DOI if available)
```

---

## 2) Add the HESCOR badge to your README

Add this badge near the top of your `README.md`:

```md
[![GitHub Org](https://img.shields.io/badge/GitHub-HESCOR-blue?logo=github&logoColor=white)](https://github.com/HESCOR)
```

---

## 3) Add topics (please include `hescor`)

Topics make repos easier to discover and group.

1. Open your repository on GitHub
2. In the right sidebar, find **About**
3. Click the **gear icon**
4. Add topics (include **hescor**), then **Save changes**

### Minimum requirement
Add the topic:
- `hescor`

### Suggested topics (pick what fits your repo)
**Domains**
- `archaeology`
- `paleoclimate`
- `paleovegetation`
- `remote-sensing`
- `phenology`
- `geospatial`
- `machine-learning`

**Languages**
- `python`, `r`, `julia`, etc.

---

## 4) Make your repo citable (CITATION.cff + Zenodo)

### A) Add `CITATION.cff` (recommended for all research outputs)
Create a `CITATION.cff` file in the **root** of your repo.

Why:
- GitHub will show a **“Cite this repository”** UI when `CITATION.cff` is present.

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
```

### B) Zenodo GitHub integration (DOIs from releases)
If your repo is connected to Zenodo via GitHub integration:
- Zenodo archives the repository and typically issues a **new DOI for each GitHub Release**.

**Concept DOI vs Version DOI (important)**
Zenodo uses:
- **Version DOI** for a specific release/version
- **Concept DOI** that represents *all versions* (useful as the stable DOI to cite “the software in general”)

**Metadata note**
If your repo contains both:
- `.zenodo.json` and
- `CITATION.cff`

then Zenodo will use **`.zenodo.json`** and ignore `CITATION.cff` *for the Zenodo archiving metadata*.  
(Keeping `CITATION.cff` is still useful because GitHub uses it for the citation UI.)

---

## 5) Add a license

Every public repo should include a license file so others know what they can do with your code/data.

### Minimum requirement
Add a file named:
- `LICENSE` (or `LICENSE.md`)

Pick a license that matches how you want others to reuse your work (common choices: MIT, CC-BY-4.0 ).

---

## 6) Final “ready to be listed” checklist

Before adding your repo to the org overview list:

- [ ] Repo is public (if possible)
- [ ] `README.md` explains what it is + how to run/use it
- [ ] HESCOR badge added to README
- [ ] Topics added (**includes `hescor`**)
- [ ] `CITATION.cff` added (and DOI included if you have one)
- [ ] Zenodo connected (if DOI is desired) and releases are used
- [ ] License file present (`LICENSE`)
