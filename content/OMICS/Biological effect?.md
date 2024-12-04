---
OMICS: "[[L3 Transcriptomics]]"
---
After normalizing the data and, if nessecary [[Batch correction|correcting]] it, the biological effect has to be validated statistically.

Three of the most important parameters for the statistical evaluation are:
1. **Fold change (FC)** - Ratio of gene expression levels between two conditions, usually $log_{2}(FC)$ is used.
   $$FC = \frac{Gene1_{ConditionA}}{Gene1_{ConditionB}}$$
2. **p-Value** - evaluates, whether the observed difference has an underlying cause or is just due to chance. A p-Value of 0.05 would represent a 5% chance that the difference is due to chance.
3. **False Discovery Rate (FDR/padj)** - With a higher amount of statistical comparisons the chance for a false positive (showing significance, although there is none) of the tests themselves increases. This multiple testing problem is addressed by analysis with FDR (normally FDR $\leq$ 0.01).

DESeq2 is a tool, that is able to perform data normalization and perform statistical tests to analyze whether there is a significant difference between sample groups.

---
Created: 2024-12-03 15:51