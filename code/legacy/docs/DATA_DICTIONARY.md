# Data Dictionary

This dictionary is reconstructed from file headers and the published paper. It is intentionally conservative where original codebooks were not found.

## Access Frequency Matrix Tables

Files: `Access_AllScenarios_Uniform.csv`, `Access_AllScenarios_Pyramid.csv`, `Access_LiverpoolLGA_Uniform.csv`

- `locality`: precinct, locality, or Liverpool LGA grouping.
- `Jobs`: reachable jobs or job-access measure at the stated cut-off.
- `cutoff`: travel-time threshold in minutes.
- `X`: scenario/frequency parameter used in the comparison notebooks.
- `T_freq`: transit frequency setting.
- `L_freq`: local feeder or lollipop/local-route frequency setting.

## Land-Use Allocation Tables

File: `TZ_Densities.csv`

- `tz16_code`, `tz16_name`: 2016 transport-zone identifier and name.
- `lga_code16`, `lga_name16`: 2016 local government area identifier and name.
- `GIC_AreaName`, `GIC_Precinct_190919`, `SGS_CoDBC_*`: precinct/development-area classification fields used in the allocation workflow.
- `ERP_2016`, `ERP_2056`: estimated resident population baseline and forecast.
- `EMP_2016`, `EMP_2056`: employment baseline and forecast.
- `Tz16_Area`: transport-zone area.
- `PopDensity_*`, `EmpDensity_*`, `*_Diff`: derived population/employment density fields and changes.

Files under `ForecastID_Projections/` and `CoDesign_Projections/` contain forecast area names, data type, year, counts, LGAs, and matched locality/precinct fields used to build 2056 control totals.

## Scenario Land-Use And Access Tables

Files: `AOD1.csv`, `AOD1-new.csv`, `AOD4.csv`, `Grid-centroid.csv`, `Grid-centroid-1.csv`

- `MB_ID`: mesh-block or derived mesh-block scenario identifier.
- `lon`, `lat`: centroid longitude and latitude.
- `T15_*`, `T30_*`: transit access at 15- and 30-minute cutoffs, with suffixes such as `U` and `P` indicating uniform or pyramid allocation.
- `Pop_U`, `Pop_P`: population assigned under uniform or pyramid scenario allocation.
- `NSW_LOCA_2`: locality name or locality grouping.
- `W15_value`, `W60_value`, `A30_value`: walk/auto access fields at indicated minute cutoffs in grid-centroid outputs.

Files under `data/scenario_land_use_and_access/land_use_allocation_uniform_pyramid/` contain mesh-block scenario allocations:

- `pop`, `job`: allocated population and jobs.
- `MB_CODE16`, `MB_ID`: source and derived mesh-block identifiers.
- `GRID_CODE`, `TOD1_CODE` to `TOD4_CODE`: scenario membership fields.
- `2056_pop`, `2056_job`: forecast population and jobs assigned to the scenario unit.

## Access Outputs

Files under `data/access_outputs/` use mode/cutoff column names such as:

- `JobsA30`, `JobsB15`, `JobsT30`, `JobsW15`: jobs reachable by auto, bike, transit, or walk at the stated cutoff.
- `MB_ID`: mesh-block identifier.
- `TOD*_ByPrecinct_*`: small aggregated summaries by precinct and mode.

## Spatial Inputs

Shapefile components under `data/spatial_inputs/` preserve selected geometries. File stems were normalized by replacing spaces and colons with underscores so the package can be checked out on common filesystems. Components with matching stems belong together.
