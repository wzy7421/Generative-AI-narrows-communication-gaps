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

## Reproducibility scope

The reproducibility package is organized around the following analyses:

1. Participant-flow accounting and study-specific analysis samples.
2. Construction of pre-treatment baseline advocacy-capacity variables and observed quality measures.
3. Study 1 writer-level models and capacity-gap contrasts.
4. Study 2 fixed-content provenance contrasts for support and approval.
5. Study 3 working logistic model, marginal approval probabilities, net outcome equalization, gap-level conversion loss, and covariance / graph-sensitivity analyses.
6. Study 4 generic-referenced support contrasts and descriptive secondary outcomes.
7. Figure-source data and supplementary-table results.

## Analysis principles

- AI assignment is defined by randomized **access** to the study interface, not by post-assignment uptake of model suggestions.
- Baseline advocacy capacity is measured from objectively scored pre-treatment sources; self-efficacy and structural-position variables are kept separate.
- Claim quality, downstream support / approval, and post-decision attribution measures are treated as distinct outcomes.
- Post-decision attribution measures are descriptive and are not interpreted as causal mediators.
- Study 3 uses the realized writer-message-evaluator graph. Reported graph irregularities are retained and addressed in covariance and graph-sensitivity analyses.
- The studies were not preregistered; focal / secondary labels are an ex post reporting hierarchy rather than a preregistered confirmatory family.

## AI-assisted writing intervention

The AI-assisted writing condition used OpenAI GPT-4.1 mini, model snapshot `gpt-4.1-mini-2025-04-14`, accessed through the OpenAI API from 15 January to 18 March 2026. Generation parameters were fixed at temperature = 0.20, top_p = 1.00, maximum output tokens = 450, frequency penalty = 0, and presence penalty = 0.

The study interface allowed up to four user turns and imposed a 450-token limit per model reply. It provided no web browsing, external retrieval, hidden participant profile, persistent conversational memory, or researcher-supplied biography. The complete system instruction is provided in `prompts/system_prompt.txt`.

## Data protection

Publicly shared analysis files are de-identified. Direct identifiers, platform account identifiers, disclosive free-text fields, and other information restricted by consent or ethics requirements are not included.

## Citation

Please cite the associated manuscript and the archived repository release when using these materials.
