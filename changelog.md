# IMPACT Changelog

## v4.1.4-dev

### Name: Maize price fix 

### Updates

- Update to maize IPR (increase by 0.5 percentage points) to fix unrealistic global maize price increase

## v4.1.3

### Bugfix

- `QS00` for `jsbol` in `HND` given half the value of `jsbnt` without which the preloader works but the model doesnt solve
- This version fixes unrealistic calorie values (e.g. in `CRI` from groundnuts) 

### Updates

- `InputFiles\IMPACT3\IMPACT3_BaseProductionTrade.gdx` updated due to fix in Entropy code which resulted in negative priors.
- `InputFiles\IMPACT3\IMPACT3_IPRsAgrs.gdx` updated to have maize `YLDGR` fix from the IPROverwriting process. The change in `InputFiles\IMPACT3\IMPACT3_BaseProductionTrade.gdx` was causing weird dips in `EGY`.

## v4.1.2

### Name: IMPACT 4.1.2

### Bugfix

- `PerCapGDP` reporting bugfix (not used in the model but fixed for consistency)

## v4.1.1

### Name: IMPACT 4.1.1 

### Updates

- `ReportGen` to account for FISH reporting (commodities and activities)

### Bugfix

- Bugfix for GLOBE model interation (`hexpdev`)
- Spelling fix in `ReportGen` for one instance of `Sierra Leone` incorrectly written as `Sierra Leon`

## v4.1.0

### Name: IMPACT (2025 IPR Update) 

### Updates

- 2025 IPR Updates  [FH+NC]

## v4.0

### Name: IMPACT (w FISH) 

### Updates

- Added fish to IMPACT main model

## v3.9

### Name: IMPACT (Base year 2021) 

### Updates or Bug-Fixes

- Updated `IMPACT3_CCData.gdx` (Fix for spongy climate impact data due to legacy code).
- Update of base year data in IMPACT (2021 -> 2021)

## v3.9.0-dev

### Name: IMPACT Base 2021 

### Updates or Bug-Fixes

- Update of base year data in IMPACT (2021 -> 2021)

### Notes

- Dev flag in this release until bugfix for CCDelta file is committed

## v3.8.2

### Name: _Hotfix v2_ for growth rates in MENA

### Updates or Bug-Fixes

- Additional bugfix for 3.8.1 implementation for growth rates in MENA. 

## v3.8.1

### Name: _Hotfix_ for MENA growth rates

### Updates or Bug-Fixes

- Bugfix for 3.8.0 implementation for growth rates in MENA. Some activities (dairy, potatoes, other, vegetables and tropical fruits) are excluded for additional shocks in MENA.

## v3.8.0

### Name: MENA-Fix

### Updates or Bug-Fixes

- Area and yield growth rates for Middle-East and North Africa

## v3.7.1

### Name: _hotfix_ 3.7.0

### Added

- `wcdc_new`: CAGR to calcualte `wcdc` numbers from 2005 data

### Updates or Bug-Fixes

- Hotfix for caluclating `wcdc` in 2020 based in 2005 data using CAGR
- Correct reporting of `wcd_s_fpu` numbers because `wcdc` calcualtion was corrected

## v3.7.0

### Name: _Water Fix_

### Added

- `outflow_coef_version`: Setting to decide if there is a one-to-one relationship for river basin outlows. Setting of `old` preseves one-to-one mapping and restores previous/old behavior in IMPACT. Setting of `new` allows one-to-many mapping. `new` is the current default.
- `outflow_coef` fraction of outflow to downstream FPUs

### Updates or Bug-Fixes

- Neighboring cells in `neigb` set
- Updated `INFLWEQ2` equation to account for `outflow_coef` parameter
- Updated `irw` parameter to account for `outflow_coef` parameter

## v3.6.2

### Name: _EAT-Lancet 2.0_

### Added

- Planetary health diets (EAT-Lancet 2.0)


### Updates or Bug-Fixes

- Fix for waste calculation (moved to overall demand calculation equation)
- Fix for Ozone and Animal productivity shocks (.\InputFiles\Scenarios\SimulationsSetUp.xlsm)

## v3.6.1

### Name: _ADB_

### Citation (Tentative)

Rosegrant MW; Sulser T, Mishra A, Cenacchi N,Willenbockel D, Dunston S, and Wiebe K. The Future of Food and Agriculture: Scenarios of Increased Public Investments and Policy Reforms for Asia and the Pacific. _Asian Development Bank_. (Forthcoming)

## v3.4

### Name: _GFS_

### Citation

Rosegrant, M.W., Sulser, T.B., Dunston, S., Mishra, A., Cenacchi, N., Gebretsadik, Y., Robertson, R., Thomas, T. and Wiebe, K., 2024. Food and nutrition security under changing climate and socioeconomic conditions. _Global Food Security_, 41, p.100755.
