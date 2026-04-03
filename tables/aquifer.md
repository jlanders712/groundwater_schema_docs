# Table: Aquifer

## Overview

- Name: aquifer
- Type: Related attribute table
- Description: Aquifer identification for the source of water to the well, includes MBMG aquifer codes and DNRC model predictions.
- Primary key: GUID
- Parent/child role: Child table

## Columns

| Field                      | Type                  | Nullable   | Alias                      | Description                                                                                                                                                                          |
|:---------------------------|:----------------------|:-----------|:---------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| OBJECTID                   | esriFieldTypeOID      | False      | OBJECTID                   |                                                                                                                                                                                      |
| gwicid                     | esriFieldTypeInteger  | True       | gwicid                     | Unique identifier assigned by MBMG                                                                                                                                                   |
| site_name                  | esriFieldTypeString   | True       | site_name                  | Most current known owner of the well/borehole                                                                                                                                        |
| mbmg_aquifer               | esriFieldTypeString   | True       | mbmg_aquifer               | GWIC aquifer code for geologic source of water assigned by MBMG                                                                                                                      |
| description                | esriFieldTypeString   | True       | description                | GWIC aquifer code geologic description                                                                                                                                               |
| east_west_poly             | esriFieldTypeString   | True       | east_west_poly             | Map unit for DNRC east/west regions used to convert aquifer codes to source aquifers                                                                                                 |
| dnrc_code                  | esriFieldTypeString   | True       | dnrc_code                  | DNRC aquifer code ID                                                                                                                                                                 |
| dnrc_source_aquifer        | esriFieldTypeString   | True       | dnrc_source_aquifer        | DNRC source aquifer name                                                                                                                                                             |
| GUID                       | esriFieldTypeGUID     | True       | GUID                       | Related table destination key for relationships                                                                                                                                      |
| GlobalID                   | esriFieldTypeGlobalID | False      | GlobalID                   | Parent table origin primary key for relationships                                                                                                                                    |
| CreationDate               | esriFieldTypeDate     | True       | CreationDate               | Record creation date                                                                                                                                                                 |
| Creator                    | esriFieldTypeString   | True       | Creator                    | Record creator identification                                                                                                                                                        |
| EditDate                   | esriFieldTypeDate     | True       | EditDate                   | Record edit date                                                                                                                                                                     |
| Editor                     | esriFieldTypeString   | True       | Editor                     | Editor ID for last recorded edit                                                                                                                                                     |
| mbmg_priority              | esriFieldTypeDouble   | True       | mbmg_priority              | GWIC priority field                                                                                                                                                                  |
| proba__dnrc_source_aquifer | esriFieldTypeDouble   | True       | proba__dnrc_source_aquifer | Aquifer ID model source aquifer prediction probability                                                                                                                               |
| proba__dnrc_code           | esriFieldTypeDouble   | True       | proba__dnrc_code           | Aquifer ID model DNRC aquifer code prediction probability                                                                                                                            |
| aquifer_id_source          | esriFieldTypeString   | True       | aquifer_id_source          | Origin of the aquifer ID assignment                                                                                                                                                  |
| dnrc_priority              | esriFieldTypeDouble   | True       | dnrc_priority              | DNRC aquifer code priority to determine final aquifer ID based on heirarchy of 1: MBMG assigned, 2: model predicted. Minimum value is merged with borehole table as final aquifer ID |
| aquifer_material           | esriFieldTypeString   | True       | aquifer_material           | Bedrock or surficial aquifer material based on the primary DNRC source aquifer name                                                                                                  |
