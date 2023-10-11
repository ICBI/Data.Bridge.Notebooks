# Summary of the Georgetown-SDOH Datawarehouse

## What is it ?
The Social Determinants of Health (SDoH) highlights environmental and non-medical factors, such as economic and social conditions, that influence the health status of an individual or a group. With SDoH, we aim to measure health disparities across the nation and determine which factors affect health outcomes and risks. Social Determinants of Health data can be found mostly in Census Bureau databases and other public databases. 

As part of the AIM AHEAD Data bridge initiative, the Georgetown-ICBI Team has downloaded, formatted and stored many of these datasets in the Google’s cloud database system BigQuery database format called the Georgetown-SDOH database 

<img src="https://github.com/ICBI/Data.Bridge.Notebooks/blob/main/AAlogo1.jpg" width="300" height="250">

## Data sources used to populate the Georgetown-SDOH Datawarehouse 


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


## Data sources with a short description
Inside the Georgetown-SDOH datawarehouse, we have a large variety of public statistical datasets related to health. The types of SDoH datasets in BigQuery are presented below.

**“Low Food Access” dataset:** Low Food Access data comes from Open Data DC and is a part of the DC Government database. It details the low food access areas in DC that are estimated to be more than a 10-minute walk from the nearest full-service grocery store. The dataset has been merged with the Census poverty data to estimate the population of food insecurity in the area. In order to be considered as food insecure, the person must be below 185% of the federal poverty line in addition to living in a low food access area. This dataset contains area information along with poverty data from the nearest grocery store in the District of Columbia.   
_BigQuery Database names:_ Low Food Access Areas 2018 (Area Type: Block Group)

**Child Opportunity Index (COI)** data comes from diversitydatakids.org, which is housed at the Heller School for Social Policy and Management at Brandeis University. The COI 2.0 is a composite index based on 29 indicators spanning the three domains of education, health and environment, and social and economic. This data captures neighborhood resources and measures and maps quality of resource and conditions that matter for children at the census tract level. The Child Opportunity Index includes demographic, education, access to resources, and public health data information.
_BigQuery Database names: _COI Child population data (Area Type: Census Tract), COI Index table (Area Type: Census Tract), COI component indicators Raw indicator values (Area Type: Census Tract), COI component indicators Z-scores (Area Type: Census Tract)

**Neighborhood Deprivation Index (NDI)** data derives from the National Cancer Institute. The NDI is created using factor analysis to identify variables from 13 measures in socioeconomic status, which includes wealth and income, education, occupation, and housing conditions. The 13 variables of measure were obtained from the Census Bureau’s five-year American Community Survey (ACS) data for 2013-2017.  The Neighborhood Deprivation Index data contains factor analysis data from measures in socioeconomic status along with the 13 measures obtained from ACS data.
_BigQuery Database names: _NDI 2013-2017 (Area Type: Census Tract)

**Area Deprivation Index (ADI)** data comes from the University of Wisconsin, which has an overlap with IOSVI and NDI data.  The Area Deprivation Index is based on a measure created by the Health Resources and Services Administration (HRSA) over thirty years ago, and allows for neighborhood rankings by socioeconomic disadvantage at a state or national level. The ADI includes factors for theoretical domains of income, education, employment, and housing quality. It can be used to inform health delivery and policy, especially for the most disadvantaged neighborhood groups.
_BigQuery Database names:_ ADI 2019 (Area Type: Block Group), ADI 2020 (Area Type: Block Group)

**Eviction Rates** data comes from the Eviction Lab at Princeton University. This dataset includes residential eviction filing information by weeks or months, along with the location area of eviction and date.
_BigQuery Database names:_ Eviction Cities Monthly Data (Area Type: County and Census Tract), Eviction Cities Weekly Data (Area Type: County and Census Tract), Eviction State Monthly Data (Area Type: Census Tract), Eviction State Weekly Data (Area Type: Census Tract)

**Census Bureau Income Inequality (SAIPE)** data from the Census Bureau includes information on poverty and median household income estimates by county and state. This data estimates income and poverty for all US states and counties as well as school-age children in poverty for all districts. The Income Inequality data contains number and percentage of children in poverty, population in poverty by state and county, and median household income of those in poverty.
_BigQuery Database names: _Small Area Income and Poverty Estimates SAIPE 2020 (Area Type: County)

