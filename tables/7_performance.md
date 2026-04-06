# Table: Performance

## Overview

- Name: performance
- Type: Related attribute table
- Description: Reported well yield attributes.
- Primary key: GUID
- Parent/child role: Child table

## Columns

Columns:

| Field                  | Type                      | Nullable   | Alias                  | Description   |
|:-----------------------|:--------------------------|:-----------|:-----------------------|:--------------|
| OBJECTID               | esriFieldTypeOID          | False      | OBJECTID               |               |
| gwicid                 | esriFieldTypeInteger      | True       | gwicid                 |               |
| site_name              | esriFieldTypeString       | True       | site_name              |               |
| testnumber             | esriFieldTypeSmallInteger | True       | testnumber             |               |
| testtype               | esriFieldTypeString       | True       | testtype               |               |
| testhours              | esriFieldTypeDouble       | True       | testhours              |               |
| yield_gpm              | esriFieldTypeDouble       | True       | yield_gpm              |               |
| pumping_waterlevel_ft  | esriFieldTypeDouble       | True       | pumping_waterlevel_ft  |               |
| drillstem_setting      | esriFieldTypeDouble       | True       | drillstem_setting      |               |
| recovery_waterlevel_ft | esriFieldTypeDouble       | True       | recovery_waterlevel_ft |               |
| recoveryhours          | esriFieldTypeDouble       | True       | recoveryhours          |               |
| drawdown               | esriFieldTypeDouble       | True       | drawdown               |               |
| pump_test_depth        | esriFieldTypeDouble       | True       | pump_test_depth        |               |
| test_flow_measured     | esriFieldTypeString       | True       | test_flow_measured     |               |
| flow_control           | esriFieldTypeString       | True       | flow_control           |               |
| GUID                   | esriFieldTypeGUID         | True       | GUID                   |               |
| GlobalID               | esriFieldTypeGlobalID     | False      | GlobalID               |               |
| CreationDate           | esriFieldTypeDate         | True       | CreationDate           |               |
| Creator                | esriFieldTypeString       | True       | Creator                |               |
| EditDate               | esriFieldTypeDate         | True       | EditDate               |               |
| Editor                 | esriFieldTypeString       | True       | Editor                 |               |
