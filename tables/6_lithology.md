# Table: Lithology

## Overview

- Name: lithology
- Type: Related attribute table
- Description: Lithologic descriptions.
- Primary key: GUID
- Parent/child role: Child layer.

## Columns
| Field                        | Type                      | Nullable   | Alias                        | Description   |
|:-----------------------------|:--------------------------|:-----------|:-----------------------------|:--------------|
| OBJECTID                     | esriFieldTypeOID          | False      | OBJECTID                     |               |
| gwicid                       | esriFieldTypeInteger      | True       | gwicid                       |               |
| site_name                    | esriFieldTypeString       | True       | site_name                    |               |
| lith_from_ft                 | esriFieldTypeDouble       | True       | Lithology from (ft)          |               |
| lith_to_ft                   | esriFieldTypeDouble       | True       | Lithology to (ft)            |               |
| lith_qaqc_flag_description   | esriFieldTypeString       | True       | lith_qaqc_flag_description   |               |
| lith_qaqc_flag               | esriFieldTypeSmallInteger | True       | lith_qaqc_flag               |               |
| original_text                | esriFieldTypeString       | True       | original_text                |               |
| text                         | esriFieldTypeString       | True       | Description                  |               |
| horizon_id                   | esriFieldTypeSmallInteger | True       | horizon_id                   |               |
| max_horizon_id               | esriFieldTypeSmallInteger | True       | max_horizon_id               |               |
| mbmg_aquifer                 | esriFieldTypeString       | True       | mbmg_aquifer                 |               |
| dnrc_code                    | esriFieldTypeString       | True       | dnrc_code                    |               |
| dnrc_source_aquifer          | esriFieldTypeString       | True       | dnrc_source_aquifer          |               |
| comp_qaqc_flag               | esriFieldTypeSmallInteger | True       | comp_qaqc_flag               |               |
| comp_qaqc_flag_description   | esriFieldTypeString       | True       | comp_qaqc_flag_description   |               |
| location_accuracy            | esriFieldTypeString       | True       | location_accuracy            |               |
| qaqc_flag                    | esriFieldTypeSmallInteger | True       | qaqc_flag                    |               |
| map_500k_dnrc_source_aquifer | esriFieldTypeString       | True       | map_500k_dnrc_source_aquifer |               |
| map_500k_dnrc_code           | esriFieldTypeString       | True       | map_500k_dnrc_code           |               |
| east_west_poly               | esriFieldTypeString       | True       | east_west_poly               |               |
| dem_30m                      | esriFieldTypeDouble       | True       | dem_30m                      |               |
| flow_accum_30m               | esriFieldTypeDouble       | True       | flow_accum_30m               |               |
| hand_30m                     | esriFieldTypeDouble       | True       | hand_30m                     |               |
| slope_deg_30m                | esriFieldTypeDouble       | True       | slope_deg_30m                |               |
| tpi_30m                      | esriFieldTypeDouble       | True       | tpi_30m                      |               |
| twi_30m                      | esriFieldTypeDouble       | True       | twi_30m                      |               |
| huc12                        | esriFieldTypeDouble       | True       | huc12                        |               |
| total_depth_ft_bgs           | esriFieldTypeDouble       | True       | total_depth_ft_bgs           |               |
| static_water_level_ft_bgs    | esriFieldTypeDouble       | True       | static_water_level_ft_bgs    |               |
| elevation_ft                 | esriFieldTypeDouble       | True       | elevation_ft                 |               |
| wse_ft                       | esriFieldTypeDouble       | True       | wse_ft                       |               |
| min_comp_from_ft             | esriFieldTypeDouble       | True       | min_comp_from_ft             |               |
| max_comp_to_ft               | esriFieldTypeDouble       | True       | max_comp_to_ft               |               |
| screen_intervals             | esriFieldTypeString       | True       | screen_intervals             |               |
| comp_type                    | esriFieldTypeString       | True       | comp_type                    |               |
| dwe_lithology                | esriFieldTypeSmallInteger | True       | dwe_lithology                |               |
| pred__material               | esriFieldTypeString       | True       | pred__material               |               |
| pred__dnrc_source_aquifer    | esriFieldTypeString       | True       | pred__dnrc_source_aquifer    |               |
| pred__dnrc_code              | esriFieldTypeString       | True       | pred__dnrc_code              |               |
| GUID                         | esriFieldTypeGUID         | True       | GUID                         |               |
| GlobalID                     | esriFieldTypeGlobalID     | False      | GlobalID                     |               |
| CreationDate                 | esriFieldTypeDate         | True       | CreationDate                 |               |
| Creator                      | esriFieldTypeString       | True       | Creator                      |               |
| EditDate                     | esriFieldTypeDate         | True       | EditDate                     |               |
| Editor                       | esriFieldTypeString       | True       | Editor                       |               |
