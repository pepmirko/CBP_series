# consideration.md — MG series (length-based renaming from MG70)

This document is the **current source of truth** for the MG library after:
1) **Renaming all non-core peptides starting from MG70** so that IDs increase with **sequence length** (ascending), and  
2) **Pruning** a small number of sequences that were duplicates or low-value at this stage.

> **Naming policy applied:** Core IDs are kept as-is (MG31–MG34).  
> All additional candidates are renumbered **MG70+** ordered by **length** (ties broken by sequence and role).

---

## 1) Current MG library

### 1.1 Core set (Cu(II)-focused, highest interpretability)
- **MG31** (from MG31): `DAHEAAKEAAKEAAKEALWKK`  
  **Role:** Baseline ATCUN  
  **Length:** 21 aa; **N-terminus:** Free
- **MG32** (from MG32): `DAHEAAKEAAKHAAAHEAAKLWKK`  
  **Role:** Champion ATCUN + HxxxH clamp  
  **Length:** 24 aa; **N-terminus:** Free
- **MG33** (from MG33): `Ac-EAAKEAAKHAAAHEAAKEAAK`  
  **Role:** Negative control, ATCUN-dead  
  **Length:** 21 aa; **N-terminus:** Acetylated
- **MG34** (from MG34): `DAHEEAAKRAAEAAKRAAEAAKRAAWK`  
  **Role:** Interaction comparator  
  **Length:** 27 aa; **N-terminus:** Free

### 1.2 Additional candidates (<30 aa), renumbered MG70+
- **MG70** (from MG43): `GGHEAAKEAAKEAAKLWKK`  
  **Role:** ATCUN-variant GGH  
  **Length:** 19 aa; **N-terminus:** Free
- **MG71** (from MG40): `DAHEAAKEAAKEAAKEAAKWKK`  
  **Role:** Minimal anchor (no Leu)  
  **Length:** 22 aa; **N-terminus:** Free
- **MG72** (from MG39): `DAHEAAKEAAKEAAKEAAKAWKK`  
  **Role:** Less hydrophobic anchor (A-WKK)  
  **Length:** 23 aa; **N-terminus:** Free
- **MG73** (from MG45): `Ac-DAHEAAKEAAKHAAAHEAAKLWKK`  
  **Role:** Ac-control of MG35  
  **Length:** 24 aa; **N-terminus:** Acetylated
- **MG74** (from MG47): `DAHEAAKEAAKEAAKHAAAHLWKK`  
  **Role:** Clamp position test  
  **Length:** 24 aa; **N-terminus:** Free
- **MG75** (from MG37): `DAHEAAKEAAKHQAAHEAAKLWKK`  
  **Role:** Clamp alternative (HQAAH)  
  **Length:** 24 aa; **N-terminus:** Free
- **MG76** (from MG36): `DAHEAAKEAAKHRAAHEAAKLWKK`  
  **Role:** HxxxH clamp polar (HRAAH)  
  **Length:** 24 aa; **N-terminus:** Free
- **MG77** (from MG46): `DAHEAAKEAAKHAAAHEAAKLYWKK`  
  **Role:** Aromatic anchor (LYWKK)  
  **Length:** 25 aa; **N-terminus:** Free
- **MG78** (from MG48): `DAHEAAKEAAKEAAKHQAAHEAAKWKK`  
  **Role:** Double EAAK before clamp  
  **Length:** 27 aa; **N-terminus:** Free
- **MG79** (from MG49): `DAHEAAKEAAKEAAKHAAAHEAAKAAWKK`  
  **Role:** Longer <30 with AAWKK  
  **Length:** 29 aa; **N-terminus:** Free

### 1.3 Additional candidates (>30 aa), renumbered MG70+
- **MG80** (from MG59): `Ac-EAAKEAAKEAAKHAAAHEAAKEAAKEAAKWKK`  
  **Role:** Ac-control long, clamp-only  
  **Length:** 32 aa; **N-terminus:** Acetylated
