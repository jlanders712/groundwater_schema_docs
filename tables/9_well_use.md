# Table: Well use

## Overview

- Name: well_use
- Type: Related attribute table
- Description: All reported uses for the well.
- Primary key: GUID
- Parent/child role: Child table

## Columns

Columns:

| Field        | Type                      | Nullable   | Alias        | Description   |
|:-------------|:--------------------------|:-----------|:-------------|:--------------|
| OBJECTID     | esriFieldTypeOID          | False      | OBJECTID     |               |
| gwicid       | esriFieldTypeInteger      | True       | gwicid       |               |
| site_name    | esriFieldTypeString       | True       | site_name    |               |
| well_use     | esriFieldTypeString       | True       | well_use     |               |
| priority     | esriFieldTypeSmallInteger | True       | priority     |               |
| GUID         | esriFieldTypeGUID         | True       | GUID         |               |
| GlobalID     | esriFieldTypeGlobalID     | False      | GlobalID     |               |
| CreationDate | esriFieldTypeDate         | True       | CreationDate |               |
| Creator      | esriFieldTypeString       | True       | Creator      |               |
| EditDate     | esriFieldTypeDate         | True       | EditDate     |               |
| Editor       | esriFieldTypeString       | True       | Editor       |               |
