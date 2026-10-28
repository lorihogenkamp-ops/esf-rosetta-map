# The ESF Rosetta Stone Map

**An interdisciplinary evidence architecture for the Evolutionary Stress Framework (ESF)**
Lori Hogenkamp · Center for Adaptive Stress · Version 2.0.0 · 2026-10-26 · CC BY 4.0
Live map: https://lorihogenkamp-ops.github.io/esf-rosetta-map/ · Zenodo: https://doi.org/10.5281/zenodo.23422797

> **Version 2.0.0 is a correction and canon-alignment release.** If you downloaded or cited version 1.0 (16 Oct 2026), please read [ERRATA.md](ERRATA.md): 14 of the 50 v1.0 citations were wrong in some element and four annotations overstated their sources. Version 1.0 remains on Zenodo unchanged as the historical baseline.

## What the map is

The map translates the ESF evidence library into a navigable structure: each source is annotated for what it argues, why it matters for the framework, what the annotation takes it to support, its limits, and what it makes possible next. Sources sit in six **evidence domains** (E1 Foundational Regulation Theory; E2 Biological Mechanisms of Stress Adaptation; E3 Developmental Calibration and Plasticity; E4 Emergence, Complexity and Network Medicine; E5 Neurodiversity, Disability and Human Variation; E6 Evolution, Ecology and Population-Level Diversity) and carry thirteen cross-cutting tags.

Since v2.0 the map's claims are the **14 Public Claims** of *The Evolutionary Stress Framework: A Field Guide* v1.0 (Zenodo [10.5281/zenodo.21937705](https://doi.org/10.5281/zenodo.21937705), 17 Oct 2026), shown verbatim with their evidence-status label (Established foundation · Strong convergent support · ESF synthesis · Active empirical hypothesis · Methodological implication), their boundary sentence, and their published anchors. The ESF Canonical Terminology and Boundary Map (same record) controls vocabulary.

## Three views

- **Sources** -- browse 57 sources by evidence domain, filter by tag, open the full annotation. 40 external sources are fully annotated, 9 are stubs queued for annotation, and 7 are ESF publication cards.
- **Claims** -- the 14 Public Claims plus one supplementary proposition (cooperative neurodiversity). Each shows its typed source links grouped by relation.
- **Topics (v1.0)** -- the 14 March 2026 map claims, kept as navigation and history. Two are retired as wording (c02, c11); five have wording superseded by the published canon. Each topic points to the Public Claims it was reassessed against and lists the sources that carried it in v1.0.

## How links work, and how they are counted

Every source-claim connection is a **typed link** with a relation, a scope, a rationale and a review status:

| Relation | Meaning |
|---|---|
| supports | the source's own findings or argument support the stated component of the claim |
| refines | the source sharpens a term, boundary or mechanism in the claim |
| constrains | the source limits how far the claim can be taken |
| challenges | the source cuts against the claim or a component of it |
| background | topically relevant context; no evidential weight claimed |
| develops | an ESF publication that proposes or formalises the claim -- displayed, never counted as independent support |

**Counting rule.** Only links with review status *approved* count toward a claim, and counts are reported per relation and per target. In v2.0.0 all 175 typed links are **proposed** (85 supports, 5 refines, 1 constrains, 66 background, 18 develops) and **none is approved**: the interface shows every claim as "0 approved · n proposed" by design. Evidential support was deliberately *not* inherited from the v1.0 claim set; each connection is being re-reviewed for relation and scope. The 128 v1.0 topic links are kept as history; 19 of them are marked as retired support readings.

A published anchor (an ESF paper in which a claim is stated) is named on the claim and never counted. Developed-in is not supported-by.

## Files

| File | What it is |
|---|---|
| `index.html` | the map: a single self-contained page (React 18 from cdnjs; Google Fonts); the data block is embedded as `<script id="esf-data" type="application/json">` |
| `esf-rosetta-map.json` | the same data as a standalone machine-readable export (schema 2.1): `meta`, `layers` (= evidence domains), `tags`, `public_claims`, `topics`, `supplementary_propositions`, `sources` (with `audit`, `legacy_links`, `claim_links`), `publications`, `intake_candidates`, `errata`, `validation` |
| `esf-rosetta-map.md` | a reading copy of the data for people and language models |
| `ERRATA.md` | corrections from v1.0, with the v1.0 and v2.0 citation text side by side |
| `CHANGELOG.md` | what changed in each version |
| `CITATION.cff` | citation metadata |
| `LICENSE` | CC BY 4.0 |

## Audit trail

Each source carries an `audit` block: `doi_identity` (confirmed), `metadata` (match / corrected / author-supplied, with a note), `annotation` (not yet checked / revised / flagged / unannotated / draft, with a note) and `links`. Corrected citations keep the v1.0 text in `full_v1`; revised annotations keep the v1.0 text in `*_v1` fields. The `validation` block records the counts the interface must reproduce.

## Citing

Hogenkamp, L. (2026). *The ESF Rosetta Stone Map: An Interdisciplinary Evidence Architecture for the Evolutionary Stress Framework* (Version 2.0.0) [Data set]. Center for Adaptive Stress. Zenodo. https://doi.org/10.5281/zenodo.23422797

See `CITATION.cff`. Please cite the version you used; the concept DOI resolves to the latest version.

## Related records

- Hogenkamp, L. (2026). The Evolutionary Stress Framework: A Field Guide, v1.0. Zenodo. https://doi.org/10.5281/zenodo.21937705
- Hogenkamp, L. (2026). Regulatory Bandwidth: A theoretical integration of present multisystem stress-regulatory capacity. *Psychoneuroendocrinology*, 192, 107955. https://doi.org/10.1016/j.psyneuen.2026.107955
- Hogenkamp, L. (2026). Regulatory capacity is not a scalar: Metrics, perturbations, and viability in network physiology. *Frontiers in Network Physiology*, 6, 1961712. https://doi.org/10.3389/fnetp.2026.1961712

## Status and intended use

The ESF is a conceptual framework, not a clinical instrument and not medical advice. The map is a research and teaching aid: a way to see which published work the framework draws on, what each source does and does not establish, and where the framework adds its own reasoning. It is maintained by the Center for Adaptive Stress (Cincinnati, Ohio; ndstress.org · evostress.blog). Corrections are welcome: open an issue in this repository or write to info@ndstress.org.
