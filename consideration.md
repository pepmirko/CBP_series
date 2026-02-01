# consideration.md — CBP library (family-based naming)

This file defines the **current peptide library** after:
1) removing previously discarded sequences (they are **not** listed here),
2) renaming peptides using the **CBP{GreekLetter}{index}** convention (family-based), and
3) ordering peptides **by family**, then **by length** within each family.

**Naming rule:** the Greek letter encodes the design family; the index increases with sequence length within that family.

## Library index (ordered by family and length)

## Family α — ATCUN baselines (no internal clamp; low-interaction regime)

- **CBPα1** *(was MG43; old internal ID MG70)*: `GGHEAAKEAAKEAAKLWKK`  
  **Length:** 19 aa; **N-terminus:** Free  
  **Intended role:** ATCUN-variant GGH

- **CBPα2** *(was MG31; old internal ID MG31)*: `DAHEAAKEAAKEAAKEALWKK`  
  **Length:** 21 aa; **N-terminus:** Free  
  **Intended role:** Baseline ATCUN

- **CBPα3** *(was MG40; old internal ID MG71)*: `DAHEAAKEAAKEAAKEAAKWKK`  
  **Length:** 22 aa; **N-terminus:** Free  
  **Intended role:** Minimal anchor (no Leu)

- **CBPα4** *(was MG39; old internal ID MG72)*: `DAHEAAKEAAKEAAKEAAKAWKK`  
  **Length:** 23 aa; **N-terminus:** Free  
  **Intended role:** Less hydrophobic anchor (A-WKK)

- **CBPα5** *(was MG50; old internal ID MG81)*: `DAHEAAKEAAKEAAKEAAKEAAKEAAKEAAKLWKK`  
  **Length:** 35 aa; **N-terminus:** Free  
  **Intended role:** Baseline long

- **CBPα6** *(was MG58; old internal ID MG83)*: `GGHEAAKEAAKEAAKEAAKEAAKEAAKEAAKLWKK`  
  **Length:** 35 aa; **N-terminus:** Free  
  **Intended role:** GGH-ATCUN long

## Family β — ATCUN + internal HxxxH clamps (Cu(II)-focused helix locking / secondary metal patch)

- **CBPβ1** *(was MG47; old internal ID MG74)*: `DAHEAAKEAAKEAAKHAAAHLWKK`  
  **Length:** 24 aa; **N-terminus:** Free  
  **Intended role:** Clamp position test

- **CBPβ2** *(was MG32; old internal ID MG32)*: `DAHEAAKEAAKHAAAHEAAKLWKK`  
  **Length:** 24 aa; **N-terminus:** Free  
  **Intended role:** Champion ATCUN + HxxxH clamp

- **CBPβ3** *(was MG37; old internal ID MG75)*: `DAHEAAKEAAKHQAAHEAAKLWKK`  
  **Length:** 24 aa; **N-terminus:** Free  
  **Intended role:** Clamp alternative (HQAAH)

- **CBPβ4** *(was MG36; old internal ID MG76)*: `DAHEAAKEAAKHRAAHEAAKLWKK`  
  **Length:** 24 aa; **N-terminus:** Free  
  **Intended role:** HxxxH clamp polar (HRAAH)

- **CBPβ5** *(was MG46; old internal ID MG77)*: `DAHEAAKEAAKHAAAHEAAKLYWKK`  
  **Length:** 25 aa; **N-terminus:** Free  
  **Intended role:** Aromatic anchor (LYWKK)

- **CBPβ6** *(was MG48; old internal ID MG78)*: `DAHEAAKEAAKEAAKHQAAHEAAKWKK`  
  **Length:** 27 aa; **N-terminus:** Free  
  **Intended role:** Double EAAK before clamp

- **CBPβ7** *(was MG49; old internal ID MG79)*: `DAHEAAKEAAKEAAKHAAAHEAAKAAWKK`  
  **Length:** 29 aa; **N-terminus:** Free  
  **Intended role:** Longer <30 with AAWKK

- **CBPβ8** *(was MG57; old internal ID MG84)*: `DAHEAAKEAAKEAAKEAAKHQAAHEAAKEAAKLWKK`  
  **Length:** 36 aa; **N-terminus:** Free  
  **Intended role:** HQAAH long

- **CBPβ9** *(was MG52; old internal ID MG85)*: `DAHEAAKEAAKEAAKEAAKHRAAHEAAKEAAKLWKK`  
  **Length:** 36 aa; **N-terminus:** Free  
  **Intended role:** Clamp HRAAH in long context

