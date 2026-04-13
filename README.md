# Pokémon Win Percentage Analysis

**Authors:** Justin Mundell, Violeta S.

---

## Overview
This project analyzes Pokémon battle data to understand how different characteristics impact win percentage. Using a dataset of ~800 Pokémon and ~50,000 battles, we evaluate how factors such as type, number of types, generation, and legendary status influence performance. :contentReference[oaicite:0]{index=0}

---

## Objectives
- Determine whether Pokémon type impacts win percentage  
- Compare performance of single-type vs dual-type Pokémon  
- Analyze the effect of generation on battle outcomes  
- Evaluate the impact of legendary status  

---

## Dataset
- ~800 Pokémon with attributes (type, stats, generation, legendary status)  
- ~50,000 battle records used to compute win percentage :contentReference[oaicite:1]{index=1}  

---

## Methods
- Data preprocessing and win percentage calculation  
- Hypothesis testing:
  - ANOVA (initial approach)
  - Kruskal-Wallis (non-parametric alternative)
  - Mann-Whitney U Test  
- Post-hoc analysis:
  - Pairwise t-tests  
  - Dunn’s test (Bonferroni correction)  
- Assumption checks:
  - Normality (Shapiro-Wilk)
  - Homogeneity of variance (Levene’s Test)  

---

## Key Findings

### Type Analysis
- Significant differences exist in win percentage across Pokémon types  
- **Bug-type Pokémon had significantly lower win rates** compared to several other types  
- Some types (e.g., Dark, Electric, Fire) showed higher median win percentages  

### Number of Types
- Dual-type Pokémon performed better:
  - **Single-type median:** ~43%  
  - **Dual-type median:** ~55%  
- Statistically significant difference confirmed via Mann-Whitney U Test  

### Generation
- No statistically significant difference in win percentage across generations  
- Median win rates were relatively similar across all generations  

### Legendary Status
- Strongest effect observed:
  - **Legendary median:** ~82%  
  - **Non-legendary median:** ~46%  
- Legendary Pokémon significantly outperform others in battles  

---

## Results
- Statistical tests consistently showed:
  - Type and number of types significantly impact performance  
  - Generation has minimal effect  
  - Legendary status has a large impact  

---

## Tech Stack
- R  
- Statistical modeling  
- Hypothesis testing  
- Data visualization  

---

## Notes
This project highlights the importance of choosing appropriate statistical methods when assumptions are violated. Non-parametric tests were used when normality and variance assumptions were not satisfied.

---