- **MG81** (from MG50): `DAHEAAKEAAKEAAKEAAKEAAKEAAKEAAKLWKK`  
  **Role:** Baseline long  
  **Length:** 35 aa; **N-terminus:** Free
- **MG82** (from MG54): `DAHEEAAKRAAEEAAKRAAEEAAKRAAEEAAKWKK`  
  **Role:** Charged long controllable  
  **Length:** 35 aa; **N-terminus:** Free
- **MG83** (from MG58): `GGHEAAKEAAKEAAKEAAKEAAKEAAKEAAKLWKK`  
  **Role:** GGH-ATCUN long  
  **Length:** 35 aa; **N-terminus:** Free
- **MG84** (from MG57): `DAHEAAKEAAKEAAKEAAKHQAAHEAAKEAAKLWKK`  
  **Role:** HQAAH long  
  **Length:** 36 aa; **N-terminus:** Free
- **MG85** (from MG52): `DAHEAAKEAAKEAAKEAAKHRAAHEAAKEAAKLWKK`  
  **Role:** Clamp HRAAH in long context  
  **Length:** 36 aa; **N-terminus:** Free
- **MG86** (from MG53): `DAHEAAKEAAKEAAKHAAAHEAAKEAAKEAAKAWKK`  
  **Role:** Clamp + propagation + anchor A-WKK  
  **Length:** 36 aa; **N-terminus:** Free
- **MG87** (from MG51): `DAHEAAKEAAKEAAKEAAKEAAAKHAAAHEAAKLWKK`  
  **Role:** Long scaffold + internal clamp  
  **Length:** 37 aa; **N-terminus:** Free
- **MG88** (from MG64): `DAHEEAAKRAAEEAAKRAAEEAAKRAAEEAAKRAAWKK`  
  **Role:** Charged long upper bound  
  **Length:** 38 aa; **N-terminus:** Free
- **MG89** (from MG55): `DAHEAAKEAAKEAAKEAAKEAAKHAAAHEAAKEAAKWKK`  
  **Role:** High stability + clamp + WKK  
  **Length:** 39 aa; **N-terminus:** Free
- **MG90** (from MG61): `DAHEAAKEAAKEAAKEAAKHAAAHEAAKEAAKEAAKLYWKK`  
  **Role:** Robust propagation + anchor LYWKK  
  **Length:** 41 aa; **N-terminus:** Free

---

## 2) Removed / postponed sequences (with rationale)

- **MG35**: `DAHEAAKEAAKHAAAHEAAKLWKK`  
  **Reason:** Exact duplicate of core champion (same sequence as MG32); keep only one to avoid redundancy.
- **MG38**: `DAHEAAKEAAKEAAKEAAKEAAKLWKK`  
  **Reason:** Redundant baseline variant very close to MG39/MG40; keep a smaller, cleaner baseline set.
- **MG41**: `DAHEEAAKRAAEEAAKRAAEEAAKWKK`  
  **Reason:** Redundant 'charged-light' comparator given that the core set already includes a charged interaction comparator (MG34).
- **MG42**: `DAHEAAKEAAKEAAKEAAKWKK`  
  **Reason:** Exact duplicate of MG40 (same sequence).
- **MG44**: `DAHEAAKEAAKHAAAHEAAKEAAKWKK`  
  **Reason:** Redundant clamp+propagation short construct; MG49 and MG46 cover the same design lever with clearer differentiation.
- **MG56**: `DAHEAAKEAAKHAAAHEAAKEAAKHAAAHEAAKLWKK`  
  **Reason:** Double HxxxH clamp increases coordination microstate complexity and reduces interpretability in first-pass screens.
- **MG60**: `DAHEAAKEAAKEAAKEAAKEAAKEAAKEAAKAWKK`  
  **Reason:** Long A-WKK anchor variant largely overlaps with baseline long (MG50) and provides limited new information.
