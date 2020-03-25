# Get-Clean-EDGAR-data

## Intro to SEC-EDGAR
EDGAR is a database that all companies, foreign and domestic, are required to file registration statements, periodic reports, and other forms electronically through.

## Project Goal
This project is done in March 2020, when working as intern at Global AI. All data is directly from EDGAR website through API and it's free so anyone can access it. This project's goal is to create two csv files, one for filing data of each file types of each company, e.g., information from 10-K/8-K/SC 13G file of Apple; the other for company data of each company.

## Source
The raw data is from EDGAR website, we use the sec_edgar_downloader package in Python to get the raw data. And the companies’ unique CIK(CENTRAL INDEX KEY), which is needed in the function to get the data, is downloaded from ’Company’ file on the EDGAR website (https://www.sec.gov/Archives/edgar/full-index/). The file types we deal with are: '8-K','10-K','10KSB','10-Q','13F-NT','13F-HR','SC 13G','SD' and 'S-1'.
According to the CIK, we have 17205 companies, each having 1-8 different files in different file types, available for data extraction (each file for different file types is the latest one).

## Code documentation
There is in-code documentation, brief but precise

## General
Please refer to the "Documentation.pdf" file to see the more detailed Readme.
