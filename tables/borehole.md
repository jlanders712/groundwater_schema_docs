# Table: Borehole

## Overview

- Name: borehole
- Type: Feature layer (points)
- Description: Spatial representation of groundwater wells and their core attributes.
- Primary key: GlobalID
- Parent/child role: Parent layer for all related tables.

## Columns

| Field                        | Type                      | Nullable   | Alias                         | Description                                                                                                               |
|:-----------------------------|:--------------------------|:-----------|:------------------------------|:--------------------------------------------------------------------------------------------------------------------------|
| OBJECTID                     | esriFieldTypeOID          | False      | OBJECTID                      |                                                                                                                           |
| gwicid                       | esriFieldTypeInteger      | True       | GWIC ID                       | Unique identifier assigned by MBMG                                                                                        |
| site_name                    | esriFieldTypeString       | True       | Site Name                     | Most current known owner of the site                                                                                      |
| geomethod                    | esriFieldTypeString       | True       | Geomethod                     | Method used to determine the latitude and longitude                                                                       |
| total_depth_ft_bgs           | esriFieldTypeDouble       | True       | Total Depth (ft)              | Reported depth of the well/borehole in feet below ground surface                                                          |
| static_water_level_ft_bgs    | esriFieldTypeDouble       | True       | Static Water Level (ft)       | Reported distance in feet below ground surface the water is found when the well is not pumping                            |
| depth_water_enters_ft_bgs    | esriFieldTypeDouble       | True       | Depth Water Enters (ft)       | Reported depth to top of shallowest completion zone                                                                       |
| stickup_ft                   | esriFieldTypeDouble       | True       | Stickup (ft)                  | Length in feet of casing above ground surface                                                                             |
| shut_in_pressure_psi         | esriFieldTypeDouble       | True       | Shut-in pressure (psi)        | Pressure in pounds per square inch for flowing artesian wells                                                             |
| water_temp_deg_C             | esriFieldTypeDouble       | True       | Water temp (deg C)            | Measured temperatue of the water in degrees celsius                                                                       |
| date_completed               | esriFieldTypeString       | True       | Date Completed                | Date the well/borehole was completed                                                                                      |
| how_drilled                  | esriFieldTypeString       | True       | Drilling method               | Drilling method used to complete the well/borehole                                                                        |
| drilling_company             | esriFieldTypeString       | True       | Drilling company              | Company name who drilled the well/borehole                                                                                |
| abandoned_flag               | esriFieldTypeString       | True       | Abandoned flag                | Flag noting whether the well has been abandoned                                                                           |
| date_abandoned               | esriFieldTypeString       | True       | Date abandoned                | Date the well was abandoned                                                                                               |
| status                       | esriFieldTypeString       | True       | status                        | Status of the well showing whether the record is a new well or modification of an existing well                           |
| flowing                      | esriFieldTypeString       | True       | flowing                       | Flag noting whether the well is flowing from artesian pressure                                                            |
| construction_type            | esriFieldTypeString       | True       | construction_type             |                                                                                                                           |
| notes_borehole               | esriFieldTypeString       | True       | notes_borehole                | Well construction notes                                                                                                   |
| map_500k_dnrc_source_aquifer | esriFieldTypeString       | True       | map_500k_dnrc_source_aquifer  | Map unit for DNRC source aquifer                                                                                          |
| map_500k_dnrc_code           | esriFieldTypeString       | True       | map_500k_dnrc_code            | Map unit for DNRC aquifer code                                                                                            |
| east_west_poly               | esriFieldTypeString       | True       | east_west_poly                | Map unit for DNRC east/west regions used to convert aquifer codes to source aquifers                                      |
| huc12                        | esriFieldTypeDouble       | True       | huc12                         | 12-digit hydrologic unit code from the USGS Watershed Boundary Dataset                                                    |
| dem_30m                      | esriFieldTypeDouble       | True       | dem_30m                       | Ground surface elevation derived from a 30-meter digital elevation model (DEM)                                            |
| flow_accum_30m               | esriFieldTypeDouble       | True       | flow_accum_30m                | Flow accumulation value derived from a 30-meter digital elevation model (DEM)                                             |
| hand_30m                     | esriFieldTypeDouble       | True       | hand_30m                      | Height above nearest drainage (HAND) value derived from a 30-meter digital elevation model (DEM)                          |
| slope_deg_30m                | esriFieldTypeDouble       | True       | slope_deg_30m                 | Land surface slope in degrees derived from a 30-meter digital elevation model (DEM)                                       |
| tpi_30m                      | esriFieldTypeDouble       | True       | tpi_30m                       | Topographic position index (TPI) derived from a 30-meter digital elevation model (DEM)                                    |
| twi_30m                      | esriFieldTypeDouble       | True       | twi_30m                       | Topographic wetness index (TWI) derived from a 30-meter digital elevation model (DEM)                                     |
| all_uses                     | esriFieldTypeString       | True       | All uses                      | Reported purpose/s for water from the well as listed on the well log                                                      |
| yield_gpm                    | esriFieldTypeDouble       | True       | Yield (gpm)                   | Reported well yield in gallons per minute                                                                                 |
| qaqc_flag                    | esriFieldTypeSmallInteger | True       | qaqc_flag                     | Quality control checks result, 0 - passed, 1 - missing values, 2 - location error or other high severity error            |
| qaqc_flag_description        | esriFieldTypeString       | True       | qaqc_flag_description         | Description of results of quality control checks                                                                          |
| location_error               | esriFieldTypeSmallInteger | True       | location_error                | Flag indicating whether location error was identified                                                                     |
| depth_water_enters_fillna    | esriFieldTypeSmallInteger | True       | depth_water_enters_fillna     | Flag indicating if null depth water enters value was filled with total depth, applicable to open-bottom construction type |
| location_accuracy            | esriFieldTypeString       | True       | location_accuracy             | Location accuracy flag based on geomethod                                                                                 |
| location_mismatch            | esriFieldTypeDouble       | True       | location_mismatch             | Flag denoting whether TRS-derived coordinates differ from actual TRS coordinates                                          |
| distance_to_locationid_ft    | esriFieldTypeDouble       | True       | distance_to_locationid_ft     | Distance of well location to correct TRS coordinates, applicable for TRS geomethod                                        |
| min_comp_from_ft             | esriFieldTypeDouble       | True       | min_comp_from_ft              | Top of first screened interval in feet below ground surface                                                               |
| max_comp_to_ft               | esriFieldTypeDouble       | True       | max_comp_to_ft                | Bottom of last screened interval in feet below ground surface                                                             |
| screen_intervals             | esriFieldTypeString       | True       | screen_intervals              | Min/max depth below ground surface for all screened intervals                                                             |
| comp_type                    | esriFieldTypeString       | True       | comp_type                     | Well completion type                                                                                                      |
| comp_qaqc_flag               | esriFieldTypeSmallInteger | True       | comp_qaqc_flag                | Flag indicating whether completion table passed quality control checks                                                    |
| comp_qaqc_flag_description   | esriFieldTypeString       | True       | comp_qaqc_flag_description    | Description of results from completion table quality control checks                                                       |
| lith_qaqc_flag               | esriFieldTypeSmallInteger | True       | lith_qaqc_flag                | Flag indicating whether lithology table passed quality control checks                                                     |
| lith_qaqc_flag_description   | esriFieldTypeString       | True       | lith_qaqc_flag_description    | Description of results from lithology table quality control checks                                                        |
| lithology_records            | esriFieldTypeSmallInteger | True       | lithology_records             | Flag indicating whether lithology records are available                                                                   |
| elevation_ft                 | esriFieldTypeDouble       | True       | Ground surface elevation (ft) | Ground surface elevation in feet derived from 30-meter digital elevation model (DEM)                                      |
| wse_ft                       | esriFieldTypeDouble       | True       | Water surface elevation (ft)  | Water surface elevation in feet derived from 30-meter digital elevation model (DEM) and reported static water level (swl) |
| dnrc_source_aquifer_final    | esriFieldTypeString       | True       | DNRC Source Aquifer           | Primary DNRC source aquifer name                                                                                          |
| dnrc_code_final              | esriFieldTypeString       | True       | DNRC Aquifer Code             | Primary DNRC aquifer code ID                                                                                              |
| aquifer_id_source            | esriFieldTypeString       | True       | Source Aquifer ID Origin      |                                                                                                                           |
| GlobalID                     | esriFieldTypeGlobalID     | False      | GlobalID                      | Parent table origin primary key for relationships                                                                         |
| CreationDate                 | esriFieldTypeDate         | True       | CreationDate                  | Record creation date                                                                                                      |
| Creator                      | esriFieldTypeString       | True       | Creator                       | Record creator identification                                                                                             |
| EditDate                     | esriFieldTypeDate         | True       | EditDate                      | Record edit date                                                                                                          |
| Editor                       | esriFieldTypeString       | True       | Editor                        | Editor ID for last recorded edit                                                                                          |
| date_completed_dt            | esriFieldTypeDate         | True       | Date Completed - new          | Well completion date, conversion of date_completed string field to datetime                                               |
| driller_name                 | esriFieldTypeString       | True       | driller_name                  | Driller name of who completed the well/borehole                                                                           |
| aquifer_material             | esriFieldTypeString       | True       | Aquifer material              | Bedrock or surficial aquifer material based on the primary DNRC source aquifer name                                       |
