# Ecohydrological inference contract

Use this template when proposing an EOFM application, adding an evidence record, or designing a benchmark. Complete each field at the level needed for an independent reader to reconstruct the claim.

## 1. Scientific target

- **Target name:**
- **Physical definition and units:**
- **Inference tier:** T1 retrieval/index · T2 state/flux · T3 mechanism/event/outcome
- **Intended use:**
- **Domain of validity:** ecosystems, hydroclimates, seasons, event ranges, and management conditions

## 2. Observation pathway

- **EO sensors and products:**
- **Measurement pathways:** reflected optical · thermal emission · microwave emission/scattering · fluorescence · ancillary/modelled
- **Processing level and transformations:**
- **Representation:** model/version, checkpoint or embedding product, pretraining objective, pooling, and update schedule
- **Complementary inputs:** meteorology, terrain, soil, land cover, process-model output, or local observations

## 3. Spatial and temporal support

- **Nominal sampling distance:**
- **Effective input support:** pixel, footprint, field, reach, catchment, or region
- **Target/reference support:**
- **Temporal sampling and aggregation:**
- **Scale-matching procedure:**
- **Expected process timescale or memory:**

## 4. Reference evidence

- **Reference source and version:**
- **Reference directness:** independent observation · derived retrieval/product · model output · proxy label
- **Measurement or derivation uncertainty:**
- **Independence from model inputs and pretraining data:**
- **Known spatial, temporal, or sampling bias:**

## 5. Evaluation design

- **Adaptation regime and label budget:** frozen embeddings · linear probing · parameter-efficient adaptation · full fine-tuning · prompting
- **Baselines:** raw EO, engineered features, random initialisation, task-specific ML/DL, process model, hybrid workflow
- **Held-out shifts:** site · basin · biome · year · climate · event · sensor · resolution · label regime
- **Predictive metrics:**
- **Temporal diagnostics:** phase, onset, lag, memory, extremes, and recovery
- **Physical diagnostics:** bounds, coupled-variable relations, conservation or closure, and event timing
- **Uncertainty diagnostics:** calibration, interval coverage, sharpness, and error detection
- **Reproducibility information:** code, model version, data version, split definitions, seeds, and compute

## 6. Claim and falsification

- **Supported claim:**
- **Evidence boundary:**
- **Result that would falsify or materially weaken the claim:**
- **Unresolved attribution:** contribution of pretraining, architecture, input data, local observations, or process constraints
- **Operational or scientific readiness level:** exploratory · comparative · validated within domain · prospectively evaluated
