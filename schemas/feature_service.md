# Feature Service Schema: Groundwater Wells

## Overview

This feature service represents groundwater wells as a spatial layer with nine related non-spatial tables.  
Each well feature is the parent record for multiple child records capturing aquifer ID, lithologic description, casing information, and other details linked by a unique well identifier.

## Components

- **Parent feature layer**
  - Name: `borehole`
  - Type: Feature layer (points)
  - Geometry: Point
  - Spatial reference: NAD83/Montana (WKID 32100)
  - Key fields:
    - `gwicid`   (integer, business key)
    - `GlobalID` (GUID, origin primary key for relationships)

- **Related tables**
  1. `aquifer`
  2. `aquifer_predictions`
  3. `aquifer_predictions_summary`
  4. `casing`
  5. `completion`
  6. `lithology`
  7. `performance`
  8. `sites`
  9. `well_use`

Each related table stores records associated with a single well via a foreign key field (`GUID`) that references `borehole.GlobalID`.

## Relationships

All relationships are one-to-many from the parent spatial layer to each related table.  
There are no relationships defined between the related tables themselves.

| Origin layer | Origin key  | Destination table           | Destination key   | Cardinality |
|--------------|-------------|-----------------------------|-------------------|-------------|
| Wells        | globalid    | aquifer                     | GUID              | 1:M         |
| Wells        | globalid    | aquifer_predictions         | GUID              | 1:M         |
| Wells        | globalid    | aquifer_predictions_summary | GUID              | 1:M         |
| Wells        | globalid    | casing                      | GUID              | 1:M         |
| Wells        | globalid    | completion                  | GUID              | 1:M         |
| Wells        | globalid    | lithology                   | GUID              | 1:M         |
| Wells        | globalid    | performance                 | GUID              | 1:M         |
| Wells        | globalid    | sites                       | GUID              | 1:M         |
| Wells        | globalid    | well_use                    | GUID              | 1:M         |
