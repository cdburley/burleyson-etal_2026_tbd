# Exploiting Diversity in Extreme Weather Events for Assessing Grid Reliability

Casey D. Burleyson<sup>1\*</sup>, Osten Anderson<sup>1</sup>, Cameron Bracken<sup>1</sup>, Heng Wan<sup>1</sup>, and Nathalie Voisin<sup>1,2</sup>

<sup>1 </sup> Pacific Northwest National Laboratory, Richland, WA, USA  
<sup>2 </sup> University of  Washington, Seattle, WA, USA  

\* corresponding author: casey.burleyson@pnnl.gov

## Abstract
TBD

## Journal reference
TBD

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
Use the following notebooks to run the analysis and reproduce the main and supplementary figures used in this publication.

| Figure Numbers |           Script Name            |                               Description                               | 
|:--------------:|:--------------------------------:|:-----------------------------------------------------------------------:|
|       1        |     plot_nerc_regions.ipynb      |                Plots the TPL-008-1 Standard NERC regions                |
|      TBD       | plot_hw_cs_characteristics.ipynb |              Plots heat wave and cold snap characteristics              |
|      TBD       |   plot_annual_generation.ipynb   | Plots the distributinon of demand and generation by type for each month |
|      TBD       |     plot_case_studies.ipynb      |  Plots key stress metrics and the generation mix for the case studies   |