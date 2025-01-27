## About

The Future of Families and Child Wellbeing Study (FFCWS) is an NIH-sponsored collaborative study that relied on a stratified, multistage sampling method encompassing 4,898 children born between 1998 and 2000. The study deliberately oversampled births to unmarried mothers at a ratio of 3 to 1, which ensured a comprehensive national representation of Black, Hispanic, and low-income families within the cohort. To date, there have been 7 waves of data collection at approximately ages 1, 3, 5, 9, 15, and 22, with the latest round commencing in late 2020. 

The Future of Families Sleep Sub-Study (Year 15 Wave 6) collected wrist-worn actigraphy sleep data from adolescents (14 to 18 years old) for one week (7 days) of a national diverse longitudinal birth cohort. Participants also completed a daily diary in which they answered questions about their mood, diet, physical activity, and screen use.

The NSRR FFCWS Sleep Actigraphy Dataset includes wrist-worn actigraphy data and daily diary from 923 participants (with at least 1 valid day of actigraphy data across a total of n = 5,491 daily actigraphy observations).

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

### Actigraphy epoch-by-epoch files


## Access and usage restrictions

The FFCWS dataset is only available for non-commercial use.

## Citation and acknowledgement

When using this dataset, users must cite the following:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
> 

Users must include the following text in any Acknowledgements:

> The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## Changelog

*January 2025*

- Make FFCWS dataset available for data requests

## References

- FFCWS on the National Sleep Research Resource (NSRR): https://sleepdata.org/datasets/ffcws/
- FFCWS GitHub Data Dictionary: http://github.com/nsrr/ffcws-data-dictionary
- FFCWS GitHub Documentation: https://github.com/nsrr/ffcws-documentation

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
