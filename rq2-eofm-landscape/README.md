# RQ2 · The EOFM landscape

> **Research question:** Which EO modalities, spatial and temporal supports, representation strategies, and adaptation routes are covered by current EOFMs, and which capabilities required for ecohydrology remain underrepresented?

The RQ2 catalogues map the field at the level of named model versions and scholarly records. They support questions about observation pathways, temporal design, spatial sampling, parameter scale, representation access, release chronology, and the strength of ecohydrological evidence.

## Current snapshot

- **60 model/version records** representing **52 model families**.
- **34 multimodal records** and 26 single-pathway records.
- Observation groups: 23 optical only, 16 optical plus microwave/SAR, 18 broader multisensor or ancillary, and three other or single non-optical.
- Temporal support: 21 single/snapshot, 16 paired or short sequence, 20 explicit time series, and three annual embedding/product records.
- Ecohydrological evidence coding: one direct independent-measurement record, two direct product/proxy records, and 57 indirect or prospective records.

Reflected optical observations dominate the eligible release set. SAR supplies most microwave coverage. Explicit thermal pretraining remains uncommon, and passive-microwave emission and solar-induced fluorescence were absent as explicit pretraining pathways at the cutoff.

## Files

### [`eofm-models.csv`](eofm-models.csv)

One row per model/version. Important fields include:

| Field | Meaning |
|---|---|
| `model_name`, `model_family` | Version-level identity and reconciled family identity |
| `first_release_year`, `release_date` | Earliest verified public scholarly release |
| `publication_status`, `doi`, `arxiv_id`, `url` | Traceable bibliographic source |
| `observation_pathways`, `modality_group`, `multimodal` | Coded EO inputs and pathway breadth |
| `temporal_support`, `explicit_temporal` | Snapshot, paired/short-sequence, explicit time-series, or annual-product design |
| `resolution_min_m`, `resolution_max_m`, `resolution_mid_m` | Reported pretraining sampling distance or transparent plotting proxy |
| `parameters_m` | Reported encoder or named-variant parameter count |
| `ecohydrological_evidence` | Direct independent, direct product/proxy, or indirect/prospective evidence class |
| `coding_basis`, `notes` | Source basis and retained interpretation notes |

### [`publications.csv`](publications.csv)

The broader publication-role corpus used for the temporal analysis. It separates model descriptions, reviews or perspectives, and benchmark or evaluation studies while retaining candidate and family linkage.

### [`datasets.csv`](datasets.csv)

An initial inventory of named pretraining, embedding, and evaluation resources that are central to the review. Dataset roles are kept explicit because pretraining inputs, derived embedding products, task labels, and independent reference observations support different scientific claims. The inventory links to a primary description and includes a separate access field where a stable provider page has been verified.

## Interpretation notes

- Release counts describe activity and do not provide independent model counts when families share data, architecture, code, or benchmarks.
- Nominal sampling distance describes input sampling. Effective ecohydrological support also depends on sensing depth, footprint, pooling, and target aggregation.
- Multimodal coding establishes the presence of multiple input pathways. Cross-modal alignment, robustness to missing inputs, and process-specific complementarity require empirical evaluation.
- Public checkpoints and served embedding products have different adaptation, transparency, versioning, and compute implications.
- `n/r` and empty cells preserve unreported characteristics.

See [RQ3](../rq3-applications/README.md) for application evidence and [RQ4](../rq4-benchmarking/README.md) for controlled evaluation requirements.
