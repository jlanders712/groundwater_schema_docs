# Table: Aquifer Predictions Summary

## Overview

- Name: aquifer_predictions_summary
- Type: Related attribute table
- Description: DNRC machine learning model aquifer predictions, including DNRC source aquifer and DNRC aquifer code, aggregated as single predictions per GWIC ID.
- Primary key: GUID
- Parent/child role: Child layer.

## Columns

Columns:
| Field                                                            | Type                      | Nullable   | Alias                                                            | Description   |
|:-----------------------------------------------------------------|:--------------------------|:-----------|:-----------------------------------------------------------------|:--------------|
| OBJECTID                                                         | esriFieldTypeOID          | False      | OBJECTID                                                         |               |
| gwicid                                                           | esriFieldTypeInteger      | True       | gwicid                                                           |               |
| site_name                                                        | esriFieldTypeString       | True       | site_name                                                        |               |
| mbmg_aquifer                                                     | esriFieldTypeString       | True       | mbmg_aquifer                                                     |               |
| orig__dnrc_code                                                  | esriFieldTypeString       | True       | orig__dnrc_code                                                  |               |
| orig__dnrc_source_aquifer                                        | esriFieldTypeString       | True       | orig__dnrc_source_aquifer                                        |               |
| location_accuracy                                                | esriFieldTypeString       | True       | location_accuracy                                                |               |
| map_500k_dnrc_source_aquifer                                     | esriFieldTypeString       | True       | map_500k_dnrc_source_aquifer                                     |               |
| map_500k_dnrc_code                                               | esriFieldTypeString       | True       | map_500k_dnrc_code                                               |               |
| east_west_poly                                                   | esriFieldTypeString       | True       | east_west_poly                                                   |               |
| dem_30m                                                          | esriFieldTypeDouble       | True       | dem_30m                                                          |               |
| flow_accum_30m                                                   | esriFieldTypeDouble       | True       | flow_accum_30m                                                   |               |
| hand_30m                                                         | esriFieldTypeDouble       | True       | hand_30m                                                         |               |
| slope_deg_30m                                                    | esriFieldTypeDouble       | True       | slope_deg_30m                                                    |               |
| tpi_30m                                                          | esriFieldTypeDouble       | True       | tpi_30m                                                          |               |
| twi_30m                                                          | esriFieldTypeDouble       | True       | twi_30m                                                          |               |
| huc12                                                            | esriFieldTypeString       | True       | huc12                                                            |               |
| total_depth_ft_bgs                                               | esriFieldTypeDouble       | True       | total_depth_ft_bgs                                               |               |
| static_water_level_ft_bgs                                        | esriFieldTypeDouble       | True       | static_water_level_ft_bgs                                        |               |
| elevation_ft                                                     | esriFieldTypeDouble       | True       | elevation_ft                                                     |               |
| wse_ft                                                           | esriFieldTypeDouble       | True       | wse_ft                                                           |               |
| min_comp_from_ft                                                 | esriFieldTypeDouble       | True       | min_comp_from_ft                                                 |               |
| max_comp_to_ft                                                   | esriFieldTypeDouble       | True       | max_comp_to_ft                                                   |               |
| screen_intervals                                                 | esriFieldTypeString       | True       | screen_intervals                                                 |               |
| comp_type                                                        | esriFieldTypeString       | True       | comp_type                                                        |               |
| overall_pred__dnrc_source_aquifer                                | esriFieldTypeString       | True       | overall_pred__dnrc_source_aquifer                                |               |
| overall_proba__dnrc_source_aquifer                               | esriFieldTypeDouble       | True       | overall_proba__dnrc_source_aquifer                               |               |
| overall_pred__dnrc_code                                          | esriFieldTypeString       | True       | overall_pred__dnrc_code                                          |               |
| overall_proba__dnrc_code                                         | esriFieldTypeDouble       | True       | overall_proba__dnrc_code                                         |               |
| aquifer_error                                                    | esriFieldTypeSmallInteger | True       | aquifer_error                                                    |               |
| code_error                                                       | esriFieldTypeSmallInteger | True       | code_error                                                       |               |
| mean_proba_material__bedrock                                     | esriFieldTypeDouble       | True       | mean_proba_material__bedrock                                     |               |
| mean_proba_material__surficial                                   | esriFieldTypeDouble       | True       | mean_proba_material__surficial                                   |               |
| mean_proba_dnrc_source_aquifer__Basin_Fill_and_Alluvial_Sediment | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Basin_Fill_and_Alluvial_Sediment |               |
| mean_proba_dnrc_source_aquifer__Bearpaw_Pierre_Formations        | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Bearpaw_Pierre_Formations        |               |
| mean_proba_dnrc_source_aquifer__Claggett_Formation               | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Claggett_Formation               |               |
| mean_proba_dnrc_source_aquifer__Colorado_Group                   | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Colorado_Group                   |               |
| mean_proba_dnrc_source_aquifer__Eagle_Virgelle_Telegraph_Creek_F | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Eagle_Virgelle_Telegraph_Creek_F |               |
| mean_proba_dnrc_source_aquifer__Fort_Union_Formation             | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Fort_Union_Formation             |               |
| mean_proba_dnrc_source_aquifer__Fox_Hills_Hell_Creek_Lance_Forma | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Fox_Hills_Hell_Creek_Lance_Forma |               |
| mean_proba_dnrc_source_aquifer__Fractured_Rock                   | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Fractured_Rock                   |               |
| mean_proba_dnrc_source_aquifer__Judith_River_Formation           | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Judith_River_Formation           |               |
| mean_proba_dnrc_source_aquifer__Kootenai_Formation               | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Kootenai_Formation               |               |
| mean_proba_dnrc_source_aquifer__Livingston_Group                 | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Livingston_Group                 |               |
| mean_proba_dnrc_source_aquifer__Madison_Group                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Madison_Group                    |               |
| mean_proba_dnrc_source_aquifer__Morrison_Ellis_Upper_Paleozoic_F | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Morrison_Ellis_Upper_Paleozoic_F |               |
| mean_proba_dnrc_source_aquifer__Two_Medicine_Formation           | esriFieldTypeDouble       | True       | mean_proba_dnrc_source_aquifer__Two_Medicine_Formation           |               |
| mean_proba_dnrc_code__110ALVM                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__110ALVM                                    |               |
| mean_proba_dnrc_code__112DRFT                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__112DRFT                                    |               |
| mean_proba_dnrc_code__120PLNC                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__120PLNC                                    |               |
| mean_proba_dnrc_code__120SDMS                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__120SDMS                                    |               |
| mean_proba_dnrc_code__120VLCC                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__120VLCC                                    |               |
| mean_proba_dnrc_code__125FRUN                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__125FRUN                                    |               |
| mean_proba_dnrc_code__211BRPW                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211BRPW                                    |               |
| mean_proba_dnrc_code__211CLGT                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211CLGT                                    |               |
| mean_proba_dnrc_code__211CLRD                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211CLRD                                    |               |
| mean_proba_dnrc_code__211EGLE                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211EGLE                                    |               |
| mean_proba_dnrc_code__211FHHC                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211FHHC                                    |               |
| mean_proba_dnrc_code__211JDRV                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211JDRV                                    |               |
| mean_proba_dnrc_code__211LVGS                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211LVGS                                    |               |
| mean_proba_dnrc_code__211TMDC                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__211TMDC                                    |               |
| mean_proba_dnrc_code__217KOTN                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__217KOTN                                    |               |
| mean_proba_dnrc_code__221MRSN                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__221MRSN                                    |               |
| mean_proba_dnrc_code__310UDFD                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__310UDFD                                    |               |
| mean_proba_dnrc_code__330MDSN                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__330MDSN                                    |               |
| mean_proba_dnrc_code__340UDFD                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__340UDFD                                    |               |
| mean_proba_dnrc_code__400BELT                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__400BELT                                    |               |
| mean_proba_dnrc_code__500GNSC                                    | esriFieldTypeDouble       | True       | mean_proba_dnrc_code__500GNSC                                    |               |
| GUID                                                             | esriFieldTypeGUID         | True       | GUID                                                             |               |
| GlobalID                                                         | esriFieldTypeGlobalID     | False      | GlobalID                                                         |               |
| CreationDate                                                     | esriFieldTypeDate         | True       | CreationDate                                                     |               |
| Creator                                                          | esriFieldTypeString       | True       | Creator                                                          |               |
| EditDate                                                         | esriFieldTypeDate         | True       | EditDate                                                         |               |
| Editor                                                           | esriFieldTypeString       | True       | Editor                                                           |               |
