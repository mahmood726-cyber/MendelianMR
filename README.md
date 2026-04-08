# MendelianMR

Browser-based Mendelian Randomization analysis tool.

## Methods
- **IVW** (fixed + random effects) — primary estimate
- **MR-Egger** — directional pleiotropy detection via intercept test
- **Weighted Median** — robust when ≥50% weight from valid instruments
- **Simple Median** — robust when ≥50% instruments valid
- **MR-PRESSO** — outlier detection with global test + Bonferroni correction

## Diagnostics
- Cochran's Q, I² heterogeneity
- F-statistics for instrument strength
- Leave-one-out sensitivity analysis

## Plots
- Scatter (SNP-exposure vs SNP-outcome with method lines)
- Forest (individual Wald ratios + summary diamonds)
- Funnel (asymmetry detection)
- Leave-one-out

## Example Datasets
- LDL → CHD (28 SNPs)
- BMI → T2DM (14 SNPs)
- SBP → Stroke (8 SNPs)
- CRP → CHD (5 SNPs, pleiotropy example)

## Live Demo
https://mahmood726-cyber.github.io/MendelianMR/

## Author
Mahmood Ahmad, Tahir Heart Institute
