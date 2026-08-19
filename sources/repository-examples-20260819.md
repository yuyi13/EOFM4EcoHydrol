# Repository-design sources reviewed on 19 August 2026

This repository uses the compact research-companion principles from the `yu-repo` skill and adapts them for a literature-centred evidence resource. The following public repositories informed the implementation.

| Repository | Pattern reviewed | Design decision adopted here |
|---|---|---|
| [xiaoaoran/awesome-rsfms](https://github.com/xiaoaoran/awesome-rsfms) | Survey companion with model, dataset, benchmark, and paper groupings | Keep the review paper visible and connect resource groups to the scientific synthesis |
| [Jack-bo1220/Awesome-Remote-Sensing-Foundation-Models](https://github.com/Jack-bo1220/Awesome-Remote-Sensing-Foundation-Models) | Frequently updated model and dataset tables with paper, code, weight, and data links | Retain traceable source and access fields while separating version-level model records from broader publications |
| [ESIPFed/Awesome-Earth-Artificial-Intelligence](https://github.com/ESIPFed/Awesome-Earth-Artificial-Intelligence) | Separation of tools, models, weights, and literature | Distinguish resource role and third-party access conditions |
| [cv-mines/multi-view-datasets-survey](https://github.com/cv-mines/multi-view-datasets-survey) | Survey repository with searchable CSV data, documentation, tables, and assets | Use machine-readable CSVs as the maintained evidence layer and Markdown as the interpretive guide |
| [XAI4SAR/GenAIxSAR](https://github.com/XAI4SAR/GenAIxSAR) | Domain-specific survey resources tied to a paper | Keep domain scope explicit and expose the companion citation near the top of the README |

The resulting structure is organised by the four research questions in the preprint. This preserves the logic of the review while supporting direct access to model, application, dataset, and benchmark records. A single long README would make evidence provenance and update ownership harder to maintain, so each RQ has a scoped guide and associated source tables.
