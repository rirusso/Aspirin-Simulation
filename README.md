# Aspirin-Simulation

This repository contains the CSV files and code to run the simulation described in the paper "Self-administration of aspirin after chest pain for the prevention of premature cardiovascular mortality in the US: A population-based analysis." The purpose of this project was to quantify the potential population-level effect of self-administering aspirin within 4 hours of severe chest pain onset to reduce mortality post-AMI, using the US population as a case-study, and estimate the increased risk of death due to bleeding. The net impact on annual deaths, the years of life saved, costs and cost-effectiveness of this intervention were also estimated.

All data included in CSV files are provided in tables in the online supplementary materials. 

## CSV files

**MIcount.csv**
Acute myocardial infarction (AMI) related death counts from CDC Wonder 2019. Rows 1-10 correspond to males, and 11-20 correspond to females. 
_Column 1_ includes the most conservative definition of AMI, defined as the following ICD-10 Codes - I21 Acute MI; I46 Cardiac arrest
_Column 2_ includes the main analysis in which AMI was defined as the following ICD-10 Codes- I21 Acute MI; I22 Subsequent MI; I24 Other acute ischaemic heart disease; I46 Cardiac arrest; I49 Other cardiac arrhythmias; I51 Complications and ill-defined heart disease
_Column 3 _includes the least conservative definition of AMI, defined as the following ICD-10 Codes - I21 Acute MI; I22 Subsequent MI; I24 Other acute ischemic heart disease; I46 Cardiac arrest; I49 Other cardiac arrhythmias; I51 Complications and ill-defined heart disease

**CFR.csv**
1-year case fatality rate for ischemic heart disease (IHD) approximating AMI from Globorisk for the United States and Canada. Rows 1-10 correspond to males, and 11-20 correspond to females. 

**life_expect.scv**
CDC's National Vital Statistics Life Expectancy Estimates for the year 2018

**bleedingmortality.csv**
Excess bleeding (GIH and ICH) mortality rates per 100,000 persons from CDC Wonder 2019 including the following ICD 10 codes:  I61.0 (Intracerebral haemorrhage in hemisphere, subcortical); I61.1 (Intracerebral haemorrhage in hemisphere, cortical); I61.2 (Intracerebral haemorrhage in hemisphere, unspecified); I61.3 (Intracerebral haemorrhage in brain stem); I61.4 (Intracerebral haemorrhage in cerebellum); I61.5 (Intracerebral haemorrhage, intraventricular); I61.6 (Intracerebral haemorrhage, multiple localized); I61.8 (Other intracerebral haemorrhage); I61.9 (Intracerebral haemorrhage, unspecified); I62.0 (Subdural haemorrhage (acute)(nontraumatic)); I62.1 (Nontraumatic extradural haemorrhage); I62.9 (Intracranial haemorrhage(nontraumatic), unspecified); K92.2 (Gastrointestinal haemorrhage, unspecified)

**popdistribution.csv**
US population counts from US Census Bureau, 2019, by 5-year age and sex. Rows 1-10 correspond to males, and 11-20 correspond to females. 

## Aspirin Simulation 
The Rmd file "Aspirin Simulation" includes the model used to estimate the deaths delayed in this project using the data from the CSV files as well as estimates of sensitivity of chest pain, positive predictive value of chest pain for AMI, relative risk reduction of death due to aspirin, relative risk of excess bleeding due to aspirin, current aspirin use, and cost for aspirin. Detailed information on these parameters are available in Table 1: Model Parameters and Data sources. The file includes step by step instructions for running a model for deaths delayed from aspirin, deaths due to bleeding, years of life saved, costs, and costs per year of life saved.


