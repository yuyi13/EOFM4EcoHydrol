# RQ4 · Benchmarking EOFMs for ecohydrology

> **Research question:** Which benchmark designs and diagnostic criteria are needed to evaluate accuracy, temporal dynamics, physical consistency, uncertainty, transferability, and readiness for scientific or operational use?

RQ4 treats benchmarking as scientific specification. A benchmark connects a model output to an ecohydrological claim through a defined observation and reference pathway, an adaptation protocol, and a domain of validity.

## Files

| File | Contents |
|---|---|
| [`benchmark-evidence.csv`](benchmark-evidence.csv) | Study-level audit of 10 general EOFM suites and 10 ecohydrological evaluations |
| [`benchmark-blueprint.csv`](benchmark-blueprint.csv) | Target-first design for six ecohydrological families, including reference data, support, shifts, and diagnostics |
| [`context-sources.csv`](context-sources.csv) | Conceptual and infrastructure sources used to frame benchmark requirements |
| [`datasets.csv`](datasets.csv) | Initial catalogue of process, reference, and EOFM-oriented data infrastructure discussed in the review |

## Eight diagnostic dimensions

| Dimension | Evaluation question |
|---|---|
| **Process target** | Is the physical quantity, unit, inference tier, and intended use explicit? |
| **Reference directness** | Does the evaluation distinguish independent observations from retrievals, products, proxies, and model outputs? |
| **Temporal dynamics** | Are phase, onset, lag, memory, extremes, and recovery evaluated at process-relevant support? |
| **Transfer or shift** | Are sites, basins, biomes, years, climates, events, sensors, resolutions, or regimes held out? |
| **Adaptation fairness** | Are inputs, label budgets, heads, optimisation, and compute controlled across models and baselines? |
| **Physical consistency** | Are bounds, water–energy–carbon coupling, balance or closure, and event timing tested out of sample? |
| **Uncertainty or reliability** | Are calibration, coverage, sharpness, error detection, and decision risk examined? |
| **Reproducibility** | Are data versions, splits, model versions, code, seeds, and compute available? |

## Evidence-led priorities

General EOFM suites in the audit provide strong fair-adaptation and reproducibility practices. Ecohydrological evaluations provide stronger process targeting, reference directness, temporal tests, and distribution-shift designs. Future benchmarks can integrate these strengths while expanding physical-consistency and uncertainty diagnostics.

The benchmark ledger uses ordinal scores:

- `0` — criterion absent;
- `1` — partial or indirect coverage through a proxy, restricted subset, or incomplete test;
- `2` — criterion explicitly operationalised.

Scores provide a transparent coverage audit. They do not constitute a performance leaderboard.

## Target-first workflow

1. Define the physical target, units, inference tier, and intended domain.
2. Select observation and reference pathways with known support and uncertainty.
3. Match spatial and temporal support before calculating performance.
4. Fix adaptation rules, label budgets, baselines, and repeated-run reporting.
5. Hold out the shifts that matter for the intended scientific or operational claim.
6. Report predictive, temporal, physical, uncertainty, cost, and reproducibility diagnostics together.

The [benchmark blueprint](benchmark-blueprint.csv) instantiates this workflow for soil water and storage, surface energy and ET, carbon exchange and stocks, vegetation condition, catchment response, and disturbance and recovery.
