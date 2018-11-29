# SMART
This is the source code repository for the **Soil Moisture and Runoff simulation Toolkit** (**SMART**). SMART is a computationally efficient semi-distributed hydrologic modeling application for soil moisture, lateral flow and runoff simulation at a catchment scale.


## Description
The Soil Moisture and Runoff Toolkit (SMART) is a GIS-based hydrological modelling framework designed for semi-distributed hydrologic modelling in MATLAB. The framework is based upon the delineation of contiguous and topographically connected Hydrologic Response Units (HRUs). 

To reduce the number of computational elements, simulations are performed across a series of perpendicular cross sections to a stream or equivalent cross sections (ECS) in each first order sub-basin using a 2-dimensional, Richards’ equation based distributed hydrological model.

**Main features of SMART are:**
- Automation of sub-basin, HRU and cross section or equivalent cross section delineations of the entire catchment.
- Reducing computational time by reducing the number of computational elements through ECS delineation
- Any hydrologic model can be implemented in this framework

SMART pre- and post-processing scripts are written in **MATLAB** to automate the sub-basin, HRU and cross section delineations, model simulations across multiple cross sections, and to post-process model outputs. The MATLAB Parallel Processing Toolbox is used for simultaneous simulations of cross sections and is further reduced computational time.


## Credits
If you use SMART, please credit these three following papers:
- Ajami, H., Khan, U., Tuteja, N.K., Sharma, A.2016. Development of a computationally efficient semi-distributed
hydrologic modeling application for soil moisture, lateral flow and runoff simulation. *Environmental Modelling & Software*.
doi: 10.1016/j.envsoft.2016.09.002

- Khan, U., Tuteja, N.K., Ajami, H., Sharma, A.2014. An equivalent cross-sectional basis for semidistributed hydrological modeling. *Water Resources Research*, 50(5)4395-4415.

- Khan, U., Tuteja, N.K., Sharma, A.2013. Delineating hydrologic response units in large  upland catchments and its evaluation using soil moisture simulations. *Environmental Modelling & Software*, (46) 142-154.
 
In addition, a manual describes the implementation of SMART in detail:

- Ajami, H., Khan, U., Tuteja,  N.k., Sharma, A.2016. Semi-Distributed Hydrologic Modelling with Soil Moisture and Runoff Toolkit (SMART) User’s Manual. Version 1.0. 


If use the 2-dimensional Richards’ equation based distributed hydrological model of SMART (U3M-2D), please credit the following publications:
- Tuteja, N. K., Vaze, J., Murphy, B., Beale, G.T.B.2004. CLASS: Catchment scale multiple landuse atmosphere soil water and solute transport model, Tech. Rep. 04/12, Coop. Res. Cent. for Catchment Hydrol., Canberra. <http://www.toolkit.net.au/Tools/CLASSU3M-1D/publications>.

- Vaze, J., Tuteja, N.K., Teng, J.2004. CLASS Unsaturated Moisture Movement Model U3M-1D-User’s Manual, NSW Dep. of Infrastruct., Plann. and Nat. Resour., Sydney, Australia.

Recent publications on SMART: 

- Khan, U., H. Ajami, N.K. Tuteja, A. Sharma, S. Kim. 2018. Catchment Scale Simulations of Soil Moisture Dynamics Using an Equivalent Cross-Section based Hydrological Modelling Approach, Journal of Hydrology. https://doi.org/10.1016/j.jhydrol.2018.07.066

- Ajami, H., A. Sharma. 2018. Disaggregating Soil Moisture to Finer Spatial Resolutions - A Comparison of Alternatives, Water Resources Research, https://doi.org/10.1029/2018WR022575

## Software Requirements
- Microsoft Windows 7 operating system 
- MATLAB 2014b or later release
-	Terrain Analysis Using Digital Elevation Models (TauDEM) software developed by David G. Tarboton. The link to download the TauDEM package is (http://hydrology.usu.edu/taudem/). The command line version of TauDEM is used in SMART and users do not need ArcGIS license to use this software. 


## SMART Code Information
- SMART is written in MATLAB. The terrain processing steps are performed using the command line version of the TauDEM. 
- The unsaturated zone hydrologic model, U3M-2D, is written in C#. The compiled version of the model is provided with the toolkit. 


## License
SMART is distributed under the GNU Public License Version 3.
