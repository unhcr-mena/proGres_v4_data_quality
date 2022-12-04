# data_quality

This repository contains jupyter notebooks (and reference data) used for quality checks on registration data of UNHCR's persons of concern (proGres v4) along with implementation of solutions (validation and/or correction of phone numbers and location spellings). 

The current implementation is meant for Egypt, but can be repurposed with minor changes to conduct data quality checks on other operations. 

Notebooks 00 and 01 identify irregularities in the following proGres v4 tables: individual, registration group, address, documents, and specific needs. 

## Guide for reproducibility:

1) Refer to the setup instructions and requirements listed in: 00_DQ_setup_instructions.xlsx and 00_requirements.txt
\n
2) To get data quality indicators (irregularities) associated with progres ids, run:
   01_data_quality_checks.ipynb
\n
3) To get data quality indicators (irregularities) associated with progres ids AND all the tables needed as input for the data quality PowerBi dashboard, run: 
   01_tables_needed_for_PowerBi_dashboard > 01_data_quality_checks_including_all_tables_needed_for_dashboard.ipynb
\n
4) Phone number validation:
   03_phone_number_validation > 03_phonenumber_validator.ipynb
\n
5) Location / Address spelling correction: 
   02_spelling_correction_for_location_names > 02_location_spelling_correction.ipynb
\n
6) Official admin names:
   04_get_official_admin_names_ocha_and_proGres_v4 > 04_Egypt_Syria_OCHA_vs_proGresv4_locations.ipynb
   \n *** OCHA names needed for input are available in the 'data' directory
