# Diamond Pricing: Assessing the Impact of the 4C’s on Blue Nile Diamonds

**Group 8**: Jacob Kuchta, Emmanuel Leonce, Bardia Nikpour, Victor Ontiveros  
**Date**: March 24, 2024  

---

## Project Overview

This project investigates the relationship between a diamond's price and its key characteristics, commonly referred to as the "4C's":
1. **Cut**
2. **Color**
3. **Clarity**
4. **Carat**

Using a dataset of 1,214 diamonds sourced from [Blue Nile](http://bluenile.com), we analyze how each of these variables influences a diamond's price. The study employs descriptive statistics, visualizations, and regression models to derive meaningful insights.

---

## Contents
1. **Report Summary**
2. **High-Level Overview**
3. **Key Findings**
4. **Data Exploration**
   - Data Set and Variables
   - Visualizations for Price, Carat, Cut, Color, and Clarity
5. **Linear Regression Analysis**
6. **Conclusions**

---

## Report Summary

### High-Level Overview
This study aims to provide a clear understanding of what makes diamonds valuable by analyzing the 4C's:
- **Cut**: How well a diamond is shaped and polished to reflect light.
- **Color**: The degree of colorlessness in a diamond.
- **Clarity**: The presence of internal (inclusions) or external (blemishes) flaws.
- **Carat**: The weight of the diamond.

By analyzing these variables, we assess their individual and combined impact on the diamond's price.

---

## Key Findings
1. **Cut**: Superior cuts (e.g., Astor Ideal) significantly increase a diamond's price.
2. **Color**: Surprisingly, color does not have a major impact on price.
3. **Clarity**: Flawless (FL) diamonds are rare and command premium prices, but slight imperfections do not drastically affect price.
4. **Carat**: Carat weight strongly influences price, with a 1% increase in weight leading to approximately a 2% increase in price.

### Key Insight
Movies and media have created an undue emphasis on carat weight, while cut quality may be more influential in determining a diamond's beauty and value.

---

## Data Exploration

### Dataset
- **Source**: [Blue Nile](http://bluenile.com)
- **Size**: 1,214 diamonds
- **Key Variables**:
   - **Price**: The price of each diamond.
   - **Carat**: The weight of the diamond.
   - **Cut**: Categorical (e.g., Good, Very Good, Ideal, Astor Ideal).
   - **Color**: Categorical (D to J).
   - **Clarity**: Categorical (FL, IF, SI1, SI2, etc.).

### Visualizations and Summaries
- **Price**: Highly skewed distribution, transformed using log(price) for analysis.
- **Carat**: Positively skewed; log transformation applied.
- **Cut**: Astor Ideal diamonds tend to have the highest median prices.
- **Color**: Price distributions do not vary significantly across color grades.
- **Clarity**: FL diamonds are rare and expensive; lower clarity grades correspond with lower prices.

---

## Regression Analysis

### Initial Model: Price vs. Carat
- A linear relationship exists between carat and price but violates regression assumptions (heteroscedasticity).

### Transformed Model: log(Price) vs. log(Carat)
- The final regression model is:
   
   \[ \text{log(price)} = 8.5212 + 1.9440 \cdot \text{log(carat)} \]

- **Interpretation**: For every 1% increase in carat weight, the price of a diamond increases by approximately 1.94%.

---

## Conclusion
Our analysis highlights that while carat weight remains a dominant factor in determining a diamond's price, the cut quality plays a crucial role in enhancing its value. Consumers can make more informed decisions by balancing carat weight, cut, and clarity to achieve the best value for their investment.

---

## Tools and Libraries
- **Languages**: R
- **Libraries**: ggplot2, dplyr, tidyverse

---

## Acknowledgments
This project was completed as part of a team effort by **Group 8** for the course project: *Diamond Pricing Analysis*.

---

## Contact
For questions or further details about this project, please contact:  
**Emmanuel Leonce**  
**Email**: [deoleojr016@gmail.com]  
**Affiliation**: University of Virginia, Master's in Data Science

