# Curated and Standardized Research Datasets

## About
ICBI faculty conduct research using public and proprietary datasets to advance Precision Medicine. They are involved in developing and applying Bioinformatics and Medical informatics methods to derive actionable knowledge from genomics, electronic health records, registries, patient-reported, public health and other datasets. 

Below is a list of specialized datasets that were co-developed by ICBI investigators and collaborators. These datasets are currently managed by ICBI and available to GUMC investigators for research use. Please contact the ICBI investigators listed under each dataset to initiate a collaboration.

## REMBRANDT (REpository for Molecular BRAin Neoplasia DaTa) Dataset 
**ICBI Investigators** – Yuriy Gusev, Krithika Bhuvaneshwar, Camelia Bencheqroun, Subha Madhavan

**Description**: The REMBRANDT dataset was originally created at the National Cancer Institute and funded by Glioma Molecular Diagnostic Initiative. The data was collected from 2004-2006. In 2015, the NCI transferred this dataset to Georgetown, and it is now physically located on the Georgetown Database of Cancer (G-DOC), a cancer data integration and sharing platform for hosting alongside other cancer studies. REMBRANDT includes genomic data from 261 samples of glioblastoma, 170 of astrocytoma, 86 tissues of oligodendroglioma, and a number that are mixed or of an unknown subclass. Outcomes data include more than 13,000 data points.

The dataset is accessible for conducting clinical translational research using the open access Georgetown Database of Cancer (G-DOC) (new window) platform. In addition, the raw and processed genomics and transcriptomics data have also been made available via the public NCBI GEO repository as a super series GSE108476 (new window). Such combined datasets would provide researchers with a unique opportunity to conduct integrative analysis of gene expression and copy number changes in patients alongside clinical outcomes (overall survival) using this large brain cancer study

**Raw data**: GSE108476
**MRI images**: The Cancer Imaging Archive (TCIA) (new window)
**Citations:** Gusev Y, Bhuvaneshwar K, Song L, Zenklusen JC, Fine H, Madhavan S. ‘The REMBRANDT study, a large collection of genomic data from brain cancer patients.’ Nature Scientific Data, Aug 2018.
Madhavan S, Zenklusen JC, Kotliarov Y, Sahni H, Fine HA, Buetow. Rembrandt: helping personalized medicine become a reality through integrative translational research. Molecular Cancer Research. Feb 2009.

## Georgetown Pediatric Cancer Outcomes Database
**ICBI Investigators**: Shruti Rao, Subha Madhavan

**Collaborators:** Aziza Shad, Kenneth Tercyak

**Description:** The Georgetown Pediatric Cancer Outcomes Database was co-developed by investigators at the Georgetown University Medical Center (GUMC) Lombardi Comprehensive Cancer Center (LCCC), the Pediatric Hematology Oncology and Bone Marrow Transplantation Program and ICBI. The 620 pediatric cancer patients (as of May 2015) in this database were diagnosed with various cancers at Lombardi Cancer Center’s Pediatric Oncology Program and were enrolled or treated as per Children’s Oncology Group (COG) protocols between 1990 and 2014. GUMC’s EMR systems – ARIA, AMALGA along with the paper charts were curated to obtain complete clinical information for these patients. Several retrospective research projects have been conducted on this pediatric cancer outcomes database such as – evaluation of secondary cancers in this patient cohort after therapy; assessment of risk factors associated with childhood cancer therapy and extracting predictor variables for late effects of childhood cancer treatments from clinical notes.

**Data Formats:** Excel/CSV, SAS, SPSS, R, Stata

## Georgetown Immuno Oncology Registry
**ICBI Investigators:** Adil Alaoui, Jia Li Dong, Camelia Camelia Bencheqroun, Samir Gupta, Subha Madhavan

**Collaborators:** Neil Shah, Michael Atkins, Chiranjeev Dash

**Description:** Our multidisciplinary team of clinicians and informaticians built a centralized research data warehouse for ImmunoOncology that is enabling novel hypothesis generation and retrospective outcomes research at the 10 DC-Baltimore based MedStar Health network hospitals. Data sources include hospital medical records, Labs, pathology, radiology, and Cancer Registry data. Data was extracted from different hospital systems and integrated into REDCap to allow clinicians to capture additional data from patient charts. Our integrative approach helps assess outcomes in patients with different comorbidities across all hospitals, effects of treatment with steroids on immune toxicities and their outcomes, use of various drugs before and during ImmunoOncology treatment and their impact on outcomes and toxicities. Toxicities and adverse events data in EHRs is not comprehensive. Hence, in addition to data extracted using ICD codes from structured fields/tables, we are using our in house developed NLP methodologies to automatically identify toxicities in patient charts. The Immuno Oncology registry has 758 patients as of Jan 2020.

**Data Formats:** Excel/CSV, SAS, SPSS, R, Stata

**Citations:** Shah NJ, Al-Shbool G, Blackburn M, Cook M, Belouali A, Liu SV, Madhavan S, He AR, Atkins MB, Gibney G, Kim C.’Safety and efficacy of immune checkpoint inhibitors (ICIs) in cancer patients with HIV, hepatitis B, or hepatitis C viral infection.’ J Immunother Cancer. 2019 Dec 17;7(1):353. doi: 10.1186/s40425-019-0771-1. PMID: 31847881

## CARIS Molecular Diagnostic Dataset
**ICBI Investigators:** Kanchi Krishnamurthy, Adil Alaoui

**Collaborators:** John Marshall

