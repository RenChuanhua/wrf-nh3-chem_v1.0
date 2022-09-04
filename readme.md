The WRF-NH3-Chem model a dynamic NH3 emission model capable of calculating NH3 emission rate interactively with time- and spatial-varying meteorological and soil conditions. It is embedded into the regional WRF-Chem model (version 3.9.1).



Following the steps below, the user can install the model and start using it


1. replace the original file in WRF/chem directory with ***emissions_driver.F*** and ***chem_driver.F*** in the ***code-modified*** directory. The modified code is annotated with "WRF-NH3-CHEM modifed by renchuanhua"


2. replace the original file in WRF/Registry directory with ***registry.chem*** and ***Registry.EM_COMMON*** in our ***registry-variable*** dir.


3. put subdirectories ***./input-binary/nh3_agrisoil/fertilizer/freeinten/graze/industry/residential/transport*** into ***geog_data_path***


4. replace the ***GEOGRID.TBL*** file in ***WPS***

5.  finally, turn on the dynamic NH3 emission model in WRF-Chem by specifying nh3emis_opt = 1 in ***chem*** section of ***namelist.input*** file 
