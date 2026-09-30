# Data release

This directory is reserved for the de-identified analysis datasets and figure-source data associated with the manuscript.

## Recommended final files

- `study1_writers.csv` — retained Study 1 writer records.
- `study2_evaluators.csv` — retained Study 2 evaluator records.
- `study3_writers.csv` — retained Study 3 writer/message records.
- `study3_evaluations.csv` — Study 3 evaluator-message decision records.
- `study4_evaluators.csv` — retained Study 4 evaluator records.
- `figure_source_data/` — compact source tables used to construct manuscript figures.
- `codebook.csv` — variable names, labels, units, coding, missing-value conventions, and analysis roles.

The released data should preserve the analysis units and treatment indicators used in the manuscript while removing direct or indirect identifiers not needed to reproduce the reported analyses.

## Required checks before public release

1. Participant-flow counts reproduce Supplementary Table S1.
2. Study 1 retains 4,608 analyzed writers.
3. Study 2 retains 3,456 analyzed evaluators.
4. Study 3 retains 3,456 writers, 6,912 evaluators, and 27,648 evaluator-message decisions.
5. Study 4 retains 4,608 analyzed evaluators.
6. Treatment labels, country/context indicators, reporting-point variables, and outcome units match the manuscript.
7. No direct identifiers or disclosive free-text fields are included.

If consent or ethics restrictions prevent release of a raw field, provide the derived analysis variable used in the published models whenever possible and document the restriction here.
