# Contributing to EOFM4EcoHydrol

Contributions that improve the completeness, accuracy, provenance, or accessibility of the evidence base are welcome.

## In scope

- EOFM model or version releases;
- reviews, perspectives, and comparative evaluations;
- ecohydrological EOFM applications;
- pretraining, embedding, adaptation, benchmark, and independent-reference datasets;
- corrections to metadata, coding, access links, or evidence interpretation; and
- benchmark protocols and diagnostics relevant to the four research questions.

## Minimum information

Every suggestion should provide:

1. a title and stable primary-source link, DOI, or arXiv identifier;
2. the relevant RQ or RQs;
3. the resource role: model, publication, dataset, application evidence, benchmark, or context;
4. a short explanation of ecohydrological relevance;
5. official code, model-weight, embedding, or data links when available;
6. licence and access information where known; and
7. for empirical studies, the target, reference source, validation scope, baselines, and reported direction of evidence.

## Evidence principles

- Prefer primary papers, official proceedings, provider repositories, model cards, and dataset documentation.
- Preserve version identity and the earliest verified public scholarly release date.
- Separate demonstrated application evidence from prospective relevance.
- Record null, negative, and conditional results alongside positive results.
- Leave unresolved fields empty and explain uncertainty in a notes field.
- Do not upload third-party papers, model weights, or datasets unless their licence clearly permits redistribution.

## Workflow

Open a resource-suggestion issue for an initial screening decision or submit a pull request that changes the relevant CSV and its RQ guide when needed. Keep each pull request focused on one resource group or a small, reviewable set of records. Include source links in the pull-request description.

CSV files use UTF-8 encoding, one header row, and stable column names. Quote fields that contain commas or line breaks. Preserve existing identifiers so that downstream references remain valid.