- **MG62**: `DAHEAAKEAAKEAAKEAAKEAAKEAAKEAAKEAAKWKK`  
  **Reason:** EAAKx7 super-scaffold overlaps with baseline long (MG50) without adding clamp/anchor leverage; low incremental value.
- **MG63**: `DAHEAAKEAAKEAAKHAAAHEAAKEAAKEAAKHRAAHEAAKLWKK`  
  **Reason:** Dual mixed clamps (HAAAH + HRAAH) likely generates many microstates; postpone to later phase if needed.

---

## 3) Design logic (why these sequences exist)

### 3.1 ATCUN-like Cu(II) capture head (H₂N–X–X–His)
Most MG peptides start with **DAH** (or **GGH** in specific controls), i.e. an ATCUN-like N-terminus intended to bind **Cu(II)** strongly in water.

**Key implications**
- A **free N-terminus is mandatory** for ATCUN-like coordination (**no N-acetylation**).
- Cu(II) binding is **pH-dependent** (backbone amide deprotonation contributes to the N₄ site).
- Compared to Cu–Aβ binding (many microstates), ATCUN-like binding is generally **more structurally defined**, improving competition assays and parameterization.

### 3.2 Embedded i,i+4 His clamps (HxxxH)
Several peptides include an internal **HxxxH** motif (e.g., `HAAAH`, `HRAAH`, `HQAAH`).

**Design intent**
- Residues at i and i+4 sit on the same helical face, enabling **metal-assisted stabilization** of an α-helical turn and/or providing a secondary metal-contact patch.

**Interpretation caveat**
- His-based clamps can generate **multiple coordination microstates** (tautomer/protonation/geometry). This is expected; treat it as designed heterogeneity.

### 3.3 EAAK-based helical scaffold
EAAK-like repeats provide:
- high solubility,
- strong intrinsic helix propensity as length increases,
- reduced self-aggregation risk relative to hydrophobic helices.

### 3.4 Aromatic anchor near the C-terminus (W)
Many sequences include a single **Trp (W)** near the end (e.g., `...LWKK`, `...WKK`, `...LYWKK`).

**Design intent**
- weak engagement of hydrophobic patches (e.g., Aβ hydrophobic core) **without** β-zipper-prone hydrophobic runs.

---

## 4) Controls (non-negotiable for clean interpretation)

### 4.1 ATCUN-dead negative controls (N-acetylated)
Peptides prefixed with **Ac-** are intended to **disable ATCUN-like Cu(II) binding** while keeping the internal clamp/scaffold intact.  
Use these to isolate effects due to internal His clamps vs N-terminal Cu capture.

---

## 5) Recommended computational readouts (minimum set)

For each MG peptide (apo and Cu-bound), and for competition systems (Aβ + Cu + MG):
1) **Helicity (DSSP)**: time series + per-residue helix propensity  
2) **Cu coordination stability**: Cu–donor distances; coordination numbers; geometry metrics  
3) **Cu exposure**: SASA around Cu center as a reactivity proxy  
4) **Aβ–MG contacts**: contact maps; residence times; interaction hotspots  
5) **Self-association**: MG–MG contacts (especially for long/charged constructs)  
6) If feasible: **Cu transfer thermodynamics** (ΔG_exchange) for  
   `Aβ–Cu + MG → Aβ + MG–Cu`

---

## 6) Practical ranking rule
Prefer candidates that simultaneously:
1) show stable **Cu capture** by MG in competition,
2) maintain **high helicity** without self-aggregation,
3) reduce Aβ aggregation-prone metrics (β-content, inter-Aβ contacts) **and/or** increase Aβ α-helical population (to be quantified),
4) show reduced predicted/observed **redox activity** relative to Cu–Aβ (to be tested, not assumed).

---

## 7) Machine-readable source of truth
A fully updated CSV reflecting this renaming and pruning is provided as:  
`MG_Series_Length_Renamed_from70.csv`