- **CBPβ10** *(was MG53; old internal ID MG86)*: `DAHEAAKEAAKEAAKHAAAHEAAKEAAKEAAKAWKK`  
  **Length:** 36 aa; **N-terminus:** Free  
  **Intended role:** Clamp + propagation + anchor A-WKK

- **CBPβ11** *(was MG51; old internal ID MG87)*: `DAHEAAKEAAKEAAKEAAKEAAAKHAAAHEAAKLWKK`  
  **Length:** 37 aa; **N-terminus:** Free  
  **Intended role:** Long scaffold + internal clamp

- **CBPβ12** *(was MG55; old internal ID MG89)*: `DAHEAAKEAAKEAAKEAAKEAAKHAAAHEAAKEAAKWKK`  
  **Length:** 39 aa; **N-terminus:** Free  
  **Intended role:** High stability + clamp + WKK

- **CBPβ13** *(was MG61; old internal ID MG90)*: `DAHEAAKEAAKEAAKEAAKHAAAHEAAKEAAKEAAKLYWKK`  
  **Length:** 41 aa; **N-terminus:** Free  
  **Intended role:** Robust propagation + anchor LYWKK

## Family γ — N-acetylated ATCUN-dead controls (mechanism dissection)

- **CBPγ1** *(was MG33; old internal ID MG33)*: `Ac-EAAKEAAKHAAAHEAAKEAAK`  
  **Length:** 21 aa; **N-terminus:** Acetylated  
  **Intended role:** Negative control, ATCUN-dead

- **CBPγ2** *(was MG45; old internal ID MG73)*: `Ac-DAHEAAKEAAKHAAAHEAAKLWKK`  
  **Length:** 24 aa; **N-terminus:** Acetylated  
  **Intended role:** Ac-control of MG35

- **CBPγ3** *(was MG59; old internal ID MG80)*: `Ac-EAAKEAAKEAAKHAAAHEAAKEAAKEAAKWKK`  
  **Length:** 32 aa; **N-terminus:** Acetylated  
  **Intended role:** Ac-control long, clamp-only

## Family δ — charged interaction comparators (Aβ engagement / α-induction stress-test)

- **CBPδ1** *(was MG34; old internal ID MG34)*: `DAHEEAAKRAAEAAKRAAEAAKRAAWK`  
  **Length:** 27 aa; **N-terminus:** Free  
  **Intended role:** Interaction comparator

- **CBPδ2** *(was MG54; old internal ID MG82)*: `DAHEEAAKRAAEEAAKRAAEEAAKRAAEEAAKWKK`  
  **Length:** 35 aa; **N-terminus:** Free  
  **Intended role:** Charged long controllable

- **CBPδ3** *(was MG64; old internal ID MG88)*: `DAHEEAAKRAAEEAAKRAAEEAAKRAAEEAAKRAAWKK`  
  **Length:** 38 aa; **N-terminus:** Free  
  **Intended role:** Charged long upper bound

---

# Design considerations

## Family α — ATCUN baselines (no internal clamp; low-interaction regime)

### Design intent
ATCUN-like N-termini (DAH or GGH) on an EAAK helical scaffold provide **strong, structurally defined Cu(II) capture** in water with minimal additional interaction features. These constructs are meant to answer: *“How much can Cu(II) sequestration alone shift Aβ conformational/aggregation metrics?”*

### Key caveats
- Requires a **free N-terminus** (no acetylation).
- Cu(II) binding is **pH-dependent** (backbone amide deprotonation contributes).
- These peptides are expected to be the **cleanest** and most interpretable, but may show **limited Aβ α-helix induction** unless Cu removal alone is sufficient.

### Peptide-specific notes

- **CBPα1**: ATCUN head variant (GGH) to probe sensitivity to DAH vs GGH.
- **CBPα2**: DAH-ATCUN baseline for Cu(II) capture with minimal confounders.
- **CBPα3**: DAH-ATCUN baseline for Cu(II) capture with minimal confounders. Minimal aromatic anchor (WKK) for reduced hydrophobicity.
- **CBPα4**: DAH-ATCUN baseline for Cu(II) capture with minimal confounders. Softer hydrophobic anchor (A-WKK) vs LWKK.
- **CBPα5**: DAH-ATCUN baseline for Cu(II) capture with minimal confounders.
- **CBPα6**: ATCUN head variant (GGH) to probe sensitivity to DAH vs GGH.

