# ciceroscm-calibrated-configuration-sets

Data repository for ciceroscm calibrated configuration sets and calibrated ensembles

The configuration file `config_file.json` is used to define and run the calibration, and the resulting ensemble is defined in the `calibrated_ciceroscm_ensemble.json`

The current version was calibrated for RCMIP phase III to run with ciceroscm v.2.1.3 https://doi.org/10.5281/zenodo.23401839.

Ensemble files in the `calibrated_ensembles` folder are ensembles calibrated for, used and described in the paper:
`Pattern effects shift climate sensitivity constraints in simple climate models` Sandstad et al 2026 in prep. The
filenames correspond to the various calibration setups as described there.

Default dataset was calibrated using the cscm-calibrate setup https://doi.org/10.5281/zenodo.20497648
Updated calibrations in the `calibrated_ensembles` folder were calibrated using an enhanced and updated version of that https://doi.org/10.5281/zenodo.23395267 


## Driver files

This repository also contains files used to drive the historical experiment to do the calibration

* `gases_vupdate_2024_WMO_added_new.txt` ciceroscm gas parameter file used for the calibration
* `historical_em_gases_vupdate_2024_WMO_added_new.txt` CMIP7 historical emissions from RCMIP phase III on ciceroscm format
* `historical_conc_gases_vupdate_2024_WMO_added_new.txt` CMIP7 historical concentrations from RCMIP phase III on ciceroscm format 
* `natemis_CH4_ode_method_from_March2026_vupdate_2024_WMO_added_new.txt` natural emissions of CH4 calculated to match historical concentrations
* `natemis_N2O_ode_method_from_March2026_vupdate_2024_WMO_added_new.txt`natural emissions N2O calculated to match historical concentrations
* `solar_RCMIP_historical_RCMIP3.txt` CMIP7 historical (and future projections of) annual solar forcing from RCMIP phase III on ciceroscm format
* `VOLC_RCMIP_historical_RCMIP3.txt` CMIP7 historical (and future projections of) annual volcanic forcing (on monthly format) from RCMIP phase III on ciceroscm format
* `LUCalbedo_RCMIP_historical_RCMIP3.txt` CMIP7 historical (and future projections of) annual volcanic forcing from RCMIP phase III on ciceroscm format (sum of land use albedo and irrigation)