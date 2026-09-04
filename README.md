## Data description

Environmental and biogeochemical data for the **Clarion–Clipperton Zone (CCZ)** 
and the surrounding region were extracted from simulations of the **EC Earth System Model**.

The extraction region, hereafter referred to as **CCZ+10**, extends from:

- **Longitude:** 170°W to 100°W
- **Latitude:** 10°S to 30°N

Data were retained on the native curvilinear EC-Earth ocean grid, without 
spatial interpolation.

### Historical data

Historical environmental conditions were obtained from the **EC-Earth3-ESM-1** model under the `esm-hist` experiment and ensemble member `r1i1p1f1`. Model output was extracted from the BSC EC-Earth archive for the period **1985–2014**.

Monthly variables were retained at their original temporal resolution, resulting in **360 monthly time steps** over the 30-year historical period. Global model fields were first restricted to the **CCZ+10** domain while preserving the native model grid.

The historical dataset comprises the following environmental and biogeochemical variables:

- `chldiatos`: chlorophyll associated with diatoms
- `chlmiscos`: chlorophyll associated with other or miscellaneous phytoplankton
- `co3satcalc`: calcite carbonate saturation-related product
- `dfe`: dissolved iron
- `dissic`: dissolved inorganic carbon
- `epcalc100`: calcite export at 100 m
- `expc`: particulate organic carbon export
- `no3`: nitrate
- `o2`: dissolved oxygen
- `ph`: seawater pH
- `phyc`: phytoplankton carbon
- `po4`: phosphate
- `si`: silicate
- `so`: seawater salinity
- `talk`: total alkalinity
- `thetao`: seawater potential temperature

For variables represented throughout the water column, processed historical products contain **bottom-layer conditions**. Variables intrinsically defined at a particular depth or without a vertical dimension were retained according to their native model definition.

For example, `epcalc100` represents export at **100 m** and was therefore not subjected to bottom-layer extraction.