## Family β — ATCUN + internal HxxxH clamps (Cu(II)-focused helix locking / secondary metal patch)

### Design intent
Same ATCUN capture head as family α, plus an embedded **HxxxH (i,i+4) clamp** (e.g., HAAAH/HQAAH/HRAAH). The clamp is designed to (i) stabilize an α-helical turn and (ii) provide an additional metal-contact patch or interaction handle—without introducing long hydrophobic runs.

### Key caveats
- His clamps can generate **multiple coordination microstates** (tautomer/protonation/geometry). This increases complexity but is acceptable if tracked explicitly.
- Clamp placement (closer to the C-terminus vs central) can change interaction patterns; interpret outcomes relative to α-family baselines.
- Do not assume the clamp “wins” Cu from ATCUN; treat it primarily as a **helix/interaction modulator**.

### Peptide-specific notes

- **CBPβ1**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ2**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ3**: HQAAH clamp: expected to change His microstate distribution vs HAAAH. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ4**: HRAAH clamp adds a local cationic patch and can increase Aβ encounter rate. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ5**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Stronger aromatic anchor (LYWKK) for increased hydrophobic engagement (watch β-templating risk).
- **CBPβ6**: HQAAH clamp: expected to change His microstate distribution vs HAAAH.
- **CBPβ7**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Weaker anchor (A-WKK) to reduce hydrophobicity while retaining Trp contact.
- **CBPβ8**: HQAAH clamp: expected to change His microstate distribution vs HAAAH. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ9**: HRAAH clamp adds a local cationic patch and can increase Aβ encounter rate. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ10**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Weaker anchor (A-WKK) to reduce hydrophobicity while retaining Trp contact.
- **CBPβ11**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Single Trp anchor (LWKK) for moderate hydrophobic engagement.
- **CBPβ12**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif.
- **CBPβ13**: HAAAH clamp is the canonical i,i+4 His clamp used as primary helix-locking motif. Stronger aromatic anchor (LYWKK) for increased hydrophobic engagement (watch β-templating risk).

## Family γ — N-acetylated ATCUN-dead controls (mechanism dissection)

### Design intent
These are **ATCUN-dead controls** achieved by **N-acetylation**. They preserve the helical scaffold (and clamps where present) while disabling the key Cu(II) capture geometry. They answer: *“Are observed effects due to ATCUN Cu capture, or due to scaffold/clamp interactions?”*

### Key caveats
- N-acetylation removes the free N-terminus required for ATCUN-like Cu(II) binding, but **residual weak Cu binding** to His may still occur at high metal loadings.
- Use γ-family peptides at matched concentrations to deconvolute electrostatic and structural effects.

### Peptide-specific notes

- **CBPγ1**: N-acetylated: primary role is mechanistic control (ATCUN disabled).
- **CBPγ2**: N-acetylated: primary role is mechanistic control (ATCUN disabled).
- **CBPγ3**: N-acetylated: primary role is mechanistic control (ATCUN disabled).

## Family δ — charged interaction comparators (Aβ engagement / α-induction stress-test)

### Design intent
These constructs increase the **electrostatic encounter rate** with Aβ (higher charged residue density) to test whether **Aβ α-helix induction** can be promoted by transient binding while still keeping the design mostly helical/soluble.

### Key caveats
- Higher risk of **non-specific polyelectrolyte binding** and ambiguous readouts; always benchmark against α/β families.
- These are best treated as **stress-tests** rather than clean mechanistic probes.

### Peptide-specific notes

- **CBPδ1**: Charged comparator: higher interaction propensity; interpret only relative to α/β baselines.
- **CBPδ2**: Charged comparator: higher interaction propensity; interpret only relative to α/β baselines.
- **CBPδ3**: Charged comparator: higher interaction propensity; interpret only relative to α/β baselines.

---

## Recommended readouts (minimum)
For each peptide (apo and Cu-bound) and for competition systems (Aβ + Cu + peptide):
1) **Helicity (DSSP)**: time series + per-residue helix propensity
2) **Cu coordination stability**: Cu–donor distances, coordination number, geometry metrics
3) **Cu exposure**: SASA around Cu center as a reactivity proxy
4) **Aβ–peptide contacts**: contact maps + residence times
5) **Self-association**: peptide–peptide contacts (especially for long/charged constructs)
6) If feasible: **Cu transfer thermodynamics** (ΔG_exchange) for `Aβ–Cu + peptide → Aβ + peptide–Cu`
