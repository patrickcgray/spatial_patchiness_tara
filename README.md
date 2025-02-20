This repository contains the code for the manuscript "*Emergent patterns of patchiness differ between physical and planktonic properties in the ocean*" Nature Communications 16, 1808 (2025). https://doi.org/10.1038/s41467-025-56794-x

Authors: Patrick Clifton Gray<sup>\*,1,2</sup>, Emmanuel Boss<sup>1</sup>, Guillaume Bourdin<sup>1</sup>, Mission Microbiomes AtlantECO<sup>‡</sup>, Tara Pacific Consortium<sup>‡</sup>, Yoav Lehahn<sup>\*2</sup> 

1. School of Marine Sciences, University of Maine, Orono, ME, USA
2. Department of Marine Geosciences, Charney School of Marine Sciences, University of Haifa, Haifa, Israel

‡ Members of the Mission Microbiomes AtlantECO and the Tara Pacific Consortium are listed at the end of the paper.

*Corresponding authors: Patrick Gray (patrick.gray@maine.edu) and Yoav Lehahn (ylehahn@univ.haifa.ac.il)

While a rich history of patchiness research has explored spatial structure in the ocean, there is no consensus over the controls on biological patchiness and how physical-ecological-biogeochemical processes and patchiness relate. The prevailing thought is that physics structures biology, but this has not been tested at basin scale with consistent in situ measurements. Here we use the slope of the relationship between variance vs spatial scale to quantify patchiness and ~650,000 nearly continuous (dx ~ 200 m) measurements - representing the Atlantic, Pacific, and Southern Oceans - and find that patchiness of biological parameters and physical parameters are uncorrelated. We show variance slope is an emergent property with unique patterns in biogeochemical properties distinct from physical tracers, yet correlated with other biological tracers. These results provide context for decades of observations with different interpretations, suggest the use of spatial tests of biogeochemical model parameterizations, and open the way for studies into processes regulating the observed patterns.

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
