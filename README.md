# Project Title: The Effect of Farmlands on Surrounding Areas

## Project Overview

This project investigates the impact of farmlands, specifically their classification as commercial or non-commercial, on the surrounding areas' socioeconomic status. Utilizing advanced spatial data analysis methods and data sourced from both the U.S. Census Bureau and the U.S. Department of Agriculture (USDA), we aim to identify correlations between farmland density and socioeconomic indicators.

## Key Objectives

- Analyze the relationship between different types of farmlands (commercial and non-commercial) and surrounding socioeconomic factors.
- Establish methods for categorizing farmlands based on rural and urban area types.
- Identify potential applications for demographic research, policy development, and vertical farming strategies.

## Data Sources

1. **NSES Indicator Data**: Extracted from the U.S. Census Bureau’s 2011-2015 American Community Survey, this summative index describes socioeconomic status by census tracts.
2. **Cropland Raster Layer**: Time-enabled raster data sourced from the National Agricultural Statistics Service (NASS).
3. **USDA Sales Data**: Information on sales and equipment derived from the USDA Census of Agriculture.

## Methodology

1. **Data Preparation**:

   - Extract socioeconomic indicators (e.g., household income, unemployment rate, poverty rate) from the NSES dataset.
   - Integrate cropland data using geospatial analysis to calculate density by census tract.
   - Import and process USDA sales data to classify farmlands as commercial or non-commercial.

2. **NSES Indicator Calculation**:
   The NSES is calculated using the formula:\
   NSES = log(median household income) + (-1.129 \* (log(percent of female-headed households))) + (-1.104 \* (log(unemployment rate))) + (-1.974 \* (log(percent below poverty))) + .451\*((high school grads)+(2\*(bachelor's degree holders)))

3. **Classification of Farmlands**:

   - **Commercial Farmlands**: Defined by sales greater than \$350,000 as per USDA standards.
   - **Non-Commercial Farmlands**: Farmlands with sales below this threshold.

4. **Spatial Analysis**:

   - Calculate cropland density for each tract.
   - Classify areas into cropland and non-cropland (lowest 5% by density).
   - Map socioeconomic data against cropland classification to observe potential impacts.

5. **Statistical Testing**:

   - Perform hypothesis testing to compare socioeconomic impacts:
     - P-value for Non-Cropland vs. Non-Commercial Cropland: 0.008
     - P-value for Non-Cropland vs. Commercial Cropland: 1.23e-6

## Results Summary

- The analysis revealed significant differences in socioeconomic status between areas dominated by non-commercial and commercial farmlands.
- Commercial farmlands correlate with higher positive socioeconomic indicators compared to non-commercial or non-cropland regions.

## Potential Applications

- **Demographic Research**: Understanding socioeconomic trends in agricultural regions.
- **Policy Development**: Informing agricultural policies and community planning.
- **Vertical Farming Initiatives**: Identifying opportunities for sustainable development in urban areas.

## Visuals
[Refer to the project presentation] (https://github.com/R1chZhang/Socioeconomic-Impact-from-Farmland-Distribution/blob/main/Results_Presentation.pdf)

## Conclusion

This project underscores the complex relationship between farmland type and socioeconomic status, offering insights for further research and policy considerations.

## References

1. Droller, Federico, and Martin Fiszbein. “Staple Products, Linkages, and Development: Evidence from Argentina.” *The Journal of Economic History* (2021).
2. Wang, S., Bai, X., Zhang, X., et al. “Urbanization can benefit agricultural production with large-scale farming in China.” *Nature Food* 2, 183–191 (2021).
3. Miles, Jeremy and Weden, Margaret; Lavery, Diana; Escarce, José; Kathleen Cagney; Shih, Regina. 2016. “Constructing a Time-Invariant Measure of the Socio-Economic Status of U.S. Census Tracts.” Journal of Urban Health, vol. 93, issue no.1, pp. 213-232.
