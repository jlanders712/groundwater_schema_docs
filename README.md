# Water Sciences Bureau Groundwater Database

The Water Sciences Bureau’s Groundwater Section manages well and aquifer data derived from the Montana Bureau of Mines and Geology (MBMG) Groundwater Information Center (GWIC) database. The dataset includes value-added attributes such as quality control flags, elevation and topographic indices, and machine learning–based aquifer ID predictions. Data obtained from GWIC undergo a comprehensive cleaning and quality control process before publication. Data is updated frequently as new records are added to the GWIC database.

The database is available as a hosted feature service at: https://mtdnrc.maps.arcgis.com/home/item.html?id=c010e491a91940e99f23ad8c513e043a

Groundwater well data is obtained from the MBMG GWIC database feature service: https://mbmgmap.mtech.edu/server/rest/services/Water_Resources/GWIC_Database/FeatureServer

The ETL pipeline documentation is available at: https://github.com/jlanders712/gwic_ETL_pipeline

## Quality Control and Location Accuracy Flags
Well data QC checks include missing values, invalid datatypes, out-of-range values, and location verification. A description of any failed checks are appended to the QC flag description field, and summarized in the QC flag field according to the severity of the error. Refer to the ETL pipeline documentation for a description of each QC check.

### QC Flags
| Flag    | Description                                             | 
|:--------|:--------------------------------------------------------|
|    0    | Passed all QC checks                                    | 
|    1    | Missing values (e.g., total depth, static water level   | 
|    2    | Location error or other high severity error             | 

### Location Accuracy Flags
Location accuracy flags are derived from the geomethod attribute. All GPS-based geomethod values are classified as Excellent accuracy. All other geomethod values, which rely on Township–Range–Section descriptions, are classified according to how precisely the location is specified within the section (for example, full section, quarter section, or smaller quarter-section subdivisions).

| Flag    | Description                                                                                                 | 
|:----------------|:----------------------------------------------------------------------------------------------------|
|    Excellent    | Location derived with a GPS                                                                         | 
|    Good         | Location derived from TRS with at least quarter-quarter section precision, or map/photo geomethod   | 
|    Fair         | Location derived from TRS with quarter section precision                                            | 
|    Poor         | Location derived from TRS with section precision                                                    | 
