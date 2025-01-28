## About

The [Future of Families and Child Wellbeing Study (FFCWS)](https://ffcws.princeton.edu/) is an NIH-sponsored collaborative study that relied on a stratified, multistage sampling method encompassing 4,898 children born between 1998 and 2000. The study deliberately oversampled births to unmarried mothers at a ratio of 3 to 1, which ensured a comprehensive national representation of Black, Hispanic, and low-income families within the cohort. To date, there have been 7 waves of data collection at approximately ages 1, 3, 5, 9, 15, and 22, with the latest round commencing in late 2020. 

The Future of Families Sleep Sub-Study (Year 15 Wave 6) collected wrist-worn actigraphy sleep data from adolescents (14 to 18 years old) for one week (7 days) of a national diverse longitudinal birth cohort. Participants also completed a daily diary in which they answered questions about their mood, diet, physical activity, and screen use.

The NSRR FFCWS Sleep Actigraphy Dataset includes wrist-worn actigraphy data and daily diary from 923 participants with at least 1 valid day of actigraphy data across a total of n = 5,491 daily actigraphy observations.

## Methods

### Home Visit

The home visit was conducted during Year 15 (Wave 6); a randomly selected sub-sample of N = 1,090 participating in Year 15 home visits was asked to wear a Philips Spectrum 7 accelerometer on their non-dominant wrist for seven consecutive days to track their sleep. This sub-sample also completed a daily diary in which they answered questions about their mood, diet, physical activity, and screen use on Qualtrics.com at approximately 19:00 (7:00 PM) each night.

The diary collected data on the subject’s previous night's sleep quality and activities, as well as behaviors and mood throughout the following day. The publicly available information includes school attendance and schedule, media usage, reading, homework time, mood, and details on breakfast and caffeine intake. These inquiries pertained to the duration from bedtime until the beginning of the next day's journal entry.

### Actigraphy collection

Calculated actigraphy data was collected using a Philips Spectrum 7 accelerometer on their non-dominant wrist during Year 15 for seven consecutive days. Data collection occurred from 2014 to 2016 and during all months of the year, including summer months. The participants were instructed to wear the actigraphy watch all the time, day, or night, except when the watch could be damaged (participating in contact sports or exposed to extreme temperatures). The watch was water resistant, but participants were asked to take the device off while bathing or swimming. Following the study period, the participants mailed the devices to a data coordinating center (Westat). Staff at Westat downloaded the actigraphy recording from each device using Philips Actiware software version 6.0.4 and shared it with staff in the Sleep, Health, and Society Collaboratory (SHSC) at Penn State via Secure File Transfer Protocol (SFTP). Staff in the SHSC exported the 30-second epoch data from Actiware 6.0.4 to CSV files in preparation for scoring. The medium sensitivity wake threshold option in the software (40 counts per minute) was selected for calculating sleep variables.

### Actigraphy scoring

Two independent, trained scorers viewed and scored each recording using a validated algorithm (see 2013 Marino et al. Sleep; DOI: 10.5665/sleep.3142). Scorers determined sleep intervals by using the AMBER 1.0 interface to determine a decrease in activity levels and the aid of light levels for sleep onset and sleep offset. Scorers determined cut-point times, validity of days, and set sleep intervals, without using information from a sleep diary. 

- _Cut-point times_: Determined by the “start” and “end” of a 24-hour day. The preferred cut-point was noon for each recording. This time could be shifted to select a time that intersects the minimum number of sleep periods and off-wrist periods for a given recording.
- _Valid days_: Determined by the amount of time a participant had their accelerometer on. Each accelerometer had an on-wrist detection feature that allowed scorers to view when participants were not wearing the device.
- _Naps_: Defined as 30 continuous minutes of diminished activity outside of the main sleep interval. 
- _Night sleep_: Sleep interval that was measured if there was an awakening period of 1 hour or more during the nighttime sleep interval.
- _Sleep onset_: Defined as the nighttime sleep duration start time. Also determined as the time of the first 30-second epoch with activity count that was >10 counts preceded by 5 consecutive 30-second epochs < 10 counts. The accelerometer must have been worn at least two hours before this onset period.
- _Sleep offset_: Defined as the nighttime sleep duration end time. Also determined as the time of the first 30-second epoch with activity count that was >10 counts preceded by 5 consecutive 30-second epochs < 10 counts.
- _Rest periods_: Scorers determined sleep intervals using a decrease in activity levels and the aid of light levels for sleep onset and sleep offset

## Data de-identification

All personally identifiable information (PII) has been removed from the data files by the NSRR team.

## Data overview

### Covariate/phenotype datasets (CSV)

The [covariate dataset files](:files_path:/datasets) (**ffcws-dataset-0.1.0.csv** and **ffcws-harmonized-dataset-0.1.0.csv**) contain 923 rows respectively. The first column ([idnum](:variables_path:/idnum)) is the unique FFCWS subject identifier. The **ffcws-dataset** file is a combination of two (2) [original datasets (ffcws_yr15_demo_20240806 and ACT_wave62024v2)](:files_path:/original).

The dataset columns are described in the accompanying data dictionary files. The variables data dictionary file includes column names (id), labels (display names), descriptions, and other metadata. Categorical variables also include an associated "domain" (e.g., 1=Male, 2=Female), which are described in the domains data dictionary file. 

The history of the covariate dataset and data dictionary files have been tracked on GitHub (https://github.com/nsrr/ffcws-data-dictionary). 

The harmonized-dataset contains many of the most frequently used demographic and sleep variables. These variables were curated by the NSRR team. Key variables include:

  <table>
    <tr><td><b>Variable</b></td><td><b>Label</b></td></tr>
    <tr><td><a href=":variables_path:/nsrr_age">nsrr_age</a></td><td>Subject age</td></tr>
    <tr><td><a href=":variables_path:/nsrr_sex">nsrr_sex</a></td><td>Subject sex</td></tr> 
    <tr><td><a href=":variables_path:/nsrr_race">nsrr_race</a></td><td>Subject race</td></tr> 
  </table>

### Original demographic and actigraphy data files

The [original demographic and actigraphy data files](:files_path:/original) are  available for download. 

  <table>
    <tr><td><b>Dataset</b></td><td><b>Description</b></td></tr>
    <tr><td>ffcws_yr15_demo_20240806</td><td>Demographics (also available [here](https://sleepdata.org/datasets/ffcws/variables?folder=Sociodemographics))</td></tr>
    <tr><td>ACT_wave62024v2</td><td>Summary actigraphy results</td></tr> 
    <tr><td>dailysleep_wave6</td><td>Daily actigraphy and diary data</td></tr> 
    <tr><td>FFCWS_YR15_stacked_idnum</td><td>Epoch-by-epoch (30-second) actigraphy data</td></tr> 
  </table>

The [FFCWS public data documentation website](https://ffcws.princeton.edu/data-and-documentation/public-data-documentation) includes a comprehensive description of the data collection methods and available data. 

Actigraphy (Sleep Study) documentation can be found here: 

- https://ffcws.princeton.edu/sites/g/files/toruqf4356/files/documents/ff_age_15_sleep_data_documentation_20220128.pdf
- https://ffcws.princeton.edu/sites/g/files/toruqf4356/files/documents/FF_Y15_DailyActigraphy-diary_documentation_2023.09.07.pdf

## Access and usage restrictions

The FFCWS dataset is only available for non-commercial use.

## Citation and acknowledgement

When using this dataset, users must cite the following:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
> 
> [Master L, Nye RT, Lee S, Nahmod NG, Mariani S, Hale L, Buxton OM. Bidirectional, Daily Temporal Associations between Sleep and Physical Activity in Adolescents. Sci Rep. 2019 May 22;9(1):7732. doi: 10.1038/s41598-019-44059-9. PMID: 31118441; PMCID: PMC6531611.](https://pubmed.ncbi.nlm.nih.gov/31118441/)

Users must include the following text in any Acknowledgements:

> The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002). Research reported in this publication was supported by the Eunice Kennedy Shriver National Institute of Child Health and Human Development (NICHD) of the National Institutes of Health under award numbers R01HD073352 (to LH), R01HD36916, R01HD39135, and R01 HD40421, as well as a consortium of private foundations.

<details>
<summary>Other key FFCWS citations (click to expand)</summary>
<br>
<ul>
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/37138384/" target="_blank">Master L, Nahmod NG, Mathew GM, Hale L, Chang AM, Buxton OM. Why so slangry (sleepy and angry)? Shorter sleep duration and lower sleep efficiency predict worse next-day mood in adolescents. J Adolesc. 2023 Aug;95(6):1140-1151. doi: 10.1002/jad.12182. Epub 2023 May 3. PMID: 37138384; PMCID: PMC10524335.</a>
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/35010906/" target="_blank">Mathew GM, Reichenberger DA, Master L, Buxton OM, Chang AM, Hale L. Too Jittery to Sleep? Temporal Associations of Actigraphic Sleep and Caffeine in Adolescents. Nutrients. 2021 Dec 23;14(1):31. doi: 10.3390/nu14010031. PMID: 35010906; PMCID: PMC8746933.
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/35715858/" target="_blank">Mathew GM, Reichenberger DA, Master L, Buxton OM, Hale L, Chang AM. Worse sleep health predicts less frequent breakfast consumption among adolescents in a micro-longitudinal analysis. Int J Behav Nutr Phys Act. 2022 Jun 17;19(1):70. doi: 10.1186/s12966-022-01265-5. PMID: 35715858; PMCID: PMC9205101.</a>
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/37410005/" target="_blank">Mathew GM, Reichenberger DA, Master L, Buxton OM, Chang AM, Hale L. Actigraphic Sleep Variability is Associated With Lower Positive Mood in Adolescents. J Adolesc Health. 2023 Sep;73(3):478-485. doi: 10.1016/j.jadohealth.2023.04.019. Epub 2023 Jul 6. PMID: 37410005; PMCID: PMC10524712.</a>
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/29157638/" target="_blank">Nahmod NG, Lee S, Buxton OM, Chang AM, Hale L. High school start times after 8:30 am are associated with later wake times and longer time in bed among teens in a national urban cohort study. Sleep Health. 2017 Dec;3(6):444-450. doi: 10.1016/j.sleh.2017.09.004. Epub 2017 Oct 16. PMID: 29157638; PMCID: PMC5726563.</a>
	<li>
		<a href="https://pubmed.ncbi.nlm.nih.gov/30395345/" target="_blank">Nahmod NG, Lee S, Master L, Chang AM, Hale L, Buxton OM. Later high school start times associated with longer actigraphic sleep duration in adolescents. Sleep. 2019 Feb 1;42(2):zsy212. doi: 10.1093/sleep/zsy212. PMID: 30395345; PMCID: PMC6369724.</a>

</ul>

</details>

## Changelog

*January 2025*

- Make FFCWS dataset available for data requests

## References

- FFCWS Princeton University website: https://ffcws.princeton.edu/
- FFCWS on the National Sleep Research Resource (NSRR): https://sleepdata.org/datasets/ffcws/
- FFCWS GitHub Data Dictionary: http://github.com/nsrr/ffcws-data-dictionary
- FFCWS GitHub Documentation: https://github.com/nsrr/ffcws-documentation

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
