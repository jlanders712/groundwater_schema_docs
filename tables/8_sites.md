# Table: Sites

## Overview

- Name: sites
- Type: Related attribute table
- Description: Site metadata.
- Primary key: GUID
- Parent/child role: Child table

## Columns

Columns:

| Field                      | Type                  | Nullable   | Alias                      | Description   |
|:---------------------------|:----------------------|:-----------|:---------------------------|:--------------|
| OBJECTID                   | esriFieldTypeOID      | False      | OBJECTID                   |               |
| gwicid                     | esriFieldTypeInteger  | True       | gwicid                     |               |
| site_name                  | esriFieldTypeString   | True       | site_name                  |               |
| latitude                   | esriFieldTypeDouble   | True       | latitude                   |               |
| longitude                  | esriFieldTypeDouble   | True       | longitude                  |               |
| geomethod                  | esriFieldTypeString   | True       | geomethod                  |               |
| datum_latlon               | esriFieldTypeString   | True       | datum_latlon               |               |
| date_latlon                | esriFieldTypeString   | True       | date_latlon                |               |
| llmapscale                 | esriFieldTypeString   | True       | llmapscale                 |               |
| latacc                     | esriFieldTypeDouble   | True       | latacc                     |               |
| lonacc                     | esriFieldTypeDouble   | True       | lonacc                     |               |
| altitude_ft_amsl           | esriFieldTypeDouble   | True       | altitude_ft_amsl           |               |
| method_altitude            | esriFieldTypeString   | True       | method_altitude            |               |
| datum_altitude             | esriFieldTypeString   | True       | datum_altitude             |               |
| date_altitude              | esriFieldTypeString   | True       | date_altitude              |               |
| township                   | esriFieldTypeString   | True       | township                   |               |
| range                      | esriFieldTypeString   | True       | range                      |               |
| section                    | esriFieldTypeDouble   | True       | section                    |               |
| qsection                   | esriFieldTypeString   | True       | qsection                   |               |
| sequence_no                | esriFieldTypeDouble   | True       | sequence_no                |               |
| county                     | esriFieldTypeString   | True       | county                     |               |
| state                      | esriFieldTypeString   | True       | state                      |               |
| drainage_basin             | esriFieldTypeString   | True       | drainage_basin             |               |
| drainage_basin_description | esriFieldTypeString   | True       | drainage_basin_description |               |
| huc                        | esriFieldTypeString   | True       | huc                        |               |
| addition_subdivision       | esriFieldTypeString   | True       | addition_subdivision       |               |
| block                      | esriFieldTypeString   | True       | block                      |               |
| lot                        | esriFieldTypeString   | True       | lot                        |               |
| certofsurvey               | esriFieldTypeString   | True       | certofsurvey               |               |
| parcel                     | esriFieldTypeString   | True       | parcel                     |               |
| assessortract              | esriFieldTypeString   | True       | assessortract              |               |
| geocode                    | esriFieldTypeString   | True       | geocode                    |               |
| site_type                  | esriFieldTypeString   | True       | site_type                  |               |
| irr_section                | esriFieldTypeString   | True       | irr_section                |               |
| usgs_quad                  | esriFieldTypeString   | True       | usgs_quad                  |               |
| notes                      | esriFieldTypeString   | True       | notes                      |               |
| site_identifier            | esriFieldTypeString   | True       | site_identifier            |               |
| GUID                       | esriFieldTypeGUID     | True       | GUID                       |               |
| GlobalID                   | esriFieldTypeGlobalID | False      | GlobalID                   |               |
| CreationDate               | esriFieldTypeDate     | True       | CreationDate               |               |
| Creator                    | esriFieldTypeString   | True       | Creator                    |               |
| EditDate                   | esriFieldTypeDate     | True       | EditDate                   |               |
| Editor                     | esriFieldTypeString   | True       | Editor                     |               |
