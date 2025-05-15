# North American Data Validation

## Overview
This project focuses on data validation and logical mapping for North American suppliers, specifically targeting Canadian and American supplier datasets. The aim is to ensure structured, reliable, and high-quality data by addressing inconsistencies in address, city, province/state, and postal code information.

## Project Objective
The main objective is to automate and streamline the validation of supplier data using Python scripts, especially where ETL processes fail due to unstructured or incomplete inputs.
This script is designed to:

* Perform Exploratory Data Analysis (EDA) to detect irregularities.
* Apply robust logical mapping techniques to normalize and validate supplier information.
* Generate validation reports to highlight mismatches and direct attention to data that needs correction.

## The Problem
Canadian suppliers were not mapping correctly to their unique identifiers unless all key fields like province, city, postal code, and address were properly aligned. Although ETL pipelines exist to resolve such mappings, they were not reliable due to the unstructured nature of the input data.

This inconsistency led to:

* Failed or incorrect data mappings
* Dirty or incomplete downstream reporting
* Delays in report generation and delivery

## Solution
To overcome this, a custom Python-based validation framework was developed. This solution includes:

### Core Logic:

* Province and State normalization using predefined mappings
* City and postal code standardization
* Fuzzy matching for minor address variations
* A scoring system to evaluate record completeness and validity

## Features:

* Generates automated validation reports
* Flags records that need manual verification
* Easy integration into existing ETL or data ingestion pipelines
* Handles both Canadian and American supplier datasets

## Benefits

* Accelerates data quality assurance before ingestion into analytical reports
* Minimizes manual intervention by detecting issues upfront
* Improves accuracy in supplier profiling and reporting
* Enables structured and clean data flow into reporting tools