**Social Explorer and Census Demographics database** consists of Census Bureau and American Community Survey data measuring demographics, economic and business information, crime, health, and environmental studies. The Census Redistricting Data, Census Population Ethnicity data, and FBI Crime Data 2019 are included inside Social Explorer, which contains information on ethnicity, school, and crime population.
_BigQuery Database names: _ ACS5Year2020Estimates (Area Type: County), Census 2020 Ethnicity Population Data (Area Type: County), Census 2020 Redistricting Data (Area Type: County), Education Attainment Reformatted (Area Type: County), Educational Attainment by County (Area Type: County), FBI Crime Data 2019 (Area Type: County), School Data 2018 (Area Type: Places)

**Area Health Resource (AHR)** data derives from Health Resources & Services Administration, which provides health care to people that are geographically isolated, economically or medically vulnerable. The Area Health Resources Files contain data on health care professions, health facilities, population characteristics, economics, health professions training, hospital utilization and expenditures, and environment at the county, state, and national levels. This specific health care resource information database contains clinical data by year, profession, population, and location along with subsets of data by various health profession and population demographic subcategories. 
_BigQuery Database_ names: Area Health Resource 2019 (Area Type: County), Area Health Resource 2020 (Area Type: County), Area Health Resource 2021 (Area Type: County), Area Health Resource State and National Level 2019 (Area Type: State), Area Health Resource State and National Level 2020 (Area Type: State), Area Health Resource State and National Level 2021 (Area Type: State)

**Social Capital Index (SOCAP)** data comes from the Penn State Department of Agricultural Economics, Sociology, and Education, which obtain their data sources from the US Census Bureau, MIT Election Lab, and National Center for Charitable Statistics. SOCAP is created using principal component analysis of establishments per 10,000 population, voter turnout, Census response rate, and non-profit organizations per 10,000 population. It consists of datasets, maps, and other resources related to social capital. The Social Capital Index data also details the number of establishments for different fitness and sports centers as well as political, business, religious, civic, labor, and professional organizations. 
_BigQuery Database names: _Social Capital SOCAP 2014 (Area Type: County), Social Capital SOCAP 2019 (Area Type: County)

**Social Vulnerability Index (SVI)** data consists of data from the US Centers for Disease Control and Prevention (CDC) and Agency for Toxic Substances and Disease Registry (ATSDR) to help public health officials and emergency response planners identify and map the communities that most need support on hazardous events. SVI indicates the relative vulnerability of every US Census tract and ranks them on 16 social factors, including unemployment, racial and ethnic minority status, and disability, then further groups them into four themes. The data contains information on percentile ranking for housing types and transportation, minority status, household composition and characteristics, and socioeconomic status.
_BigQuery Database names:_ SVI 2018 (Area Type: Census Tract), SVI 2020 County Level (Area Type: County), SVI 2020 County Tract Level (Area Type: Census Tract)

**Minority Health Social Vulnerability Index (Minority Health SVI)** data are developed by the CDC and US Department of Health and Human Services (HHS) Office of Minority Health. The Minority Health SVI is used to enhance existing resources to identify racial and ethnic minority communities that were greatly impacted due to COVID-19. This dataset is an extension of Social Vulnerability Index (SVI). Minority Health SVI indicates the relative vulnerability of every US county, and combines 15 social factors that are included in SVI with additional factors known to be associated with COVIS-19 outcomes. The factors include socioeconomic status, household composition and disability, minority status and language, housing type and transportation, health care infrastructure and access, and medical vulnerability. The last two factors are specific to Minority Health SVI. 
_BigQuery Database names_ : Minority SVI 2018 (Area Type: County)

**SEER/CDC County Level Cancer Incidence and Mortality (SEER Cancer Incidence and Mortality)** data comes from the SEER and CDC State Cancer Profiles and shows geographic profile information on cancer burden in the US. This data reveals geographic disparities across different population subgroups for cancer incidence and mortality, cancer risk factors, and cancer screening. The SEER Cancer Incidence and Mortality data details information on death rate and incidence rate of all stages of cancer sites around the country.
_BigQuery Database names_: County level cancer incidence data 2014-2018 (Area Type: County), County level cancer mortality data 2014-2018 (Area Type: County)

