# What is the CBP Project (CarusoBasilePeptides)

**CBP (CarusoBasilePeptides)** is a set of *designed peptide libraries* intended to (i) **compete for Cu(II)** binding and (ii) **modulate Aβ (amyloid-β) conformational equilibria**, with the longer-term goal of promoting conformational states that are less compatible with oligomerization.

This repository (**CBP_series**) is the **main hub**: it hosts the mapping tables and global documentation. Family-specific structural ensembles are stored in dedicated sub-repositories.

---

## Scientific rationale (high-level)
The aggregation pathway of amyloid-β (Aβ) is strongly influenced by:
- **metal coordination** (especially Cu(II), but also other metal ions in some contexts),
- **electrostatics and ionic strength**,
- **secondary-structure equilibria** (disordered ↔ β-prone ↔ helical conformers).

CBP libraries are designed to:
1. Provide **high-affinity Cu(II) competitors** (relative to Aβ),
2. Shift the conformational balance of Aβ (directly or indirectly) toward states less prone to aggregation,
3. Offer a modular space of candidates that can be screened computationally and experimentally.

> Note: the exact mechanistic hypothesis and downstream experimental validation are intentionally kept modular, so the project can accommodate multiple testable routes (binding competition, conformational templating, electrostatic modulation, etc.).

---

## Repository structure (where things live)

### Main hub (this repo)
**CBP_series** contains:
- Global documentation and design notes
- **Mapping tables** that describe the peptide library and its metadata:
  - `CBP_mapping.csv`
  - `CBP_mapping_enriched.csv`
- Any cross-family analyses (when present)

### Family repositories (structural ensembles)
Family-specific repositories contain the structural outputs and notes for each sub-library:
- **CBP_alphas** → https://github.com/pepmirko/CBP_alphas
- **CBP_betas**  → https://github.com/pepmirko/CBP_betas
- **CBP_gammas** → https://github.com/pepmirko/CBP_gammas
- **CBP_deltas** → https://github.com/pepmirko/CBP_deltas

**Reference conditions (unless otherwise stated):**
- Structures computed with **PEP-FOLD4**
- **pH 7.5**
- **Ionic strength: 10 mM**

---

## Data conventions
### IDs and naming
- Peptides are identified consistently across CSV tables and family repositories.
- File naming aims to preserve a stable mapping between:
  - peptide identifier (ID / code),
  - family membership (alpha/beta/gamma/delta),
  - structural models (e.g., ranked outputs / multiple conformers).

### What the CSVs represent
- `CBP_mapping.csv`:
  - minimal mapping needed to connect peptide IDs to sequences and families.
- `CBP_mapping_enriched.csv`:
  - extended metadata (design descriptors, annotations, or computed fields), when available.

> If additional columns are introduced over time, the enriched table is the preferred location to avoid breaking downstream parsers.

---

## How to navigate the project
1. Start from **CBP_series** to understand the library structure and identifiers.
2. Use the **mapping tables** to locate the peptide/family you need.
3. Jump to the corresponding **family repository** to retrieve structural ensembles (PDBs) and family-specific notes.
4. If you are doing analysis across families, keep scripts/notebooks here in the main hub.

---

## Versioning and reproducibility
- Changes to peptide definitions or mapping tables should be tracked via commits.
- When structural ensembles are updated (re-runs / different settings), the family repository should:
  - document the computational settings,
  - keep prior versions clearly tagged or archived (e.g., release assets), when relevant.

---

## Citation and reuse
If you reuse or build on this project:
- Cite the repository (or the associated manuscript, if/when available).
- Retain the peptide IDs and mapping structure to maintain traceability.

Suggested citation (placeholder):
> CarusoBasilePeptides (CBP project), pepmirko GitHub repositories, accessed YYYY-MM-DD.

---

## Contact / ownership
Project owner: **pepmirko**  
For questions, open an Issue in the main hub repo (**CBP_series**) so discussions stay centralized.
