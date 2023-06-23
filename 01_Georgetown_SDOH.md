# Summary of the Georgetown-SDOH Database

## What is it ?
As part of the AIM AHEAD Data bridge initiative, the Georgetown-ICBI Team has downloaded, formatted and stored many of these datasets in the Google’s cloud based datawarehouse system BigQuery.

## Data sources used to populate the Georgetown-SDOH Database with a short description

====> Some of the short descriptions need to be better summarized


| Name of BigQuery table                                         | Short description                                                        | Source                                                                                                   | Link                                                                                                              |
|----------------------------------------------------------------|--------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Low Food Access                                                | Area info from nearest grocery, merged with poverty data                 | Open   Data DC                                                                                           | https://opendata.dc.gov/                                                                                          |
| Child Opportunity index                                        | Measures resources for children                                          | diversitydatakids.org                                                                                    | diversitydatakids.org                                                                                             |
| Neighborhood   Deprivation Index                               | Factor analysis data from measures in socioeconomic status               | National   Cancer Institute                                                                              | https://www.cancer.gov/                                                                                           |
| Area Deprivation Index                                         | Factors for income, education, housing quality, employment               | University   of Wisconsin                                                                                | https://www.neighborhoodatlas.medicine.wisc.edu/                                                                  |
| Eviction Rates                                                 | Eviction information by area                                             | Eviction   Lab                                                                                           | https://evictionlab.org/                                                                                          |
| Income Inequality                                              | Poverty and median household income estimate                             | Census                                                                                                   |         https://www.census.gov/topics/income-poverty/income-inequality.html                                       |
| Cencus demographics (Social explorer)                          | Census data measuring demographics, economic and business information    | https://www.socialexplorer.com/                                                                          | https://www.socialexplorer.com/                                                                                   |
| Area Health Resource                                           | Health care resource information                                         | Area   Health Resource                                                                                   | https://data.hrsa.gov/topics/health-workforce/ahrf                                                                |
| Social Capital Index                                           | Resource data on social capital                                          | US   Census Bureau, MIT Election Lab, National center for Charitable  Statistics                         |         https://aese.psu.edu/nercrd/community/social-capital-resources                                            |
| Social Vulnerability Index dataset                             | Percentile ranking for socioeconomics and housing                        | US   Centers for Disease Control and Prevention/ Agency for Toxic Substances and   Disease      Registry |         https://www.atsdr.cdc.gov/placeandhealth/svi/data_documentation_download.html                             |
| County level cancer incidence and mortality data               | Death and incidence rate of all cancer sites around the county           | SEER   and CDC State Cancer Profiles                                                                     | https://statecancerprofiles.cancer.gov/                                                                           |
| County-level BRFSS Health data (Labeled as County Health data) | Health measures by county                                                | County   Health Rankings and      Roadmaps                                                               | https://www.countyhealthrankings.org/sites/default/files/medi      a/document/2022%20Analytic%20Documentation.pdf |
| Social Deprivation Index (SDI)                                 | Measures levels of disadvantage across small areas                       | Robert   Graham Center                                                                                   |         https://www.graham-center.org/maps-data-tools/social-deprivation-index.html                               |
| AHRQ SDOH Data                                                 | Social, economic, education, infrastructure, healthcare measures         | Agency   for Healthcare Research and Quality (AHRQ)                                                      |         Social   Determinants of Health Database \| Agency for Healthcare Research and Quality   (ahrq.gov)       |
| Minority Health SVI                                            | Factors measuring socioeconomic status, housing, health, minority status | CDC   and U.S. Department of Health and Human Services (HHS) Office of Minority   Health                 |         https://www.minorityhealth.hhs.gov/minority-health-svi/                                                   |
| ASCII US Cancer Site Statistics (USCS)                         | Cancer Types & Childhood cancer data                                     | CDC                                                                                                      |         https://www.cdc.gov/cancer/uscs/dataviz/download_data.htm                                                 |


## Methodology
Detailed metadata about each data source was first noted such as, information about the number of records, date of last upate, type of access and data formats. 
A summary of the attributes (i.e. variables) and its data type was also made. Depending on the information desired, multiple datasources were merged based on a common attribute such as the "Geographic Entity ID" or GEOID

Detialed summaries of how each data source are provided in this mult-tab excel sheet: ====> ADD FILE HERE 

## How to access the Georgetown-SDOH database
The information summarized in the Georgetown-SDOH database is accessible through multiple ways
(a) Access using python scripts that can directly query the Georgetown-SDOH Bigquery database (easiest and most popular, hence highly recommended)
(b) Directly querying the Georgetown-SDOH Bigquery database using SQL-like commands (read-only access offered on a case-by-case basis to a limited audience with experience in programming)
(c) Access using R script (future)
(d) Access using BigQuery APIs (future)

Detailed tutorials are provided for each option

## Tutorials
* Tutorial 1: How to extract information from the Georgetown-SDOH Bigquery database using python scripts
* Tutorial 2: 


