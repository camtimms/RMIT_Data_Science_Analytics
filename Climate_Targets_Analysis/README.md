# Climate Targets Analysis: Will Australia Meet its 2030 Greenhouse Gas Emissions Targets?

**Author:** Campbell Timms (S3720784)  
**Course:** Applied Analytics (MATH1324)  
**Institution:** RMIT University

## Project Overview

This project investigates whether Australia will meet its ambitious 2030 greenhouse gas emissions reduction targets through comprehensive data analysis, statistical modeling, and hypothesis testing. Using official government data sources, the analysis employs linear regression modeling to forecast emissions trends and evaluate the likelihood of achieving climate commitments.

## Research Question

**Will Australia meet its 2030 greenhouse gas emissions targets?**

Australia has committed to reducing greenhouse gas emissions by 43% below 2005 levels by 2030 under the Climate Change Act (2022), as part of its broader Net Zero Plan for 2050.

## Key Findings

- **Prediction:** Australia will likely miss its 2030 emissions target based on current trends
- **Projected Emissions (2030):** 94.26 Mt CO2-e
- **Target Level:** 88.16 Mt CO2-e (43% below 2005 levels)
- **Statistical Confidence:** 95% confidence interval [93.42, 95.10] Mt CO2-e
- **Hypothesis Test Result:** Rejected null hypothesis - predicted emissions will exceed target levels

## Data Sources

### 1. National Greenhouse Gas Inventory Quarterly Update (September 2023)
- **Source:** Department of Climate Change, Energy, the Environment and Water (DCCEEW)
- **Coverage:** Quarterly emissions data from 2004-2023
- **Industries:** Electricity, Transport, Agriculture, Industrial Processes, Land Use Change, and more
- **Format:** Actual, seasonally adjusted, and trend data in Mt CO2-e

### 2. Energy Account Australia (2021-22 Financial Year)
- **Source:** Australian Bureau of Statistics (ABS)
- **Coverage:** Energy supply and consumption by source (2011-2022)
- **Key Metrics:** Renewable energy output in Petajoules (PJ)
- **Focus:** Solar, wind, and hydro energy trends

## Methodology

### Statistical Analysis
1. **Descriptive Statistics:** Industry-wise emissions analysis and renewable energy trends
2. **Linear Regression Modeling:** Time-series prediction model for total emissions
3. **Hypothesis Testing:** One-sample t-test with 95% confidence intervals
4. **Model Validation:** Residual analysis and Q-Q plots for assumption checking

### Key Assumptions
- Linear relationship between time and emissions continues
- Normal distribution of residuals (tested via Q-Q plots)
- Homoscedasticity (constant variance of residuals)

## Results & Insights

### Emissions Trends
- **Overall Reduction:** 25.4% below 2005 levels as of September 2023
- **Major Contributors to Reduction:**
  - Land Use, Land Use Change and Forestry (LULUCF): Significant carbon sequestration
  - Electricity: Renewable energy transition reducing emissions
  - Other industries showing minimal change

### Renewable Energy Progress
- **Growth Rate:** 19% increase in renewable energy (2021-2022)
- **Market Share:** 30% of domestic electricity use
- **Source Breakdown:**
  - Solar: +25% (125 PJ)
  - Wind: +17% (105 PJ)
  - Hydro: +12% (61 PJ)

### Future Projections
- **2030 Forecast:** Will narrowly miss target by ~6 Mt CO2-e
- **2050 Outlook:** Current trends insufficient for net-zero emissions
- **Critical Dependencies:** Continued growth in renewable electricity and land-based carbon sequestration

## File Structure

```
Climate_Targets_Analysis/
├── README.md                                          # This file
├── Climate_Targets_Analysis.Rmd                      # Main R Markdown analysis
├── Climate_Targets_Analysis_pres.html               # HTML presentation output
├── styles.css                                       # Custom CSS styling
├── Data Files/
│   ├── nggi-quarterly-update-sept-2023-data-sources.xlsx
│   └── 46040DO0001_2021_22.xlsx
└── Images/
    ├── wind_turbine.jpg                             # Background image
    ├── 2022-climate-action.png                     # Climate action signing
    ├── rudd-kevin.jpg                              # Kevin Rudd Kyoto Protocol
    ├── LULUC.png                                   # Land use change diagram
    └── lighttail.png                               # Distribution illustration
```

## Technical Requirements

### R Packages Used
```r
library(ggplot2)      # Data visualization
library(dplyr)        # Data manipulation
library(tidyr)        # Data tidying
library(knitr)        # Report generation
library(readxl)       # Excel file import
library(lubridate)    # Date handling
library(ggrepel)      # Enhanced plot labeling
library(patchwork)    # Multiple plot arrangement
```

### System Requirements
- R version 4.0+
- RStudio (recommended)
- Required packages (install via `install.packages()`)

## Usage Instructions

1. **Clone/Download** the project repository
2. **Install Dependencies:**
   ```r
   install.packages(c("ggplot2", "dplyr", "tidyr", "knitr", 
                      "readxl", "lubridate", "ggrepel", "patchwork"))
   ```
3. **Set Working Directory** to the project folder
4. **Run Analysis:**
   ```r
   # Open and knit the R Markdown file
   rmarkdown::render("Climate_Targets_Analysis.Rmd")
   ```
5. **View Results** in the generated HTML presentation

## Key Visualizations

The analysis includes several important visualizations:
- **Total Emissions Timeline:** Historical trends with future projections
- **Industry Breakdown:** Emissions by sector over time
- **Renewable Energy Growth:** Solar, wind, and hydro trends
- **Statistical Diagnostics:** Residual plots and Q-Q plots for model validation

## Limitations & Future Work

### Model Limitations
- Linear regression assumes continued linear trends
- Limited to two-variable relationships (time vs. emissions)
- Q-Q plots indicate light-tailed distribution affecting normality assumption

### Suggested Improvements
- **Multi-variable Models:** Include economic, policy, and technology variables
- **Industry-Specific Analysis:** Separate models for each emission sector
- **Non-linear Modeling:** Account for potential policy inflection points
- **Scenario Analysis:** Model different policy intervention scenarios

## Policy Implications

The analysis suggests that meeting 2030 targets requires:
1. **Accelerated Renewable Transition:** Beyond current 83% renewable electricity target
2. **Enhanced Land Use Management:** Continued forest growth and carbon sequestration
3. **Industry-Specific Interventions:** Address sectors with stagnant emissions
4. **Policy Innovation:** New approaches for hard-to-abate sectors

## References

Key data sources and literature:
- Department of Climate Change, Energy, the Environment and Water (DCCEEW)
- Australian Bureau of Statistics (ABS)
- United Nations Framework Convention on Climate Change (UNFCCC)
- Climate Change Act 2022 (Australia)
- Paris Agreement (2015)

## Contact

For questions about this analysis or to request additional information:
- **Student:** Campbell Timms
- **Student ID:** S3720784
- **Course:** MATH1324 Applied Analytics
- **Institution:** RMIT University

---

*This analysis was completed as part of the Applied Analytics course at RMIT University. The findings represent academic research and should not be considered as official policy recommendations.*