**Description:** Molecular profiling of any patient’s tumor identifies their disease biomarker pattern that then allows that patient’s medical team to select personalized treatment options that they may not have previously considered. ICBI investigators collaborated with the Ruesch center on a project that involves the molecular profiling of cancer patients seen at Georgetown. We obtained and analyzed test results of around 3900 patients (as of Jul 2019) from Caris Molecular Intelligence™ service with the ultimate goal of better informing treatment decisions. We are currently pursuing several projects centered around these datasets, including correlating survival with choice of standard vs personalized treatment, correlation of mutational burden and microsatellite instability in colorectal cancer, development of open-source visualization and analysis tools for molecular profiling, and comprehensive comparisons with public resources such as TCGA and AACR Genie.

Data Formats: Excel/CSV

## Stage II Colorectal Cancer – Multi-omics Molecular Profiling Dataset 
**ICBI Investigators:** Yuiry Gusev, Krithika Bhuvaneshwar, Subha Madhavan

**Collaborators:** Lou Weiner

**Description:** Colorectal cancer (CRC) patient biospecimens with extensive clinical and follow-up data were selected from the Indivumed GmbH biobank for 40 patients (20 relapse and 20 no-relapse). The patients consisted of 12 with late stage I, and 28 with stage II. Four patients (out of 12) with late stage I had experienced relapse (~33%), and it is important to note that 12 patients (out of 28) with stage II were relapse-free (~43%). Therefore, the relapse-free group of samples, and the group with relapse are both represented by a mixture of late stage I and stage II patients. Only nine stage II patients (out of 28) had rectal cancer; of these 6 had relapsed within 5 years. Of more than 180 clinical attributes, 64 were shortlisted based on relevance to clinical outcome and biomarker analysis. The molecular data included gene expression, DNA copy number, microRNA, serum and urine metabolites. 

**Data Formats:** Tab delimited text files

**Citations:** Subha Madhavan,,* Yuriy Gusev, Thanemozhi G. Natarajan, Lei Song, Krithika Bhuvaneshwar, Robinder Gauba, Abhishek Pandey, Bassem R. Haddad, David Goerlitz, Amrita K. Cheema, Hartmut Juhl, Bhaskar Kallakury, John L. Marshall, Stephen W. Byers, and Louis M. Weiner. ‘Genome-wide multi-omics profiling of colorectal cancer identifies immune determinants strongly associated with relapse’. Frontiers in Genetics, Nov 2013, 4: 236 

## ICBI Molecular Simulation Datasets 
**ICBI Investigators:** Matthew McCoy

**Description:** Protein structure simulation results generated from the SNP2SIM workflow, and used to develop protein specific models of variant function. Contains metadata on simulation configuration/parameterization, and output from Nanoscale Molecular Dynamics (NAMD) and Autodock Vina. 

**Data Formats:** NAMD output binaries (MD simulation results) or text files stored in the SNP2SIM defined file structure.

**Citations:**
* McCoy, M.D., Shivakumar, V., Nimmagadda, S. et al. SNP2SIM: a modular workflow for standardizing molecular simulation and functional analysis of protein variants. BMC Bioinformatics 20, 171 (2019). 
* McCoy, M.D., Madhavan, S. A Computational Approach for Prioritizing Selection of Therapies Targeting Drug Resistant Variation in Anaplastic Lymphoma Kinase. AMIA Joint Summits on Translational Science (2017). 

## OMOP-mapped Cancer Dataset 
**ICBI Investigators:** Shuo Wang, Kanchi Krishnamurthy, Adil Alaoui

**Description:** Our team is developing short and long-term strategies to map oncology-specific electronic health record data (EHR) hosted and managed in ARIA into the Observational Medical Outcomes Partnership common data model (OMOP CDM), which is one of the leading standard data models used in nationwide research and information sharing initiatives. OMOP was developed to be a shared analytics model and it has been adopted by the Observational Health Data Sciences and Informatics (OHDSI) Consortium. Our approach was to transform oncology EHR data and related databases into a common format as well as a common representation (terminologies, vocabularies, coding schemes), and then perform systematic analyses using a library of standard analytic routines that were developed and shared by the community based on the common data format.

## Bladder Cancer Dataset for Immuno Oncology analysis
**ICBI Investigators:** Yuriy Gusev, Krithika Bhuvaneshwar

**Collaborators:** Geoffrey Gibney

**Description:** This is a public gene expression dataset containing primary bladder cancer samples. It includes 165 primary bladder cancer samples, 23 recurrent non-muscle invasive tumor tissues, 58 normal looking bladder mucosae surrounding cancer and 10 normal bladder mucosae for microarray analysis. Available in NCBI GEO at Series GSE13507

**Data Formats:** Same as in NCBI GEO

## Pfizer grant with Medstar and Hackensack
**ICBI Team:** Yuriy Gusev, Krithika Bhuvaneshwar, Adil Alaoui, Camelia Bencheqroun

**Link** https://tma.georgetown.edu 

**Description**: Clinical pathways are systems-based tools for creating greater transparency around care decision making, therapeutic selection, and care delivery, and they improve quality and efficiency by reducing non value-added intra-provider variability in care. The goal of the project is to build a comprehensive clinical pathway system to increase the understanding and use of Next Generation Sequencing (NGS) in Non-Small Cell Lung Cancer (NSCLC) by general oncologists, pathologists, and oncology nurse navigators. This new and innovative pathway training system will make decision-making easier for clinicians who are trying to understand the appropriate tests and treatment algorithms for their patients. 
