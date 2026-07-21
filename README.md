# EOFM4EcoHydro

**Earth observation foundation models for process-aware ecohydrological monitoring**

EOFM4EcoHydro is a curated resource hub for the use of Earth observation foundation models (EOFMs) in ecohydrology. It is being developed as the companion repository for the review paper *Advancing Spatiotemporal Ecohydrological Monitoring with Earth Observation Foundation Models: Concepts, Progress and Challenges*, which is in preparation for *IEEE Geoscience and Remote Sensing Magazine*.

The primary purpose of this repository is to organise papers, EOFMs, datasets, benchmarks and open-source tools relevant to ecohydrological research. Particular attention is given to the inference of dynamic and coupled water, energy, vegetation and carbon processes from heterogeneous Earth observation data.

## Scope

The repository will cover five connected resource groups:

1. **Papers** — reviews, model papers, benchmark studies and ecohydrological applications.
2. **EO foundation models** — model descriptions, supported observation modalities, code, weights and documented adaptation strategies.
3. **Datasets** — pretraining datasets, downstream task datasets and independent validation data.
4. **Benchmarks and evaluation** — tasks, metrics and experimental designs for spatial, temporal, sensor, scale and geographic transfer.
5. **Tools and examples** — software, tutorials and reproducible workflows for adapting or evaluating EOFMs.

This resource collection is intended to connect model development with ecohydrological process meaning. It therefore distinguishes satellite observations and retrieval signals from inferred states, fluxes and higher-level products. It also records whether reported applications are supported by independent validation, product intercomparison, process constraints or only prospective relevance.

## Ecohydrological domains

| Domain | Representative observations, variables and applications |
|---|---|
| Water | Surface and root-zone soil moisture, vegetation water content, inundation, terrestrial water storage and drought |
| Energy | Land surface temperature, evapotranspiration, sensible and latent heat partitioning and surface energy balance |
| Vegetation and carbon | Phenology, solar-induced chlorophyll fluorescence, gross primary productivity, ecosystem carbon exchange and water-use efficiency |
| Coupled processes | Plant water stress, drought onset and recovery, irrigation, heat stress and water–energy–carbon feedbacks |

## Resource organisation

The planned repository structure is:

```text
EOFM4EcoHydro/
├── papers/       # Reviews, methods, applications and evidence tables
├── models/       # EOFM catalogue, model metadata, code and weights
├── datasets/     # Pretraining, downstream and validation datasets
├── benchmarks/   # Tasks, metrics, data splits and evaluation protocols
├── tools/        # Libraries, tutorials and reproducible examples
└── figures/      # Taxonomies and figures associated with the review
```

Where practical, resource tables will be provided in both readable Markdown and machine-readable formats such as CSV. The catalogue will record metadata including publication year, observation modality, spatial and temporal coverage, target variable, adaptation setting, validation source, geographic scope, code availability, data access and licence.

## Dataset categories

Dataset roles will be reported separately because they provide different forms of evidence:

| Dataset role | Purpose |
|---|---|
| Pretraining data | Learning general or multimodal EO representations |
| Adaptation data | Fine-tuning, linear probing, prompting or other downstream adaptation |
| Benchmark data | Comparing models under a defined task and evaluation protocol |
| Independent validation data | Evaluating physical or process relevance using field measurements, flux towers, monitoring networks or other independent references |

## Resource selection principles

Resources will be included when they have a clear connection to EOFMs, enabling methods or ecohydrological applications. Entries should link to primary and traceable sources wherever possible. Model capability claims will be separated from prospective applications, and reported performance will be interpreted with respect to target observability, reference-data uncertainty, spatial and temporal scale, and distribution shift.

The repository will not rank EOFMs using a single aggregate score. Comparisons should instead report the task, data split, baseline, metric and transfer setting needed to interpret performance.

## Project status

The repository is under active development alongside the GRSM review. The initial release will prioritise:

- a structured paper catalogue;
- an EOFM catalogue with official paper, code and model-weight links;
- pretraining, downstream and validation dataset inventories; and
- a benchmark matrix organised by ecohydrological variable and evaluation setting.

## Contributing

Suggestions for missing papers, models, datasets, benchmarks and tools are welcome. Please open an issue or submit a pull request with a primary source, a short explanation of the ecohydrological relevance and, where applicable, links to official code, model weights or data documentation.

## Citation

Citation information for the review paper will be added after publication. A `CITATION.cff` file and the final paper metadata will be included in a future release.

## Licence and third-party resources

The repository will provide links and metadata for third-party papers, models, code and datasets. Each resource remains subject to the licence and access conditions specified by its original provider.
