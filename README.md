# Optimising IEA Questionnaire Scales for Length and Comparability

This repository contains the code and derived outputs for preliminary analyses supporting the project **Optimising IEA Questionnaire Scales for Length and Comparability**, prepared for the IEA Research and Development Fund Call 6.

The preliminary work examines whether selected IEA questionnaire scales can be shortened while retaining close agreement with the corresponding official scale scores and preserving important country-level and achievement-related results.

## Preliminary analyses

The analyses use four student questionnaire scales from four IEA studies.

| Study | Scale | Construct |
| --- | --- | --- |
| ICILS 2023 | S_LRNINTO | Learning about internet-related tasks outside school |
| TIMSS 2023 Grade 8 | BSBGSLM | Students Like Learning Mathematics |
| PIRLS 2021 | ASBGSLR | Students Like Reading |
| ICCS 2022 | S_CITEFF | Students' Citizenship Self-Efficacy |

The preliminary procedure ranks source items in calibration systems and evaluates progressively shorter subsets in held-out systems. A weighted individual-level correlation of 0.95 with the official full scale is used as the preliminary recovery criterion.

These analyses are intended to establish feasibility and motivate the proposed research. They do not implement the complete methodology planned for the funded project, which will additionally address measurement invariance, construct-facet coverage, trend anchoring, survey-design-aware optimisation and cross-cycle validation.

## Main preliminary findings

The four scales showed different levels of reducibility.

TIMSS 2023 Grade 8 BSBGSLM was reduced from seven items to three while reaching a held-out correlation of 0.9547 with the official full scale.

ICCS 2022 S_CITEFF was reduced from seven items to five and reached a held-out correlation of 0.9609.

ICILS 2023 S_LRNINTO required all six source items to reach the preliminary recovery criterion, with a held-out correlation of 0.9506.

PIRLS 2021 ASBGSLR did not reach the 0.95 criterion even when all ten source items were retained in the reconstructed score. The resulting correlation with the official scale was 0.9325.

The variation across studies is central to the proposed project. It suggests that questionnaire-scale reduction should be evaluated scale by scale rather than through a fixed reduction rule.

## Repository structure

```text
.
├── analysis/
│   ├── README.md
│   └── IEA_RD6_Preliminary_Results.Rmd
│
├── outputs/
│   ├── README.md
│   ├── Preliminary_results_summary.csv
│   ├── Table_S1_items_per_scale.csv
│   ├── Figure_S2_omission_by_position.csv
│   ├── Figure_S2_omission_by_position.pdf
│   ├── Figure_S3_validation_correlations.csv
│   ├── Figure_S3_correlation_by_subset_size.pdf
│   ├── Figure_S4_country_means.csv
│   ├── Figure_S4_country_means_short_vs_full.pdf
│   ├── Figure_S5_country_mean_differences.csv
│   ├── Figure_S5_country_mean_differences.pdf
│   ├── Figure_S6_achievement_associations.csv
│   └── Figure_S6_achievement_associations.pdf
│
├── documentation/
│   └── README_data.md
│
├── CITATION.cff
├── LICENSE
├── .gitignore
└── README.md
