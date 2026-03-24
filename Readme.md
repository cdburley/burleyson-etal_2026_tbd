# Characterizing Diversity in Heat Wave and Cold Snap Responses for Assessing Grid Reliability

Casey D. Burleyson<sup>1\*</sup>, Nathalie Voisin<sup>1,2</sup>, Osten Anderson<sup>1</sup>, Heng Wan<sup>1</sup>, and Cameron Bracken<sup>1</sup> 

<sup>1 </sup> Pacific Northwest National Laboratory, Richland, WA, USA  
<sup>2 </sup> University of  Washington, Seattle, WA, USA  

\* corresponding author: casey.burleyson@pnnl.gov

## Abstract
Extreme weather events such as heat waves and cold snaps stress electric grids. Reliability assurance practices 
increasingly call for the utilization of historical events to “stress test” existing or projected infrastructure to 
demonstrate reliability or to evaluate the financial feasibility of proposed grid enhancements. There is, however, a 
lack of guidance on how to select those events. To inform those studies, we develop a benchmark of western United 
States (U.S.) grid responses to 38 years of coincident 2032-level weather-sensitive hourly load, wind, and solar time 
series along with weekly hydropower using the industry-vetted 2032 Anchor Data Set formulated by the U.S. Western 
Electricity Coordinating Council. We evaluate how events from regional libraries of heat waves and cold snaps across 15 
NERC subregions in the U.S. translated into diverse grid responses. Commonly used methods for ranking events by 
temperature or regional load during the event do not translate to high rankings for other stress metrics such as prices 
or the dependence on imported power. We further illustrate the challenge with three case studies demonstrating that 
events with similar regional temperatures and peak loads can produce fundamentally different operational outcomes 
depending on seasonal renewable resource availability, spatial extent, and event duration. This paper demonstrates how 
strategically selecting diverse events can enable more robust assessments of transmission needs, storage sizing and 
operations, and resource adequacy during heat waves and cold snaps. More work is needed to define stressful conditions 
for different planning applications and to inform emerging regulatory requirements.

## Journal reference
Burleyson, C.D., N. Voisin, O. Anderson, H. Wan, and C. Bracken (2026). Characterizing diversity in heat wave and cold
snap responses for assessing grid reliability. Submitted to *Applied Energy* - March 2026.

## Code reference
Burleyson, C.D., N. Voisin, O. Anderson, H. Wan, and C. Bracken (2026). Supporting code for Burleyson et al. 2026 - 
Applied Energy [Code]. Zenodo. DOI TBD.

## Data references
### Input data
| Dataset | Repository Link | DOI |
|:-------:|:---------------:|:---:|
|   TBD   |       TBD       | TBD |

### Output data
The post-processed files (resulting from the analysis scripts itemized below) are stored in the /data directory in this meta-repository.

| Dataset | Repository Link | DOI |
|:-------:|:---------------:|:---:|
|   TBD   |       TBD       | TBD |

## Reproduce my experiment
The following scripts pre-process the data in preparation for the analysis notebooks. They assume that you have the output
from the heat wave and cold snap identification workflow as well as the GridView simulations stored locally. Those files 
can be downloaded from the "Input Data" links listed above.

|                Script Name                 |                                                 Description                                                 |
|:------------------------------------------:|:-----------------------------------------------------------------------------------------------------------:|
|       process_temperature_data.ipynb       |              Cleans up the raw time series of daily temperature in each NERC TPL-008-1 region.              |
|   process_integrated_time_series.ipynb     |  Aggregates the temperature, load, and generation data into a single file for each NERC TPL-008-1 region.   |
|       process_hw_cs_libraries.ipynb        | Cleans up the raw thermal events library and adds information about loads and generation during each event. |
 
## Reproduce my figures
Use the following notebooks to run the analyses and reproduce the main and supplementary figures used in this publication.

| Figure Numbers |            Script Name            |                               Description                               | 
|:--------------:|:---------------------------------:|:-----------------------------------------------------------------------:|
|       1        |      plot_nerc_regions.ipynb      |                Plots the TPL-008-1 standard NERC regions                |
|    2,3,4,5     | plot_hw_cs_characteristics.ipynb  |              Plots heat wave and cold snap characteristics              |
|      6,9       |   plot_annual_generation.ipynb    | Plots the distributinon of demand and generation by type for each month |
|       7        |      plot_case_studies.ipynb      |  Plots key stress metrics and the generation mix for the case studies   |
|       8        | plot_event_temperature_maps.ipynb |      Plots maps of the event maximum temperature for a given event      |
|       SI       |   plot_event_time_series.ipynb    |        Plots time series of the grid response for a given event         |
|       SI       |   plot_hw_cs_correlations.ipynb   |  Plots correlation between variables for all heat waves or cold snaps   |