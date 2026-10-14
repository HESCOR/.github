# HESCOR — Human & Earth System Coupled Research

HESCOR (Human & Earth System Coupled Research) is an interdisciplinary research initiative at the **University of Cologne** that brings together Earth system science, human system modelling, and the humanities to study how interactions between **nature and culture** have shaped—and continue to shape—our world.

- Project website archive: https://hescor.github.io/
- Original project website: https://www.hescor-project.com/
- Bluesky: https://bsky.app/profile/hescor.bsky.social

---

## What we do

HESCOR combines paleoclimate/environmental reconstructions, archaeological evidence, and modern computational methods (including machine learning) to address questions such as:

- How have climatic shifts influenced human cultural evolution?
- How do human decisions and societal change impact the Earth system?
- How can computational tools help unlock the past?

The research network is structured around **ten thematic Work Packages (WPs)** spanning theory, climate modelling, dispersal/network approaches, archaeological databases, and ML-based cultural analyses.

---

## Repositories

This GitHub organization serves as a **curated entry point** to HESCOR-related code and infrastructure.

> Important: Many research outputs are intentionally hosted in **member-owned repositories** (to keep ownership, governance, and long-term URLs stable).  
> This list is here to improve visibility and discovery.

### Research software

- **ArcheoGra.jl** — Julia package for reconstructing prehistoric mobility networks from archaeological sites and calculating least-cost paths on topographic data using adaptive wavelet methods and an adaptive Dijkstra’s algorithm.\
  Repo: https://github.com/MaxBrockm/ArcheoGra.jl

- **AdvDiffMetricGraphs.jl** — Julia package for solving diffusion-reaction and advection-diffusion equations on metric graphs, including geometric multigrid solvers for modelling migration dynamics.\
  Repo: https://github.com/MaxBrockm/AdvDiffMetricGraphs.jl

- **PaleoVeg** — Python package for paleovegetation reconstruction (predicting vegetation/biome types from bioclimatic variables; includes optional C3/C4 competition corrections).  
  Repo: https://github.com/roink/PaleoVeg

- **Green Wave** — Research codebase for reconstructing vegetation phenology and “green waves” using satellite vegetation indices (e.g., NDVI), orbital/insolation forcing, and paleoclimate reconstructions, with links to questions around human mobility and settlement dynamics.  
  Repo: https://github.com/roink/green_wave

- **HEP-Model (Human Existence Potential Model)** — Research code for estimating spatially explicit human existence potential maps from archaeological presence/absence data and BioClim climate variables using a logistic-regression framework, with applications to questions of human dispersal and settlement dynamics.  
  Repo: https://github.com/ChrisWege/HumanExistencePotential

### Data infrastructure

- **ckan-docker (HESCOR fork)** — Docker Compose-based CKAN deployment setup, used as the basis for our CKAN-backed data portal/database work.  
  Repo: https://github.com/roink/ckan-docker

- **ckanext-scheming (HESCOR fork)** — CKAN extension for configuring and sharing custom metadata schemas in YAML or JSON, with support for custom validation and metadata editing and display templates.\
  Repo: https://github.com/roink/ckanext-scheming

### Project tools

- **Palaeo-landscape Explorer** — Interactive visualisations of palaeo-landscapes, research bias, and Human Existence Potential, developed for public outreach and science communication as part of the HESCOR Virtual Exhibition.\
  Repo: https://github.com/HESCOR/palaeo-landscape-explorer

- **HEP Explorer** — Interactive exploration of Human Existence Potential across Europe, developed for public outreach and science communication as part of the HESCOR Virtual Exhibition.\
  Repo: https://github.com/HESCOR/hep-explorer

- **HESCOR project website archive** — Long-term static archive of the public HESCOR WordPress website, including its educational material and interactive H5P content. Website: https://hescor.github.io/ · Repo: https://github.com/HESCOR/HESCOR.github.io

- **HESCOR Data Learning Lab (data-detective)** — Interactive browser-based educational games for research communication and public outreach, teaching data quality, variable types, and research data management. Available as a website and as downloadable H5P packages.\
  Repo: https://github.com/roink/data-detective

- **survey123_to_pdf** — Command-line workflow to turn a Survey123 CSV export into per-response A4 PDF summaries (grouping repeated blocks and skipping unanswered questions).  
  Repo: https://github.com/roink/survey123_to_pdf

---

## Contact & updates

The archived project website is the long-term hub for project information, publications, and educational material:

https://hescor.github.io/
