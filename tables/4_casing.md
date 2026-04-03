# Table: Casing

## Overview

- Name: casing
- Type: Related attribute table
- Description: Well casing attributes.
- Primary key: GUID
- Parent/child role: Child table

## Columns

| Field                 | Type                  | Nullable   | Alias                 | Description                                            |
|:----------------------|:----------------------|:-----------|:----------------------|:-------------------------------------------------------|
| OBJECTID              | esriFieldTypeOID      | False      | OBJECTID              |                                                        |
| gwicid                | esriFieldTypeInteger  | True       | gwicid                | Unique identifier assigned by MBMG                     |
| site_name             | esriFieldTypeString   | True       | site_name             | Most current known owner of the site                   |
| case_from_ft          | esriFieldTypeDouble   | True       | case_from_ft          | Top of casing interval in feet below ground surface    |
| case_to_ft            | esriFieldTypeDouble   | True       | case_to_ft            | Bottom of casing interval in feet below ground surface |
| stickup_ft            | esriFieldTypeDouble   | True       | stickup_ft            | Length in feet of casing above ground surface          |
| diameter_inches       | esriFieldTypeDouble   | True       | diameter_inches       | Casing diameter in inches                              |
| wall_thickness_inches | esriFieldTypeString   | True       | wall_thickness_inches | Casing wall thickness in inches                        |
| pressure_rating_psi   | esriFieldTypeString   | True       | pressure_rating_psi   | Casing pressure rating in pounds per square inch       |
| joint_type            | esriFieldTypeString   | True       | joint_type            | Casing joint type                                      |
| material              | esriFieldTypeString   | True       | material              | Casing material                                        |
| casing_shoe           | esriFieldTypeString   | True       | casing_shoe           | Casing shoe type                                       |
| GUID                  | esriFieldTypeGUID     | True       | GUID                  | Related table destination key for relationships        |
| GlobalID              | esriFieldTypeGlobalID | False      | GlobalID              | Parent table origin primary key for relationships      |
| CreationDate          | esriFieldTypeDate     | True       | CreationDate          | Record creation date                                   |
| Creator               | esriFieldTypeString   | True       | Creator               | Record creator identification                          |
| EditDate              | esriFieldTypeDate     | True       | EditDate              | Record edit date                                       |
| Editor                | esriFieldTypeString   | True       | Editor                | Editor ID for last recorded edit                       |
