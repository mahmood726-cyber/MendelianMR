# E156 Protocol — MendelianMR

**Project**: MendelianMR
**Created**: 2026-04-09
**Type**: methodological
**Estimand**: Causal odds ratio of exposure on outcome via genetic instruments
**Dashboard**: https://mahmood726-cyber.github.io/MendelianMR/

## E156 Body (155 words, 7 sentences)

Can browser-based Mendelian randomization replicate the causal inference pipeline traditionally requiring R or Stata packages? We implemented five MR methods — inverse-variance weighted (fixed and random effects), MR-Egger regression, weighted median, simple median, and MR-PRESSO outlier detection — as a single-file HTML application using JavaScript matrix algebra. Each method's estimator was coded from first principles: IVW as weighted regression through the origin, MR-Egger as weighted regression with intercept (InSIDE assumption), and weighted median via sorted Wald ratios with bootstrap standard errors (1,000 replicates, seeded PRNG). Applied to 28 LDL-cholesterol SNPs and coronary heart disease, the tool produces IVW OR, Cochran's Q heterogeneity, MR-Egger intercept test, F-statistics for instrument strength, and MR-PRESSO global and outlier tests with Bonferroni correction. Sensitivity analyses include leave-one-out IVW, scatter, forest, and funnel plots with method-specific regression lines. The tool fills a gap in browser-based causal inference, enabling MR analysis without software installation. This implementation is limited to two-sample summary-level MR and does not support multivariable MR or sample overlap corrections.
