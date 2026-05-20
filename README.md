# 2022-04 Access-Oriented Design

This package supports:

Lahoorpoor, B., Rayaprolu, H., Wu, H., & Levinson, D. M. (2022). Access-oriented design? Disentangling the effect of land use and transport network on accessibility. Transportation Research Interdisciplinary Perspectives, 13, 100536. https://doi.org/10.1016/j.trip.2021.100536

## Package Status

- Status: ready for public GitHub upload review.
- Generated: 2026-05-19 18:08:45 AEST.
- Paper copy: publisher-final Elsevier PDF, replacing the previous 24-page manuscript/preprint-like package copy.
- Source project: `/Users/dlev2617/Sydney Uni Dropbox/David Levinson/iMove - Liverpool Project`.

## Contents

- `paper/`: publisher-final PDF and paper reference notes.
- `data/access_frequency_matrix/`: Liverpool access comparison CSVs, by-precinct/access ZIPs, and analysis notebooks from the FrequencyMatrix workflow.
- `data/land_use_allocation/`: control totals, 2016/2056 transport-zone density tables, CoDesign/ForecastID projections, concordance archive, and land-use allocation notebooks.
- `data/scenario_land_use_and_access/`: compact mesh-block scenario access results and uniform/pyramid land-use allocation tables used to summarize Liverpool scenarios.
- `data/access_outputs/`: paper-cutoff baseline outputs and aggregated grid/TOD access outputs. Detailed per-cutoff gridded outputs are not copied because the aggregate outputs and source pointers capture the paper-level evidence with far less duplication.
- `data/spatial_inputs/`: selected spatial inputs for superblock, planned-network, developable-land, and Liverpool scenario geometry. Very large raw road, lot, and full mesh-block shapefiles are intentionally not copied.
- `code/notebooks/`: Jupyter notebooks and QGIS project files found with the Liverpool analysis.
- `docs/`: data dictionary, provenance notes, source pointer ledger, and checksums.

## Exclusions

The full Dropbox project contains multi-GB GIS and intermediate-output folders. Those are not copied into this package because they would add large, redundant, or raw-source material that is not needed for the paper-level archive. The excluded source locations and reasons are listed in `code/legacy/docs/SOURCE_POINTERS.csv`.

## Reproduction Boundary

This is an evidence and analysis-data package, not a one-command rebuild. It preserves the final paper, project notebooks, curated source/control tables, scenario land-use/access outputs, and compact spatial inputs sufficient to inspect the analysis lineage. Full regeneration may require the original QGIS/OTP/access-calculation environment and public source data described in the paper.

<!-- package-hardening-status:start -->
## Package Hardening Status

Generated: 2026-05-20 15:23:47 AEST

- Pipeline: `READY-TO-UPLOAD/PUBLIC`
- Sidecars added/updated: `PACKAGE_STATUS.md`, `PACKAGE_MANIFEST.csv`, `LICENSE_STATUS.md`.
- Paper reference copies are for local audit convenience and are not public-upload assets without rights review.
- Final GitHub upload should use the manifest include statuses and the license-status note.
<!-- package-hardening-status:end -->
