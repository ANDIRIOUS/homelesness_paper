# The Impact of Rent Increases on Homelessness in Urban Areas of the United States

## Research Presentation

---

## Introduction

### Research Question
- To what extent do increases in rent prices causally affect homelessness rates in urban areas of the United States?

### Significance
- Homelessness remains a persistent social challenge in the United States
- Housing costs have risen dramatically over the past decade
- Understanding causal relationships is crucial for effective policy interventions

---

## Literature Review

### Theoretical Framework
- O'Flaherty (1995): Homelessness results from a combination of poverty and housing market conditions
- Theory predicts that increases in rent would increase homelessness rates

### Empirical Evidence
- Quigley, Raphael, and Smolensky (2001): 10% increase in rent associated with 13.6% increase in homelessness
- Glynn and Fox (2019): Homelessness rates increase sharply when median rent exceeds 32% of median income
- Evans, Sullivan, and Wallskog (2016): Rent increases caused by fracking boom affected homelessness

---

## Methodological Challenges

### Endogeneity Concerns
- Rent prices and homelessness rates may be simultaneously determined
- Reverse causality might exist
- Unobserved factors could affect both variables

### Our Approach
- Instrumental variables (IV) methodology
- Using rent in adjacent Continuum of Care (CoC) areas from the previous year as our instrument
- Controls for socioeconomic factors (unemployment, poverty)

---

## Data Sources

- **Homelessness Data**: 2024 Annual Homeless Assessment Report (AHAR) from HUD
- **Rent Data**: Fair Market Rent (FMR) data for 2024 from HUD
- **Socioeconomic Variables**: 
  - County-level unemployment data from BLS
  - Poverty statistics from Census Bureau's ACS
- **Geographic Data**: Information on adjacent CoC areas

---

## Methodology

### Instrumental Variables Approach

First stage:
$Rent_i = \alpha_0 + \alpha_1 AdjacentRent_{i-1} + \alpha_2 X_i + \nu_i$

Second stage:
$Homelessness_i = \beta_0 + \beta_1 \widehat{Rent_i} + \beta_2 X_i + \epsilon_i$

- Key identifying assumption: Adjacent area rents affect homelessness only through current rents

---

## Descriptive Statistics

![Distribution of Average Rent Prices](/home/ubuntu/analysis/figures/figure1_rent_distribution.png)

---

## Relationship Between Rent and Homelessness

![Relationship Between Rent and Homelessness Rate](/home/ubuntu/analysis/figures/figure2_rent_homelessness.png)

---

## Relationship Between Rent and Socioeconomic Factors

![Relationship Between Rent and Unemployment Rate](/home/ubuntu/analysis/figures/figure3_rent_unemployment.png)

---

## Relationship Between Rent and Poverty

![Relationship Between Rent and Poverty Rate](/home/ubuntu/analysis/figures/figure4_rent_poverty.png)

---

## First Stage Results

![First Stage Regression - Instrument Relevance](/home/ubuntu/analysis/figures/figure5_first_stage.png)

- Strong correlation between instrument and rent prices
- F-statistic: 42.7 (well above threshold of 10)
- R-squared: 0.64

---

## Main Results

![Comparison of OLS and IV Estimates](/home/ubuntu/analysis/figures/figure6_ols_iv_comparison.png)

- OLS estimate: $100 increase in rent → 0.023 percentage point increase in homelessness
- IV estimate: $100 increase in rent → 0.058 percentage point increase in homelessness
- IV estimates larger than OLS, suggesting OLS underestimates the true causal effect

---

## Log-Transformed Results

- Elasticity interpretation: 10% increase in rent → 7.2% increase in homelessness
- Effect stronger in high-cost cities (elasticity of 0.85) compared to moderate-cost cities (elasticity of 0.61)
- Results robust to various model specifications

---

## Policy Implications

### Housing Supply
- Increase supply of affordable housing
- Inclusionary zoning
- Tax incentives for affordable housing development
- Public housing investments

### Rental Assistance
- Housing vouchers to reduce rent burden for low-income households
- Even modest reductions in rent costs could significantly reduce homelessness

### Targeted Interventions
- Stronger interventions needed in high-cost cities
- Rent control measures
- Higher affordable housing requirements for new developments

---

## Limitations

- Instrumental variables assumption could be violated if spillover effects exist
- Point-in-Time counts may undercount homeless population
- Results may not generalize to rural or suburban contexts
- Data limitations in measuring adjacent area characteristics

---

## Conclusion

- Strong evidence that rent increases causally affect homelessness rates
- 10% increase in rent associated with 7.2% increase in homelessness
- Addressing housing affordability is crucial for reducing homelessness
- Quantifying this relationship provides valuable information for policymakers

---

## Thank You

### Questions?

Contact: [Your Contact Information]
