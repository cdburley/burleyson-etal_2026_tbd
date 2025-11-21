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
TBD

|                Script Name                 |                                         Description                                         |
|:------------------------------------------:|:-------------------------------------------------------------------------------------------:|
| process_aggregate_gridview_load_data.ipynb | Aggregates output from the TELL model from the BA-level to the NERC TPL-008-1 region level. |
|       process_wind_solar_data.ipynb        |                 Formats the hourly wind and solar data into a single file.                  |
|       process_hw_cs_libraries.ipynb        |  Cleans up the raw thermal events library and adds information about loads and generation.  |


## Reproduce my figures
Use the following notebooks to reproduce the main and supplementary figures used in this publication.

| Figure Numbers |                Script Name                 |                Description                | 
|:--------------:|:------------------------------------------:|:-----------------------------------------:|
|       1        |        plot_nerc_regions.ipynb        | Plots the TPL-008-1 Standard NERC regions |
