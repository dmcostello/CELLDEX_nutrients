# CELLDEX_nutrients
Data and code for the manuscript:
Costello et al. *Global patterns and controls of nutrient immobilization on decomposing cellulose in riverine ecosystems*.


Data files include:
  * `stripCNP.csv`
  * `waterquality.csv`
  * `decomp_k.csv`
  * `immob_eco.csv`


Code files include:
  * `immob_calc.Rmd` to calculate immobilization rates from C, N, and P concentration
  * `statistical_analyses.Rmd` contains all statistical analyses in the manuscript
  * `figures.Rmd` contains all code for generating figures in manuscript

Metadata:

__`stripCNP.csv`__

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
|Nfactor|N factor|µg/punch |
|Ntmax|Time to maximum N mass|d|
|Pfactor|P factor|µg/punch |
|Ptmax|Time to maximum P mass|d|
|NP_im|N immobilization:P immobilization|mol N/mol P|
|NP_fac|N factor:P factor|mol N/mol P|

__`water_quality.csv`__
|Parameter     |Definition   |Units  |
| ------------- |-----------| -----|
|part.str|Unique stream partner code||
|NH4_ugL|Ammonium concentration|µg N/L|
|NO3_ugL|Nitrate concentration|ug N/L|
|PO4_ugL|Phosphate concentration|ug P/L|
|cond|Conductivity at 25°C|µS/cm|
|pH|pH |Standard units|
|DOC|Dissolved organic carbon|mg C/L|
|DIN|Dissolved inorganic nitrogen|µg N/L|
|DNP|DIN:SRP ratio|mol N/mol P|
|DHP|NH4:SRP ratio|mol N/mol P|

__`decomp_k.csv`__
|Parameter     |Definition   |Units  |
| ------------- |-----------| -----|
|part.str|Unique stream partner code||
|Type|Location of deployment||
|k|Decomposition rate|1/d|

__`immob_eco.csv`__
|Parameter     |Definition   |Units  |
| ------------- |-----------| -----|
|Study|Study from which rates are calculated||
|Biome|Terrestrial biome||
|Habitat|River or riparian||
|N_instant|Maximum instantaneous N flux|mg N/m^2/d|
|N_annual|Annual N flux|g N/m^2/d|
|P_instant|Maximum instantaneous P flux|mg P/m^2/d|
|P_annual|Annual P flux|g P/m^2/d|


_Variable codes and notes_  
part.str: alphabetic codes are the partner and numerical codes are the stream. Codes are defined in a database internal to the CELLDEX project.

Type: STR = stream or river incubated; RIP = riparian incubated  

Nim-NP_fac: Immobilization rates, factors, times, and ratios were calculated from strip concentrations using the code in `immob_calc.Rmd`

immob_eco: Calculations for flux estimates are found in `statistical_analyses.Rmd`

"NA" for immobilization = sample collected, but N or P mass did not increase
