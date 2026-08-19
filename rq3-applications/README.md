# RQ3 · EOFMs across ecohydrological applications

> **Research question:** What EOFM capabilities have been demonstrated across ecohydrological target classes, and how does the strength of this evidence depend on target observability, reference independence, and evaluation under environmental or sensor shifts?

RQ3 evaluates application-level evidence through the inference hierarchy established in RQ1. The source ledger contains 73 screened records: 71 eligible primary application studies, one contextual review, and one excluded non-EOFM record retained for screening provenance.

## Files

### [`application-evidence.csv`](application-evidence.csv)

The ledger records bibliographic metadata and structured evidence coding.

| Field | Meaning |
|---|---|
| `inclusion_status` | Primary evidence, review/context, or excluded record |
| `application_family` | Broad application domain used in the synthesis |
| `model_group` | EOFM or representation product evaluated by the study |
| `evidence_tier` | T1 retrieval/index, T2 state/flux, T3 mechanism/event/outcome, or a tier-spanning study |
| `evidence_role` | The role the result plays in the synthesis |
| `pathway` | Observation–representation–target pathway |
| `validation_scope` | Geographic, temporal, event, sensor, or other evaluation structure |
| `reference_directness` | Independence and physical proximity of the target reference |
| `evidence_direction` | Positive, mixed/conditional, or null/negative relative to meaningful baselines |

Abstracts are included to support screening traceability. Interpret claims through the coded evidence fields and verify details in the linked primary article.

## Evidence profile

Across the 71 eligible primary records, evidence is concentrated in T2 and T3 applications. The ledger contains 27 Tier 2 records, 36 Tier 3 records, seven records spanning Tiers 2–3, and one Tier 1 record. Reported directions comprise 52 positive, 17 mixed or conditional, and two null or negative primary records.

Current studies most consistently demonstrate reusable spatial context, label-efficient adaptation, and multimodal fusion. Evidence strength varies with:

- physical observability of the target;
- independence and uncertainty of reference data;
- alignment among input, target, and reference supports;
- contribution of meteorological forcing, local observations, or engineered covariates;
- comparison with raw EO, task-specific, randomly initialised, and process-based baselines; and
- evaluation under geographic, temporal, environmental, event, or sensor shifts.

Field-referenced evidence is emerging for vegetation and fuel water content, soil moisture, groundwater, water quality, biomass, and soil carbon. Flux evidence includes tower-partitioned GPP and ET evaluations that use operational products or hybrid daily forcing. Event-mapping studies increasingly use spatial, temporal, sensor, and event holdouts. Physical consistency, calibrated uncertainty, causal attribution, post-event recovery, and prospective decision benefit remain sparsely evaluated.

## Responsible interpretation

The evidence-direction field is a descriptive record-level synthesis across heterogeneous targets, metrics, baselines, and validation designs. A positive code does not imply process fidelity or general transfer. Null and mixed findings are retained because they define the conditions under which reusable representations add limited value.

Use [the RQ1 inference contract](../rq1-inference/inference-contract.md) to assess a particular claim and [the RQ4 benchmark framework](../rq4-benchmarking/README.md) to translate evidence gaps into an evaluation design.
