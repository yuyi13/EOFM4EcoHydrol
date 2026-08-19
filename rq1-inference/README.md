# RQ1 · From EO signals to ecohydrological inference

> **Research question:** How do EO signals and complementary data support inference of ecohydrological properties, states, fluxes, mechanisms, and decision-relevant outcomes, and where do observation physics, reference uncertainty, scale, and process constraints enter this inference chain?

RQ1 defines the scientific meaning of an EOFM result before model comparison begins. An EO measurement is shaped by sensor physics, acquisition geometry, atmospheric effects, processing, and spatial and temporal support. An EOFM representation inherits these properties together with the assumptions in its pretraining and adaptation data. A defensible downstream claim therefore links the target to the complete observation–representation–reference pathway.

## Inference hierarchy

| Level | Role | Examples | Evidence needed |
|---|---|---|---|
| **T0 · Observations** | Calibrated or processed measurements entering the inference chain | Reflected radiance or reflectance, brightness temperature, SAR backscatter, fluorescence radiance | Sensor and processing provenance; sampling and support; quality flags; uncertainty |
| **T1 · Retrievals and indices** | Variables or proxies closely connected to the observation signal | NDVI, LST, surface soil moisture retrieval, inundation, vegetation water indices | Reference matched to sensing depth and support; retrieval assumptions; scale-aware validation |
| **T2 · Estimated states and fluxes** | Ecohydrological quantities requiring stronger inversion, forcing, or partitioning assumptions | Root-zone soil moisture, ET, GPP, biomass, groundwater depth, streamflow | Independent observations where available; temporal tests; uncertainty; coupled-variable and balance diagnostics |
| **T3 · Mechanisms, events, and outcomes** | Process interpretation and decision-relevant predictions | Drought onset and recovery, flood impact, crop stress, wildfire severity, management outcomes | Event or regime holdouts; causal or mechanistic evidence; calibrated risk; prospective utility where claimed |

Tier assignment is target- and use-dependent. A variable can occupy different evidentiary roles when its reference source, intended interpretation, or decision context changes.

## Observation pathways

| Pathway | Principal ecohydrological sensitivity | Common limitations to record |
|---|---|---|
| Reflected optical | Vegetation structure, pigment, surface composition, water-sensitive spectral response | Cloud and illumination effects; canopy saturation; atmospheric correction; optical access to subsurface states |
| Emitted thermal | Surface temperature and energy-balance response | Atmospheric correction; emissivity; cloud gaps; instantaneous acquisition time; surface-to-canopy interpretation |
| Microwave emission and scattering | Surface and vegetation water status, roughness, structure, inundation | Sensing-depth and roughness effects; radio-frequency interference; coarse passive-microwave support; SAR geometry |
| Solar-induced fluorescence | Photosynthetic activity and stress-related response | Low signal-to-noise; coarse support; retrieval assumptions; aggregation over heterogeneous ecosystems |
| Ancillary, retrieved, or modelled inputs | Forcing, terrain, climate, land cover, and contextual constraints | Target leakage; circular evaluation; model and reanalysis assumptions; mismatched support |

## Specify the claim before selecting the model

Use the [inference contract](inference-contract.md) to document:

1. the physical target, units, and inference tier;
2. the EO and complementary observation pathways;
3. spatial and temporal supports for inputs, outputs, and references;
4. the role and independence of the reference data;
5. the adaptation regime and comparison baselines;
6. distribution shifts, physical diagnostics, and uncertainty tests; and
7. the domain within which the final claim is intended to hold.

## Literature entry points

[`key-literature.csv`](key-literature.csv) provides a compact set of sources used to establish the observation physics, scale, validation, process-understanding, and EOFM foundations of RQ1. The full scientific synthesis and cited evidence are available in [the preprint](https://arxiv.org/abs/2608.15282) and [the curated 196-entry reference library](../paper/references.bib).
