# Characterizing Diversity in Extreme Weather Events for Assessing Grid Reliability

Casey D. Burleyson<sup>1\*</sup>, Osten Anderson<sup>1</sup>, Cameron Bracken<sup>1</sup>, Heng Wan<sup>1</sup>, and Nathalie Voisin<sup>1,2</sup>

<sup>1 </sup> Pacific Northwest National Laboratory, Richland, WA, USA  
<sup>2 </sup> University of  Washington, Seattle, WA, USA  

\* corresponding author: casey.burleyson@pnnl.gov

## Abstract
Extreme weather events such as heat waves and cold snaps stress electric grids. Reliability assurance practices 
increasingly call for the utilization of historical events to “stress test” existing or projected infrastructure to 
demonstrate reliability or to evaluate the financial feasibility of proposed grid enhancements. To inform those studies 
we constructed regional libraries of heat waves and cold snaps across 15 NERC subregions in the United States (U.S.) 
and translated those events onto a projection of the grid in the western U.S. using the 2032 Anchor Dataset formulated 
by the U.S. Western Electricity Coordinating Council. We use illustrative examples to demonstrate that the electric 
grid in the western U.S. responds to heat waves and cold snaps in diverse ways. Commonly used methods for ranking 
events by temperature or regional load during the event do not translate to high rankings for other stress metrics such 
as the dependence on imported power. Three case studies demonstrate that events with similar regional temperatures and 
peak loads can produce fundamentally different operational outcomes depending on seasonal renewable resource 
availability, spatial extent, and event duration. This paper demonstrates how planners can make use of the broad 
spectrum of historical thermal events to evaluate grid reliability more holistically. Strategically selecting diverse 
events enables more robust assessments of transmission needs, storage operations, and resource adequacy to support 
reliability assurance studies and inform emerging regulatory requirements.

## Journal reference
Burleyson, C.D., O. Anderson, C. Bracken, H. Wan, and N. Voisin (2026). Characterizing diversity in extreme weather 
events for assessing grid reliability. Submitted to *Applied Energy* - March 2026.

## Code reference
TBD

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
|       1        |      plot_nerc_regions.ipynb      |                Plots the TPL-008-1 Standard NERC regions                |
|      TBD       | plot_hw_cs_characteristics.ipynb  |              Plots heat wave and cold snap characteristics              |
|      TBD       |   plot_annual_generation.ipynb    | Plots the distributinon of demand and generation by type for each month |
|      TBD       |      plot_case_studies.ipynb      |  Plots key stress metrics and the generation mix for the case studies   |
|      TBD       | plot_event_temperature_maps.ipynb |      Plots maps of the event maximum temperature for a given event      |
|      TBD       |   plot_event_time_series.ipynb    |        Plots time series of the grid response for a given event         |