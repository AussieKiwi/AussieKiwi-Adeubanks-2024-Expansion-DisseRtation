# AussieKiwi-Adeubanks-2024-Expansion-DisseRtation
This is a repo (in the works) for the project "Adeubanks-2024-Expansion-DisseRtation" which attempts to reproduce and expand the repo "disseRtation" by adeubanks. 

This project expands upon Austin Eubanks' research of cognitive dissonance in the 2016 and 2020 elections by including ANES data from 2024.
For his written paper follow this [Link](https://osf.io/9frup/)
For the original github project follow this [Link](https://github.com/adeubanks/disseRtation.git)

**Scripts**
There are two scripts within the "scripts" folder which generally replace Eubanks original 2016 data with 2024 data. There are also some changes to the data points used. 

**Cleanup.R**
"Cleanup.R" processes the data from its raw format (i.e., exactly as exported from ANES, anes_timeseries_2020_spss_20220210.sav, and anes_timeseries_2024_spss_20250808.sav) and exports two data sets:
df_full.RDS is the dataset that has all of the useful/relevant data, including e.g., both the computed variables and the vairables that were used for the computation.
df_analysis.RDS is the dataset that is used for the primary analyses; it began with df_full.RDS then selected down to just the variables used in the manuscript.

**Analysis.R**
"Analysis.R" reads in df_analysis.RDS and does all the modeling, tabling, plotting, etc. that is reported in the manuscript.
