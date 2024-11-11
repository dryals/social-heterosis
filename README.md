# social-heterosis
data, analysis, and results for an experiment on social heterosis in honey bees


## Publication: 

_Individual and social heterosis act independently in honey bee (Apis mellifera) colonies_

by: Ryals, D.K., Buschkoetter, A.C., J Krispn Given, and Harpur, B.A.


Pre-Print: https://doi.org/10.1093/jhered/esae043

## Analysis 

- `therm_assay.Rmd`: Complete analysis for the thermoregulation assay
- `immune_assay.Rmd`: Complete analysis for the immune challenge assay
     

## Data

- `therm_data/sensors`: raw data uploads from iButton sensors
    - within each file, serial numbers are in cell C1 and data begin on row 22 with timestamps (UTC) and temperature (C)
- `therm_data/ibkey.xlsx`: key to connect serial numbers for iButton sensors to experimental treatment and replication (see methods)
- `immune_data/observations.xlsx`: log of all observations over the course of the immune challenge assay
    - sheet 1 `removed`: all removed bees (dead or censored) including datetime (EDT), cup (replicate) ID, paint color of individual, status of removed individual (1 = dead, 0 = censored), count (for identical observations), observer initial, and note. Empty cells are considered `NA` (Not Applicable)
    - sheet 2 `cups`: data for each replication or "cup", including start datetime (EDT), end datetime (controls only), the assay ID and paint color for each included genotype (two for mixed trials, one for single trials), control status (1 = control), categorical variable "run" for all trials begun at the same time, and additional notes. Empty cells are considered `NA` (Not Applicable)
- `immune_data/id_key.xlsx`: key to link genotype ID's in `observations.xlsx` to replicate and treatment categories (see methods)

# Note

- The `figures` directory mentioned in code has been removed in accordance with publication copyright. Please see publication for complete figures.
    
