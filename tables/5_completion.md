# Table: Completion

## Overview

- Name: completion
- Type: Related attribute table
- Description: Well completion attributes.
- Primary key: GUID
- Parent/child role: Child table

## Columns

| Field                      | Type                      | Nullable   | Alias                      | Description                                                            |
|:---------------------------|:--------------------------|:-----------|:---------------------------|:-----------------------------------------------------------------------|
| OBJECTID                   | esriFieldTypeOID          | False      | OBJECTID                   |                                                                        |
| gwicid                     | esriFieldTypeInteger      | True       | gwicid                     | Unique identifier assigned by MBMG                                     |
| site_name                  | esriFieldTypeString       | True       | site_name                  | Most current known owner of the well/borehole                          |
| comp_from_ft               | esriFieldTypeDouble       | True       | comp_from_ft               | Top of completion interval in feet below ground surface                |
| comp_to_ft                 | esriFieldTypeDouble       | True       | comp_to_ft                 | Bottom of completion interval in feet below ground surface             |
| diameter_inches            | esriFieldTypeDouble       | True       | diameter_inches            | Casing diameter at completion interval in inches                       |
| number_of_openings         | esriFieldTypeString       | True       | number_of_openings         | Number of openings in completion interval                              |
| size_of_openings           | esriFieldTypeString       | True       | size_of_openings           | Size of opening in completion interval                                 |
| description                | esriFieldTypeString       | True       | description                | Description of screen interval or well completion                      |
| total_depth_ft_bgs         | esriFieldTypeDouble       | True       | total_depth_ft_bgs         | Reported depth of the well/borehole in feet below ground surface       |
| data_modification          | esriFieldTypeString       | True       | data_modification          | Description of data cleaning modifications                             |
| min_comp_from_ft           | esriFieldTypeDouble       | True       | min_comp_from_ft           | Overall top of screened interval for well                              |
| max_comp_to_ft             | esriFieldTypeDouble       | True       | max_comp_to_ft             | Overall bottom of screened interval for well                           |
| screen_intervals           | esriFieldTypeString       | True       | screen_intervals           | Top and bottom of screened interval in feet below ground surface       |
| comp_type                  | esriFieldTypeString       | True       | comp_type                  | Well completion type                                                   |
| comp_qaqc_flag_description | esriFieldTypeString       | True       | comp_qaqc_flag_description | Description of results of well completion table quality control checks |
| comp_qaqc_flag             | esriFieldTypeSmallInteger | True       | comp_qaqc_flag             | Well completion table quality control checks result                    |
| GUID                       | esriFieldTypeGUID         | True       | GUID                       | Related table destination key for relationships                        |
| GlobalID                   | esriFieldTypeGlobalID     | False      | GlobalID                   | Parent table origin primary key for relationships                      |
| CreationDate               | esriFieldTypeDate         | True       | CreationDate               | Record creation date                                                   |
| Creator                    | esriFieldTypeString       | True       | Creator                    | Record creator identification                                          |
| EditDate                   | esriFieldTypeDate         | True       | EditDate                   | Record edit date                                                       |
| Editor                     | esriFieldTypeString       | True       | Editor                     | Editor ID for last recorded edit                                       |
