# CBP Peptide Library — Cu(II) capture & Aβ helix-modulation

This repository tracks a curated library of **designed peptides** intended to:
1) **compete for Cu(II)** (Cu sequestration away from Aβ)  
2) **modulate Aβ conformational equilibria**, with special interest in shifting populations away from β-prone states and toward **α-helical** character when possible.

The library is organized for **high interpretability**: clean baselines, clamp variants, and mechanistic controls.
## What’s in this repo

### Core documents
- **`consideration.md`** — *source-of-truth human document*:  
  - complete peptide list, ordered by **family → length**
  - design rationale per family
  - peptide-specific notes and caveats
- **`CBP_mapping.csv`** — *machine-readable index*:  
  - CBP name ↔ legacy IDs ↔ sequence ↔ length ↔ family ↔ role

> If you only read one file, read **`consideration.md`**.

---

## Naming scheme (CBPα1, CBPβ3, …)

Peptides are named using the convention:

**`CBP{GreekLetter}{index}`**

- The **Greek letter encodes the design family**.
- The **index increases with peptide length within that family** (short → long).

This is deliberate: it makes it easy to compare within-family length effects and avoids mixing fundamentally different design levers.

---

## Families (high-level)

Exact membership is defined in `consideration.md`.

- **Family α** — **ATCUN baselines**  
  Minimal-confounder Cu(II) capture designs (DAH/GGH heads), no internal clamp.

- **Family β** — **ATCUN + internal HxxxH clamp**  
  Cu(II) capture plus an embedded **i,i+4 His clamp** (e.g., HAAAH/HRAAH/HQAAH) for helix locking / secondary metal-contact patch.

- **Family γ** — **ATCUN-dead controls (N-acetylated)**  
  Same scaffold/clamp features, but **N-acetylation disables ATCUN-like binding** to isolate mechanism.

- **Family δ** — **Charged interaction comparators**  
  Higher electrostatic encounter rate with Aβ (use as “stress tests” and interpret only relative to α/β baselines).

---

## Practical guidance (how to use the library)

### Minimal recommended readouts
For each peptide (apo and Cu-bound) and for competition systems (Aβ + Cu + peptide), the recommended minimum is:

1. **Helicity (DSSP)** — time series + per-residue helix propensity  
2. **Cu coordination stability** — Cu–donor distances, coordination numbers, geometry metrics  
3. **Cu exposure** — SASA around Cu center (reactivity proxy)  
4. **Aβ–peptide contacts** — contact maps + residence times  
5. **Self-association** — peptide–peptide contacts (especially for long/charged constructs)  
6. If feasible: **Cu transfer thermodynamics** (ΔG_exchange) for  
   `Aβ–Cu + peptide → Aβ + peptide–Cu`

### Controls are non-negotiable
- **N-acetylated (γ-family) peptides** are required to separate “ATCUN Cu capture” from “scaffold/clamp binding”.
- Always benchmark interaction-prone peptides (δ-family) against α/β families before interpreting any “α-induction” effects.

---

## Repository index (families)

This repository is the **main hub** of the CBP project (library + mapping tables).
The four family-specific repositories below contain the corresponding structural ensembles.

> Reference conditions (unless otherwise stated): PEP-FOLD4, pH 7.5, ionic strength 10 mM.

### Families (sub-repositories)

- **CBP_alphas** → https://github.com/pepmirko/CBP_alphas  
  PEP-FOLD4 computed structures for the **alpha** family.

- **CBP_betas** → https://github.com/pepmirko/CBP_betas  
  PEP-FOLD4 computed structures for the **beta** family.

- **CBP_gammas** → https://github.com/pepmirko/CBP_gammas  
  PEP-FOLD4 computed structures for the **gamma** family.

- **CBP_deltas** → https://github.com/pepmirko/CBP_deltas  
  PEP-FOLD4 computed structures for the **delta** family.

---

## Adding or modifying peptides

**Rule 1 — Update the machine index first**  
Add new entries to `CBP_mapping.csv` (or your upstream CSV if you regenerate it), including:
- sequence (with `Ac-` prefix if N-acetylated),
- intended role,
- family assignment rationale.

**Rule 2 — Then update `consideration.md`**  
- ensure the peptide appears in the correct family,
- keep **length ordering** within family,
- add a short peptide-specific note if it introduces a new lever.

**Rule 3 — Avoid premature complexity**
- Prefer canonical amino acids first.
- Introduce non-canonical caps/staples only after the baseline mechanism is demonstrated.

---

## License / citation
If this library is used in a manuscript or report, please cite the relevant primary literature motivating:
- ATCUN-like Cu(II) binding motifs,
- i,i+4 metal-assisted helix stabilization,
- helix capping strategies,
- and metal-triggered helix nucleation concepts (where applicable).

(Repository-specific citation guidance can be added here once finalized.)

---

