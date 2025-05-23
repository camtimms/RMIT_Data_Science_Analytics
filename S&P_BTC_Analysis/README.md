# S&P 500 and Bitcoin Price Analysis

A comprehensive statistical analysis examining the relationship between S&P 500 and Bitcoin prices over a 6-year period (2018-2024).

## 📊 Project Overview

This project analyzes the correlation and statistical properties of two major financial instruments:
- **S&P 500 (SPX)**: A stock market index tracking 500 large US companies
- **Bitcoin (BTC)**: The world's largest cryptocurrency

The analysis explores price movements, correlations, and statistical distributions to understand the relationship between traditional markets and cryptocurrency.

## 🎯 Key Findings

- **Strong positive correlation** (r = 0.8977) between S&P 500 and Bitcoin prices
- Bitcoin shows significantly higher volatility (71.6% vs 20.3% coefficient of variation)
- Both assets demonstrated resilience and growth following the 2020 COVID-19 market disruption
- Correlation varies over time, with some periods showing negative or weak correlation

## 📁 Repository Structure

```
S&P_BTC_Analysis/
├── README.md                    # This file
├── S&P_BTC_Analysis_R.Rmd      # Main R Markdown analysis file
├── S&P_BTC_Analysis_doc.html   # Compiled HTML report
├── BTC-USD-1.csv              # Bitcoin price data (2018-2024)
├── S&P 500-1.csv              # S&P 500 price data (2018-2024)
└── packages.bib               # Bibliography for R packages used
```

## 🔧 Technical Requirements

### R Packages Required
- `readr` - Data import
- `dplyr` - Data manipulation
- `tidyr` - Data tidying
- `ggplot2` - Data visualization
- `timetk` - Time series analysis

### Installation
```r
install.packages(c("readr", "dplyr", "tidyr", "ggplot2", "timetk"))
```

## 📈 Analysis Components

### 1. Descriptive Statistics
- Central tendency measures (mean, median, mode)
- Variability measures (standard deviation, range)
- Comparative analysis between datasets

### 2. Time Series Visualization
- Individual price trend analysis
- 6-month rolling correlation analysis
- Pattern identification and interpretation

### 3. Correlation Analysis
- Overall correlation coefficient calculation
- Scatter plot visualization with trend lines
- Time-based correlation variations

### 4. Distribution Analysis
- Normality testing using histograms
- Comparison with theoretical normal distributions
- Statistical interpretation of distributions

## 🚀 How to Run the Analysis

1. **Clone the repository**
   ```bash
   git clone [your-repo-url]
   cd S&P_BTC_Analysis
   ```

2. **Open R/RStudio and install required packages**
   ```r
   install.packages(c("readr", "dplyr", "tidyr", "ggplot2", "timetk"))
   ```

3. **Run the analysis**
   - Open `S&P_BTC_Analysis_R.Rmd` in RStudio
   - Click "Knit" to generate the full report
   - Or run chunks individually for step-by-step analysis

4. **View results**
   - Open `S&P_BTC_Analysis_doc.html` in your browser for the compiled report

## 📊 Data Sources

- **S&P 500 Data**: Historical daily closing prices (August 2018 - August 2024)
- **Bitcoin Data**: Historical daily adjusted closing prices (August 2018 - August 2024)

*Note: Data files are included in the repository for reproducibility*

## 🔍 Key Visualizations

The analysis includes several important visualizations:
- Time series plots showing price trends over 6 years
- Correlation heatmap by 6-month periods
- Scatter plots demonstrating the linear relationship
- Distribution histograms compared to normal distributions

## 📚 Methodology

This analysis employs several statistical techniques:
- **Pearson correlation coefficient** for relationship strength
- **Rolling correlation analysis** for temporal variations
- **Descriptive statistics** for data characterization
- **Distribution analysis** for normality assessment

## 🤖 AI Tools Acknowledgment

This project utilized AI assistance (ChatGPT) for:
- Code optimization and debugging
- Function documentation and parameter understanding
- Advanced visualization techniques
- Statistical interpretation guidance

All AI-generated content was thoroughly reviewed, tested, and integrated with understanding.

## 🎓 Academic Context

This project was completed as part of MATH1324 Applied Analytics coursework, demonstrating:
- Statistical analysis skills
- R programming proficiency
- Data visualization techniques
- Financial data interpretation
- Academic research methodology

## 📄 License

This project is for educational purposes. Data usage follows fair use principles for academic research.

## 👤 Author

**Campbell Timms** (s3720784)  
*Statistical Analysis of Financial Markets*

---

*For detailed analysis results, statistical interpretations, and comprehensive visualizations, please refer to the compiled HTML report.*
