# Analysis code

This directory is reserved for the executable analysis scripts used to reproduce the manuscript and Supplementary Information.

## Recommended script order

```text
00_environment.*
01_import_and_validate.*
02_participant_flow.*
03_construct_capacity_and_quality.*
10_study1_analysis.*
20_study2_analysis.*
30_study3_analysis.*
31_study3_sensitivity.*
40_study4_analysis.*
50_make_figures.*
60_make_supplementary_tables.*
```

Use the language actually used for the final analyses (for example, R, Python, Stata, or a documented combination) and record exact package / library versions.

## Expected outputs

### Study 1
Reproduce:
- model-implied claim quality at the reported continuous-capacity reference points;
- higher-minus-lower capacity gradients;
- the AI-assisted minus unaided gap change;
- reported uncertainty intervals and supporting reliability summaries.

### Study 2
Reproduce:
- hidden- versus visible-provenance support means;
- message-cluster-adjusted visible-minus-hidden support contrast;
- approval risk difference and odds ratio;
- any reported standardized-effect and sensitivity calculations.

### Study 3
Reproduce:
- the working logistic model;
- standardized marginal approval probabilities under U0, AS, and AV;
- capacity gradients;
- net outcome equalization under staged and visible provenance;
- gap-level conversion loss;
- capacity-specific conversion loss at C*=0;
- two-way writer/message × evaluator cluster-robust inference;
- reported three-way covariance sensitivity and graph-preserving bootstrap.

Do not condition the focal approval model on post-treatment claim quality if reproducing the manuscript specification.

### Study 4
Reproduce:
- policy-arm support means;
- generic-referenced attestation and staged-review support contrasts;
- neutral-matched contrast;
- approval proportions;
- merit-indicator diagnostic;
- exploratory attestation-versus-staged and staged-versus-generic interval comparisons;
- decision-time and policy-acceptability summaries.

## Reproducibility requirements

Each script should:
1. read only documented input files;
2. set deterministic seeds where stochastic procedures are used;
3. write derived outputs to a separate `outputs/` directory;
4. avoid manual editing of reported tables or figure-source data;
5. print or save a compact validation log containing the key participant counts and headline estimates.

A single runner script or Makefile is recommended after the actual analysis files are deposited.
