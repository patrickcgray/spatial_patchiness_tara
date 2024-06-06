This repository contains the code for the manuscript "*Emergent patterns of patchiness reflect decoupling between ocean physics and biology*" currently under review at Nature Communications.

Authors: Patrick Clifton Gray<sup>\*,1,2</sup>, Emmanuel Boss<sup>1</sup>, Guillaume Bourdin<sup>1</sup>, Mission Microbiomes AtlantECO<sup>‡</sup>, Tara Pacific Consortium<sup>‡</sup>, Yoav Lehahn<sup>\*2</sup> 

1. School of Marine Sciences, University of Maine, Orono, ME, USA
2. Department of Marine Geosciences, Charney School of Marine Sciences, University of Haifa, Haifa, Israel

‡ Members of the Mission Microbiomes AtlantECO and the Tara Pacific Consortium are listed in the Acknowledgments.

*Corresponding authors: Patrick Gray (patrick.gray@maine.edu) and Yoav Lehahn (ylehahn@univ.haifa.ac.il)

Abstract: While a rich history of patchiness research has explored spatial structure in the ocean, there is still much uncertainty over the controls on biological patchiness and how biogeochemical processes and patchiness relate. The prevailing thought is that physics structures biology in the ocean, but this has not been tested at the basin scale with consistent in situ measurements. We show that the patchiness of physics and biology are decoupled at the global scale. We use a global dataset of in situ surface optical properties from the R/V Tara program and use the slope of spatial scale vs variance to quantify patchiness. Using ~650,000 nearly continuous (dx~150m) measurements from a ship-board underway sampling system - representing five years of consistently collected data across the Atlantic, Pacific, and Southern Oceans - we find that the patchiness of physical and biological parameters are entirely uncorrelated. While their variance at a given scale is typically strongly correlated, the cascade across scales is not. We show that variance slope, our metric for patchiness, can be an emergent property with unique patterns in biological and particle properties that are distinct from physical tracers yet connected to other biological tracers. This is true even with concentration-independent properties such as average particle size. We discuss the ecosystem dynamics that could lead to these spatial patterns and suggest this as a test of parameterizations in biogeochemical models and atmospheric correction of satellite data. This work emphasizes the importance of marine ecosystem spatial patterns, which currently are rarely considered, yet could be a valuable source of insight into marine ecosystems. Spatial metrics such as the one we use are sensitive to different BGC dimensions than current monitoring approaches focusing on concentration of pigments such as chlorophyll a. 

## Code access
The notebooks included here:
1.  go from the raw data to the initial processed dataset for analysis `data_prep.ipynb`
2.  or you can begin directly with the collated data and re-create the analysis `patchiness.ipynb`.

This runs on Docker and a matching environment can be obtained by running `docker pull pangeo/pangeo-notebook:2024.04.05`

# Data Access
Data is available in the Release as an asset at this link: https://github.com/patrickcgray/spatial_patchiness_tara/releases/tag/v1.0. 
From there you can easily download the data:
1.  as the initial merged file which includes all Tara Pacific and Tara Microbiome inline optical data `merged_tara_pacific_microbiome_acs_160124.feather`
2.  or as the file where variance slope has been calculated `gdf_intermittency_full_flagged.feather`
