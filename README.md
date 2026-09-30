# Generative AI narrows communication gaps, but provenance-sensitive evaluation erodes downstream gains

Reproducibility repository for the manuscript:

**Generative AI narrows communication gaps, but provenance-sensitive evaluation erodes downstream gains**

The study examines a production-to-evaluation process in institution-facing communication. Across four complementary experiments in the United States and United Kingdom, the design separates (i) upstream effects of access to generative AI on claim production from (ii) downstream effects of visible AI provenance on human evaluation.

## Study overview

The full program contains 24,000 participant entry records and 23,040 analyzed participant records across four study modules:

- **Study 1 — Production-side equalization:** 4,608 analyzed writers. Randomized unaided versus AI-access writing; focal outcome is condition-blinded claim quality across a continuous baseline advocacy-capacity measure.
- **Study 2 — Fixed-content provenance evaluation:** 3,456 analyzed evaluators. Claim text and merit-relevant information are held fixed while truthful AI provenance is hidden versus visible.
- **Study 3 — Linked production-to-evaluation design:** 3,456 analyzed writers and 6,912 analyzed evaluators, yielding 27,648 evaluator-message decisions. The focal contrasts compare unaided production, AI-assisted production with staged provenance, and AI-assisted production with visible provenance.
- **Study 4 — Provenance architecture:** 4,608 analyzed evaluators. Generic disclosure, neutral matched disclosure, a human-control/responsibility attestation package, and staged review are compared while substantive claim content is held fixed.

The experiments use English-language consumer-complaint and workplace-grievance tasks in the United States and United Kingdom. Experimental outcomes are research-task decisions and should not be interpreted as actual refunds, employment actions, grievance resolutions, or claimant welfare.

## Repository contents

The intended release structure is:

```text
.
├── README.md
├── data/
│   └── README.md
├── code/
│   └── README.md
├── materials/
│   └── README.md
└── prompts/
    └── system_prompt.txt
```

After the final reproducibility package is deposited, the repository should additionally contain de-identified analysis datasets, executable analysis scripts, figure-source data, and machine-readable study materials. The file-level manifest should be updated at that time.

## Reproducibility workflow

The final executable package should permit a reader to reproduce the reported analyses in the following order:

1. Validate participant-flow counts and construct the study-specific analysis samples.
2. Construct pre-treatment baseline advocacy-capacity variables and the observed quality measures.
3. Reproduce Study 1 writer-level models and capacity-gap contrasts.
4. Reproduce Study 2 fixed-content provenance contrasts for support and approval.
5. Reproduce Study 3 working logistic model, marginal approval probabilities, net outcome equalization, gap-level conversion loss, and covariance / graph-sensitivity analyses.
6. Reproduce Study 4 generic-referenced support contrasts and descriptive secondary outcomes.
7. Rebuild the figure-source datasets and reproduce the manuscript figures and supplementary tables.

## Analysis principles reflected in the manuscript

- AI assignment is defined by randomized **access** to the study interface, not by post-assignment uptake of model suggestions.
- Baseline advocacy capacity is measured from objectively scored pre-treatment sources; self-efficacy and structural-position variables are kept separate.
- Claim quality, downstream support / approval, and post-decision attribution measures are treated as distinct outcomes.
- Post-decision attribution measures are descriptive and are not interpreted as causal mediators.
- Study 3 uses the realized writer-message-evaluator graph. Reported graph irregularities are retained and addressed in covariance and graph-sensitivity analyses.
- The studies were not preregistered; focal / secondary labels are an ex post reporting hierarchy rather than a preregistered confirmatory family.

## AI-assisted writing intervention

The AI-assisted interface was constrained to factual institutional self-advocacy. The complete system instruction is provided in `prompts/system_prompt.txt`.

The study interface allowed up to four user turns and imposed a 450-token limit per model reply. It provided no browsing, external retrieval, hidden participant profile, or researcher-supplied biography. The final release should additionally document the exact provider, model identifier / snapshot, API or interface version, collection dates, and generation parameters from the original experiment logs.

## Data protection

Only de-identified analysis data should be released publicly. Direct identifiers, platform account identifiers, free-text fields that could reveal participant identity, and other information restricted by consent or ethics requirements should not be deposited. If any analysis variable cannot be publicly released, the repository should document the restriction and provide an appropriate access procedure or a reproducibility-safe derived dataset.

## Citation

Please cite the associated manuscript and the archived repository release. A DOI from an archival service such as Zenodo is recommended for the version of record because a GitHub branch can change over time.

## Repository status

This repository currently contains the documentation scaffold and the study-system prompt. Before the manuscript's final public data-and-code availability statement is used, the de-identified analysis data, executable analysis scripts, figure-source data, and final configuration metadata should be deposited and checked against the manuscript and Supplementary Information.
