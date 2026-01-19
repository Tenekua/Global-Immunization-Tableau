# Global Immunization Coverage & Child Mortality (Tableau)

## Overview
This project is an interactive Tableau dashboard that integrates WHO/UNICEF immunization coverage estimates with World Bank under-5 mortality data to explore global vaccination trends and population health outcomes across countries and time.

The dashboard demonstrates end-to-end analytics skills including data normalization, multi-source integration, relational modeling, and interactive visualization design applied to real public health data.

## Live Dashboard (Tableau Public)
Tableau Public Profile:  
https://public.tableau.com/app/profile/tenekua.dugan  

## Key Questions Explored
- How does immunization coverage vary by country, vaccine type, and year?
- What global patterns emerge when comparing vaccine coverage to child mortality?
- How have coverage trends changed over time across different vaccines?

## Data Sources
- **WHO/UNICEF (WUENIC) immunization coverage estimates** — country, vaccine, year
- **World Bank** under-5 mortality indicator — country, year

> Note: Some vaccines show missing values in earlier years due to introduction timing, reporting gaps, or unavailable estimates.

## Data Preparation
- UNICEF data was delivered as multiple vaccine-specific worksheets in a single Excel file.
  - Combined worksheets using a UNION in Tableau
  - Used the Table Name field as the vaccine identifier
  - Pivoted year columns into a single Year field (long format)

- World Bank mortality data was delivered in wide format (one column per year).
  - Normalized using Excel Power Query (unpivot years into a single Year column)

- Integrated datasets in Tableau using relational modeling on:
  - ISO3 + Year

## Dashboard Views
- **Scatter Plot:** Vaccine coverage (%) vs under-5 mortality (country-level)
- **Map:** Global vaccine coverage by country
- **Time Trend:** Global average vaccine coverage over time (one line per vaccine)

## Skills Demonstrated
- Data cleaning and normalization (Power Query)
- Multi-sheet union modeling in Tableau
- Pivoting and unpivoting time-series data
- Relational data modeling with multiple sources
- Interactive dashboard design and analytical storytelling
- Public health data interpretation

## How to Use
1. Open the Tableau Public dashboard.
2. Use the Vaccine and Year filters to explore trends.
3. Hover over marks for country-level tooltips with coverage and mortality values.

## Limitations & Future Enhancements
- Add data completeness indicators by vaccine and year
- Add regional comparison dashboards
- Integrate additional outcome measures (e.g., measles incidence)
- Include socioeconomic covariates for deeper modeling

## Author
**Tenekua Dugan**  
LinkedIn: https://www.linkedin.com/in/tenekuadugan  
Tableau Public: https://public.tableau.com/app/profile/tenekua.dugan
