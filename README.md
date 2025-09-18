# Tropical drylands domiante global net carbon flux interannual variability irrespective of different biome definitions and geographic scales
This repository contains all of the code (Code folder) that was utilized in Bogucki et al. "Tropical drylands dominate global carbon flux interannual variability irrespective of different biome defintions and geographic scales". 

## Contact
Liam Bogucki. <br />
Email: lboguck@uwo.ca

## Conducting analysis
To replicate the analysis presented in Bogucki et al. "Tropical drylands dominate global carbon flux interannual variability irrespective of different biome defintions and geographic scales" the following files must be retireved and placed in the foler as follows: <br />
The TRENDY v11 flux files described in section 2.1. should be named the following where 'NAME' is replaced with the DGVM name: "fco2_NAME-S3_DEC2022-ext3_1970-2021_yearlymean_XYT.nc". The TRENDY results can be found here: https://mdosullivan.github.io/GCB/. <br />
The ESA land cover product described in section 2.2.1. should be named "ESACCI-LC-L4-LCCS-Map-300m-P1Y-aggregated-0.500000Deg-2019-v2.1.1.nc".<br />
The global area file for adjustment of the fluxes from KgC/m^2/yr to PgC/yr should be named "halfdeg_grid_area.dat" and is a global area-file at 0.5 degree solution that contains the area of each cell in m^2. <br />
The Koppen data file explained in section 2.2.1 should be named "KG_360x720.nc" and was retrieved from: "http://koeppen-geiger.vu-wien.ac.at/present.htm"<br />
The MODIS data file explained in section 2.2.2. should be named "MCD12C1.hdf".  <br />
The temperature data file explained in section 2.2.2. should be named "temp.nc". <br />
The AEZ data file explained in section 2.2.3. should be named "aez_v9v2_ENSEMBLE_rcp2p6_2020s.tif. <br />
The Aridity Index data file explained in seciton 2.2.3. should be named "halfdeg_AI.npy". <br />
The Ecoregion data files described in section 2.3. should all be placed in this folder as they are named upon download. <br />

<br />
Finally, all notebooks should be run in their entirity starting with file 000, 001, 002, 03, etc. and ending with file 015.<br />
 NOTE: The results of file 015 "015_Bootstrapping.ipynb" may be slighlty different than the results reported, as bootstrapping involves random number generation. However, the 50,000 iterations should limit the degree of variability observed.
