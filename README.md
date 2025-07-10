# Water-Table-Dynamics-in-Coastal-Ecosystems

# Water Table Depth Modeling for *Rhizophora mangle* under Salinity Stress

This Mathematica notebook models the water table depth (WTD) dynamics for *Rhizophora mangle* (Red mangrove) under varying salinity conditions. The model accounts for the ecohydrological feedbacks among salinity, evapotranspiration, soil moisture retention, and hydraulic conductivity, with a focus on how salt stress affects root-zone hydrology.

## Overview

The model simulates:
- Salinity-dependent **evapotranspiration**
- Soil water retention via **matric potential functions**
- Water table fluctuations influenced by **lateral flow, root uptake**, and **climate forcing**
- Probability density functions (PDFs) of WTD under different salinity scenarios

It is parameterized for Taylor River conditions in the Florida Coastal Everglades.

## Key Features

- **Salinity-responsive ET function** based on plant salt tolerance  
- Dynamic calculation of soil moisture field capacity (`sfc`, `sfcc[C]`)
- Salinity-sensitive **water yield functions** (\( \beta(y), \beta_c(y, C) \))
- Analytic PDFs of water table depth with and without salinity effects
- Visualization of how salinity alters the shape of the WTD distribution

## File Contents

- `WTD_MainModel.nb`: Mathematica notebook containing all model equations, parameter settings, and plots
- Output includes:
  - `pYNC[z, C]`: PDF of WTD for given salinity \( C \)
  - Normalized plots for varying salinity levels (e.g., 12, 16, 35 g/L)
  - ET vs. salinity relationship: `ETRedMangrove`

## Key Parameters

| Parameter        | Description                                        |
|------------------|----------------------------------------------------|
| `ETmaxC[C]`      | Potential ET as a function of salinity             |
| `sfcc[C]`        | Soil moisture field capacity affected by salinity  |
| `ycc[C]`         | Critical depth under salinity                      |
| `\[\beta]c[y, C]`| Yield function with salinity stress                |
| `pYNC[z, C]`     | PDF of WTD for salinity \( C \)                    |

## Example Output

- Comparative WTD distributions across salinity conditions (e.g., 12 g/L vs 35 g/L)
- Visualization of ET suppression due to salinity stress

## Dependencies

- Wolfram Mathematica 12 or higher
- No external packages required

## Contact

**Saverio Perri, Ph.D.**  
Department of Environmental Sciences  
University of California, Riverside  
[saveriop@ucr.edu](mailto:saveriop@ucr.edu)  
[Google Scholar](https://scholar.google.com/citations?user=ot-86YoAAAAJ)

