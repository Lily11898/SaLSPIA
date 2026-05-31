# Data Sources and Redistribution Notes

The MATLAB code is licensed separately under the MIT License. Review the terms
below before redistributing data files.

## Bundled LiDAR Data

The following files are derived from the Maungawhau / Mt Eden elevation model:

- `data/volcano_hires_surface_data`
- `data/maungawhau_hr.csv`

Source:

- Toitu Te Whenua Land Information New Zealand (LINZ),
  [Auckland LiDAR 1m DEM (2013)](https://data.linz.govt.nz/layer/53405-auckland-lidar-1m-dem-2013/)

License:

- [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)

Attribution:

> Contains data sourced from Toitu Te Whenua Land Information New Zealand and
> licensed for reuse under CC BY 4.0.

The files in this repository are reformatted and, for
`volcano_hires_surface_data`, subsampled for the manuscript experiments.

## External Curve Data

The following files are used by the manuscript experiments but should only be
bundled after redistribution permission has been confirmed:

| Local path | Used by | Upstream source |
| --- | --- | --- |
| `data/cur_data deer` | Reindeer contour, Example 4.3 | [giacomoorsi/ProgressiveIterationApproximation](https://github.com/giacomoorsi/ProgressiveIterationApproximation) |
| `data/s_loop_curve_data.txt` | G-loop curve, Example 4.7 | [XuejiaoYuan/LSPIA](https://github.com/XuejiaoYuan/LSPIA) |

At the time this release was prepared, the upstream repositories did not declare
an explicit data-redistribution license. Place authorized local copies at the
paths above to run the dependent experiments.

## Optional Supplementary Grid

`data/surface_data` is used only when the optional supplementary surface-ablation
case is enabled manually in `experiments/run_ablation_surface.m`. It is not needed
for the manuscript tables and is not bundled in the public release unless its
redistribution terms have been confirmed.

## Analytic Data

The blob, helix, Dini, and Peaks examples are generated directly by the MATLAB
drivers and do not require external data files.
