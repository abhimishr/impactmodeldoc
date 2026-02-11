---
# IMPACT Changelog
---
## v4.1.4 - _Berlin_
### Description:
Maize price bugfix to maintain maize-wheat price ratio
### Updates
- Update to maize IPR (increase by 0.5 percentage points) to fix unrealistic global maize price increase.
---
## v4.1.3 - _Bursa_
### Description:
### Bugfix
- `QS00` for `jsbol` in `HND` given half the value of `jsbnt` without which the preloader works but the model doesnt solve
- This version fixes unrealistic calorie values (e.g. in `CRI` from groundnuts) 
### Updates
- `InputFiles\IMPACT3\IMPACT3_BaseProductionTrade.gdx` updated due to fix in Entropy code which resulted in negative priors.
- `InputFiles\IMPACT3\IMPACT3_IPRsAgrs.gdx` updated to have maize `YLDGR` fix from the IPROverwriting process. The change in `InputFiles\IMPACT3\IMPACT3_BaseProductionTrade.gdx` was causing weird dips in `EGY`.
---
## v4.1.2 - _Tunis_
### Description:
### Bugfix
- `PerCapGDP` reporting bugfix (not used in the model but fixed for consistency)
---
## v4.1.1 - _Guayaquil_
### Description:
### Updates
- `ReportGen` to account for aquatic foods reporting (commodities and activities)
### Bugfix
- Bugfix for GLOBE model interation (`hexpdev`)
- Spelling fix in `ReportGen` for one instance of `Sierra Leone` incorrectly written as `Sierra Leon`
---
## v4.1.0 - _Lima_
### Description:
2025 Intrinsic Productivity Growth Rate (IPR) update
### Updates
- **2025 IPR Updates**  [FH+NC]
---
## v4.0 - _Penang_
### Description:
IMPACT-FISH
### Updates
- Added **aquatic foods** to IMPACT main model
---
## v3.9 - _Valparaíso_
### Description:
Updated base year from 2020 to 2021
### Updates or Bug-Fixes
- Updated **`IMPACT3_CCData.gdx`** (Fix for spongy climate impact data due to legacy code).
- Update of base year data in IMPACT **(2020 to 2021)**
---
## v3.9.0-dev - _Georgetown_
### Description:
Updated base year from 2020 to 2021 [dev]
### Updates or Bug-Fixes
- Update of base year data in IMPACT **(2020 to 2021)**
### Notes
- Dev flag in this release until bugfix for CCDelta file is committed
---
## v3.8.2 - _Kyoto_
### Description: 
Hotfix v2 for growth rates in MENA
### Updates or Bug-Fixes
- Additional bugfix for 3.8.1 implementation for growth rates in MENA. 
---
## v3.8.1 - _Valencia_
### Description: 
Hotfix for MENA growth rates
### Updates or Bug-Fixes
- Bugfix for 3.8.0 implementation for growth rates in MENA. Some activities (dairy, potatoes, other, vegetables and tropical fruits) are excluded for additional shocks in MENA.
---
## v3.8.0 - _Kavrelis_
### Description: 
MENA-Fix
### Updates or Bug-Fixes
- Area and yield growth rates for Middle-East and North Africa
---
## v3.7.1 - _Sarnora_
### Description: 
hotfix_ 3.7.0
### Added
- `wcdc_new`: CAGR to calcualte `wcdc` numbers from 2005 data
### Updates or Bug-Fixes
- Hotfix for caluclating `wcdc` in 2020 based in 2005 data using CAGR
- Correct reporting of `wcd_s_fpu` numbers because `wcdc` calcualtion was corrected
---
## v3.7.0 - _Thornbridge_
### Description: 
Water Fix
### Added
- `outflow_coef_version`: Setting to decide if there is a one-to-one relationship for river basin outlows. Setting of `old` preseves one-to-one mapping and restores previous/old behavior in IMPACT. Setting of `new` allows one-to-many mapping. `new` is the current default.
- `outflow_coef` fraction of outflow to downstream FPUs
### Updates or Bug-Fixes
- Neighboring cells in `neigb` set
- Updated `INFLWEQ2` equation to account for `outflow_coef` parameter
- Updated `irw` parameter to account for `outflow_coef` parameter
---
## v3.6.2 - _Reykjavík_
### Description:
2025 EAT-Lancet
### Added
- Planetary health diets (EAT-Lancet 2.0)
### Updates or Bug-Fixes
- Fix for waste calculation (moved to overall demand calculation equation)
- Fix for Ozone and Animal productivity shocks (.\InputFiles\Scenarios\SimulationsSetUp.xlsm)
### Citation
`Mishra, A., Sulser, T.B., Gabriel, S., Cenacchi, N., Dunston, S., Headey, D., Herrero, M., Mason-D’Croz, D. and Wiebe, K., 2025. Affordability and nutritional challenges for the future of EAT diets: an economic modelling analysis. The Lancet Planetary Health, 9(10).`

DOI: `https://doi.org/10.1016/j.lanplh.2025.101325`

---
## v3.6.1 - _Saint Cloud_
### Citation
`Rosegrant, M.W., Wiebe, K., Sulser, T.B, Mishra, A., Cenacchi, N., Willenbockel, D., Dunston, S., Kimura, S and Yao, X. The Future of Food and Agriculture: Scenarios of Increased Public Investments and Policy Reforms for Asia and the Pacific. Asian Development Bank Briefs No. 364.` 

DOI: `https://dx.doi.org/10.22617/BRF250480-2`

---
## v3.4 - _Leyton_
### Description:
Global Food Securty paper
### Citation
`Rosegrant, M.W., Sulser, T.B., Dunston, S., Mishra, A., Cenacchi, N., Gebretsadik, Y., Robertson, R., Thomas, T. and Wiebe, K., 2024. Food and nutrition security under changing climate and socioeconomic conditions. Global Food Security, 41, p.100755.`

DOI: `https://doi.org/10.1016/j.gfs.2024.100755`

---