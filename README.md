# CELLDEX_nutrients
Data and code for the manuscript:
Costello et al. *Global patterns and controls of nutrient immobilization on decomposing cellulose in riverine ecosystems*.


Data files include:
  * `stripCNP.csv`
  * `waterquality.csv`
  * `decomp_k.csv`


Code files include:
  * `immob_calc.Rmd` to calculate immobilization rates from C, N, and P concentration
  * `statistical_analyses.Rmd` contains all statistical analyses in the manuscript
  * `figures.Rmd` contains all code for generating figures in manuscript

Metadata:

__stripCNP.csv__

|Parameter     |Definition   |Units  |
| ------------- |-----------| -----|
|part.str|Unique stream partner code||
|Strip_id|Unique strip number||
|Type|Location of deployment||
|biome_short|Terrestrial biome||
|latitude||decimal degrees|
|longitude||decimal degrees|
|deploy_time|incubation time|days|
|mean_mean_daily_temp|mean site temperature|°C|
|P_ugg|Phosphorus concentration| µg/g dm|
|N_per|Nitrogen concentration|% dm|
|C_per|Carbon concentration|% dm|
|Mass|Punch mass|mg|
|Cmass|Mass of C in a punch|mg|
|CN|C:N ratio|mol C/mol N|
|CP|C:P ratio|mol C/mol P|
|NP|N:P ratio|mol N/mol P|
|Nim|N immobilization rate|µg N/g C/d|
|Pim|P immobilization rate|µg P/g C/d|
|Nfactor|N factor| |
|Ntmax|Time to maximum N mass|d|
|Pfactor|P factor| |
|Ptmax|Time to maximum P mass|d|
|NP_im|N immobilization:P immobilization|mol N/mol P|
|NP_fac|N factor:P factor|mol N/mol P|

__`water_quality.csv`__