**BRFSS County Level Health (County Health) data** from the County Health Rankings and Roadmaps includes information on health measures on a county level. County Health data includes dataset of physical health, mental health, obesity, physical inactivity, area-level access and social demographic variables across the county. It provides the measure value, numerator, denominator, and confidence intervals for all County Health Rankings, ranked and unranked measures, for each county in the nation. 
_BigQuery Database names_ : 2018 County Health Additional Measures Data (Area Type: County), 2018 County Health Outcomes and Factors Ranking (Area Type: County), 2018 County Health Outcomes and Factors Subrankings (Area Type: County), 2018 County Health Ranked Measure Data, 2018 County Health Rankings Data (Area Type: County), 2021 County Health Rankings (Area Type: County), 2022 County Health Rankings (Area Type: County), 2022 County Health Trends Data (Area Type: County)

**Social Deprivation Index (SDI)** data from the Robert Graham Center contains quantified information on levels of disadvantage across small areas. SDI measures area level deprivation based on seven demographic characteristics collected in the American Community Survey, and includes information on ethnicity, vehicle availability, housing, employment and family information, needs, education, and poverty level.
_BigQuery Database_ names: SDI 2015 County Level (Area Type: County), SDI 2015 Tract Level (Area Type: Census Tract)	  

**AHRQ SDOH data** comes from the Agency for Healthcare Research and Quality (AHRQ). The variables in the SDOH database correspond to key domains identified by AHRQ: social context, economic context, education, physical infrastructure, and healthcare context along with descriptive statistics for continuous and categorical variables. They are linked at three levels of geography data.
_BigQuery Database_ names: AHRQ SDOH County Level 2020 (Area Type: County), AHRQ SDOH Zip Code Data 2020 (Area Type: Zip Code, different from other GEOID codes), AHRQ SDOH Tract Level Data 2020 (Area Type: Census Tract)

**ASCII US Cancer Site Statistics (ASCII USCS) data** from the CDC contains US Cancer Statistics data on different cancer types and childhood cancer information. The cancer type data is grouped by demographics, such as race and ethnicity, state and region, and age. ASCII USCS also consists of brain cancer by tumor type and childhood cancer information detailed by ICCC group, age, and primary cancer site groups.
_BigQuery Database names_: USCS BySite 1999-2019, USCS ChildByAge Adjusted 1999-2019, USCS ChildByAge Cr 1999-2019, USCS ChildBySite 1999-2019, USCS ICCCByAge Adjusted 1999-2019, USCS ICCCByAge Cr 1999-2019, USCS ICCCBySite 1999-2019, USCS BrainBySite 1999-2019, USCS ByAge 1999-2019, USCS ByArea 1999-2019 (Area Type: State), USCS ByArea County 1999-2019 (Area Type: County)

## Methodology
Detailed metadata about each data source was first noted such as, information about the number of records, date of last upate, type of access and data formats. 
A summary of the attributes (i.e. variables) and its data type was also made. Depending on the information desired, multiple datasources were merged based on a common attribute such as the "Geographic Entity ID" or GEOID

Detialed summaries of how each data source are provided in this mult-tab excel sheet [HERE](https://github.com/ICBI/Data.Bridge.Notebooks/blob/main/Goal1_SDOH/ICBI%20Social%20Determinants%20Public%20Data%20Sources.xlsx)

## How to access the Georgetown-SDOH datawarehouse
The information summarized in the Georgetown-SDOH database is accessible through multiple ways. Detailed tutorials are provided for each option
* Access using python scripts that can directly query the Georgetown-SDOH Bigquery datawarehouse 
(_easiest and most popular, hence highly recommended)_
* Access using R script 
* Directly querying the Georgetown-SDOH Bigquery datawarehouse using SQL-like commands 
_(read-only access offered on a case-by-case basis to a limited audience with experience in programming)_
* Access using BigQuery APIs _(future)_

## Request access
In order to request access to these databases, please email icbi@georgetown.edu

## Tutorials for advanced users
* Tutorial 1: How to extract information from the Georgetown-SDOH Bigquery datawarehouse using python scripts
  https://github.com/ICBI/Data.Bridge.Notebooks/blob/main/Goal1_SDOH/Tutorial1_BigQueryPythonGuide.ipynb
* Tutorial 2: Accessing the Georgetown SDOH Bigquery Datawarehouse through an API
  https://github.com/ICBI/Data.Bridge.Notebooks/blob/main/Goal1_SDOH/Tutorial2_BigQueryAPI.ipynb

<img src="https://github.com/ICBI/Data.Bridge.Notebooks/blob/main/HIDSLOGO.AA1.jpg" width="400" height="70">
