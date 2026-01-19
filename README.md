# Life Expectancy Prediction Dataset

## Overview

This dataset contains comprehensive county-level data for life expectancy prediction across the United States. The dataset integrates demographic, socioeconomic, environmental, and atmospheric variables to support machine learning models for predicting mean life expectancy at the county level.

## File Information

- **Filename**: `final_combined_all_variables.csv`
- **Size**: 57 MB
- **Records**: 24,487 county-year observations
- **Variables**: 151 features

## Data Structure

### Geographic Identifiers
- County name
- State
- FIPS code

### Target Variable
- Mean Life Expectancy (years)

### Socioeconomic Variables (12)
- Poverty Rate
- High School Degree or Higher (%)
- Bachelor's Degree or Higher (%)
- Median Age
- Gini Index
- Disability Rate
- Total Population
- Median Household Income
- Unemployment Rate
- White Population (%)
- Hispanic Population (%)
- Black Population (%)

### Housing and Transportation (3)
- Households with No Vehicle (%)
- Rent Burden (+50% of Household Income)
- Single Mother Families (%)

### Atmospheric and Environmental Variables (87)

#### Temperature and Humidity
- 2m dew point temperature
- 2m temperature
- Wet bulb temperature
- Relative humidity
- Specific humidity

#### Aerosols and Particulate Matter
- Black carbon AOD at 550 nm
- Dust AOD at various size ranges
- Organic matter AOD at 550 nm
- PM₁, PM₂.₅, PM₁₀ concentrations
- Sea salt AOD at 550 nm
- Sulphate AOD at 550 nm
- Total AOD at multiple wavelengths (469-1240 nm)

#### Atmospheric Gases
- Carbon monoxide
- Ethane
- Formaldehyde
- Hydrogen peroxide
- Hydroxyl radical
- Isoprene
- Methane
- Nitric acid
- Nitrogen dioxide
- Nitrogen monoxide
- Ozone
- Peroxyacetyl nitrate
- Propane
- Sulphur dioxide

#### Geophysical Variables
- Land-sea mask
- Mean sea level pressure
- Surface geopotential
- Surface pressure
- Total column water vapour
- Snow albedo
- Snow depth
- Leaf area index (high and low vegetation)
- 10m wind speed

#### Vertically Integrated Aerosol Masses
- Dust aerosol (multiple size ranges)
- Black carbon aerosol (hydrophilic and hydrophobic)
- Organic matter aerosol (hydrophilic and hydrophobic)
- Sea salt aerosol (multiple size ranges)
- Sulphate aerosol
- Sulphur dioxide

### Frequency of Threshold Exceedance (FoT) Variables (22)
Percentage of time pollutants exceed 75th percentile or regulatory thresholds:
- Air pollutants: CO, ethane, formaldehyde, NO₂, NO, O₃, SO₂
- Particulate matter: PM₁, PM₂.₅, PM₁₀
- EPA threshold exceedances for PM₂.₅ and PM₁₀
- Temperature extremes (above 90°F, below 0°C)

### Livestock Density Variables (8)
County-level livestock counts:
- Buffalo
- Cattle
- Chicken
- Duck
- Goat
- Horse
- Pig
- Sheep

## Temporal Coverage

The dataset includes observations across multiple years, with the Year variable indicating the temporal dimension of each record.

## Data Sources

This dataset combines:
- Demographic and socioeconomic data from US Census and related sources
- Atmospheric reanalysis data from CAMS (Copernicus Atmosphere Monitoring Service)
- Environmental variables from ECMWF ERA5 reanalysis

## Use Cases

- County-level life expectancy prediction
- Environmental health impact assessment
- Socioeconomic determinants of health analysis
- Air quality and mortality research
- Feature importance analysis for public health policy

## Notes

- Missing values may exist for certain variables depending on data availability
- Atmospheric variables represent annual or seasonal aggregates
- FIPS codes enable geographic joins with other county-level datasets
- FoT (fraction of time) variables capture temporal variability in exposure patterns 
