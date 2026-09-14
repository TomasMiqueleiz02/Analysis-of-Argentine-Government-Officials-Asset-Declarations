# Analysis-of-Argentine-Government-Officials-Asset-Declarations

## Overview

Comprehensive exploratory data analysis (EDA) of public asset declarations (Declaraciones Juradas) from government officials in Buenos Aires (GCABA), following the **CRISP-DM** methodology.

This project investigates wealth distribution patterns, asset composition, and financial behavior among high-ranking government officials.

## Key Findings

📊 **Main Insights:**
- **Wealth concentration:** Majority of wealth held in **cash and deposits** (~70%), not invested in real estate
- **Outliers identified:** Small fraction of officials with significantly higher patrimonial wealth
- **Jurisdictional patterns:** Specific government agencies concentrate more high-net-worth officials
- **Asset preference:** Officials prefer liquid assets (cash, bank deposits) over real estate investments
- **Hierarchical difference:** High-ranking authorities show 3-4x median wealth compared to regular officials

## Dataset

**Source:** Official GCABA asset declarations  
**Time Period:** 2020-2023  
**Records:** 500+ government officials  
**Variables:** 14+ features including jurisdictions, positions, asset types, wealth composition

### Data Structure
- `patrimonio_total`: Total declared assets (target variable)
- `total_dinero_efectivo`: Cash holdings
- `total_depositos`: Bank deposits
- `total_b_inmuebles`: Real estate value
- `jurisdiccion`: Government agency
- `cargo`: Official position/role
- `autoridad_superior`: Binary indicator of hierarchy level

## Methodology

This analysis follows the **CRISP-DM** framework (Cross-Industry Standard Process for Data Mining):

1. **Business Understanding:** Analyze wealth distribution in government
2. **Data Understanding:** Explore structure, quality, and distributions
3. **Data Preparation:** Cleaning, handling nulls, outlier treatment
4. **EDA:** Descriptive statistics, correlations, visualizations
5. **Modeling:** Predictive analysis of wealth patterns (optional)

## Analysis Sections

### 1. Data Quality Assessment
- Null value analysis
- Duplicate detection
- Data type validation
- Standardization of categorical values

### 2. Descriptive Statistics
- Measures of central tendency (mean, median, mode)
- Dispersion analysis (std, IQR, quartiles)
- Distribution shapes
- Outlier detection using IQR method

### 3. Visual Analysis
- Distribution of wealth by jurisdiction
- Wealth by government position
- Asset composition breakdown
- Outlier concentration patterns
- Correlation heatmaps

### 4. Business Insights
- Wealth concentration metrics
- Asset allocation patterns by hierarchy
- Jurisdictional wealth comparisons
- Risk indicators for financial analysis

## Tools & Libraries

```python
pandas          # Data manipulation
numpy           # Numerical operations
matplotlib      # Static visualizations
seaborn         # Statistical graphics
scipy           # Statistical analysis
```

## Usage

### Run in Google Colab
```
1. Click on notebook in repository
2. Open with Google Colab
3. Execute cells sequentially
4. Dataset is loaded from GCABA public sources
```

### Local Usage
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scipy

# Run Jupyter
jupyter notebook Estudio_Declaraciones_Juradas.ipynb
```

## Key Visualizations

- **Boxplots:** Wealth distribution by jurisdiction and position
- **Violin plots:** Probability density of asset values
- **Heatmaps:** Correlation between asset types and total wealth
- **Bar charts:** Outlier concentration by agency
- **Pie charts:** Asset composition breakdown

## Project Team

- Tomás Miqueleiz
- Sebastián Fell
- Marcos Palacios
- Christian Tarnoski

**Institution:** Licenciatura en Ciencia de Datos - UGR (Universidad de la República del Plata)

## Deliverables

✓ **Entrega 1:** Problem formulation and data loading  
✓ **Entrega 2:** EDA and visualizations  
✓ **Entrega 3:** Modeling approach and recommendations  

## Conclusions

This analysis demonstrates how public asset declaration data can reveal significant patterns in wealth distribution within government structures. The predominance of liquid assets suggests either conservative financial strategy or deliberate wealth concealment concerns.

Potential applications:
- Government transparency audits
- Financial behavior prediction
- Corruption risk indicators
- Policy-making insights

## Notes

- All data is publicly available from official GCABA sources
- Analysis conducted following academic standards
- AI tools used for code structure only (see declaration in notebook)
- Full methodology explanation available in presentation videos

## License

Educational project - Public analysis of public data

---

**Last Updated:** 2024  
**Status:** Complete Analysis with 3 Deliverables
