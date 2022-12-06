[This data is published under an [Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) license](https://creativecommons.org/licenses/by-nc-sa/4.0/)]

# About this story

Data behind the Washington Post [story](https://www.washingtonpost.com/investigations/interactive/2022/fatal-police-shootings-unreported/): As fatal police shootings increase, more go unreported

From The Washington Post's [Fatal Force](https://www.washingtonpost.com/graphics/investigations/police-shootings-database/) project [[github]](https://github.com/washingtonpost/data-police-shootings).

# Methodology

To determine which police departments report fatal police shootings to the federal government, The Post used text-matching techniques and some manual adjustments to add federal identifier codes to each police department in The Post’s Fatal Force database. This allowed the Fatal Force data to be joined with the FBI’s Uniform Crime Reporting data for deeper analysis. For this project, reporters compared The Post’s count of police shootings by department to police-involved justifiable homicides tracked by the FBI’s Supplementary Homicide Data in its Uniform Crime Reporting Program. Many police departments have begun reporting to the FBI’s newer National Incident-Based Reporting System over the past few years, but because that system is not yet as widely adopted, the FBI said that it still incorporates NIBRS data into UCR. The Post reached out to more than 150 law enforcement agencies to explain their missing figures. Only a third responded.

The Post’s Fatal Force methodology assigns a shooting to the police department of the officer involved, regardless of where the shooting occurred. The FBI’s UCR policy is to assign a shooting to the jurisdiction where the shooting occurred, even if an officer from an outside agency was responsible. For this reason, there may be more shootings for certain agencies in the FBI data than in Fatal Force. Some departments may have submitted their data to their state but may not appear in the FBI’s data because they did not meet federal coding standards, such as Florida since 1996.

To compare agencies’ rates of shootings, reporters determined the average annual number of people killed by an agency per 1,000 officers. The Post retrieved department staffing figures from the FBI’s Crime Data API and drew on The Post’s Fatal Force data on police shootings. To account for small populations, the rates for the smallest 5 percent of agencies with shootings were excluded. While The Post incorporated shooting numbers from federal and state agencies into its top-line national figures, the analysis at a state and local level focuses only on local police departments and sheriff’s agencies. For comparing similarly sized departments in the table, searches are matched to nearby departments in the same nationwide decile in terms of number of officers.

Figures for years without officer counts were extrapolated from the average of officer counts submitted by the agency in other years. Historical SHR and NIBRS data were provided by Jacob Kaplan of the Princeton School of Public and International Affairs.
Grant figures for the National Crime Statistics Exchange and the Justice Assistance Grant program were pulled from the Justice Department’s data portal and excludes statewide grants. Only grants marked “closed” were considered in The Post’s tally.

The Post’s examination of states with laws requiring the reporting of fatal police shootings counted only those laws that include language requiring agencies to disclose the number of fatal shootings by police, all shootings by police, officer-involved deaths, law enforcement-related deaths, arrest-related deaths, justifiable homicides, the use of deadly force, the use of deadly physical force resulting in death, or the use of force or weapons discharges. Laws that require reporting only if it is requested by the state were excluded.


### Data sources

- Washington Post - Fatal Force database [[link](https://github.com/washingtonpost/data-police-shootings)]
- FBI Crime Data API [[link](https://crime-data-explorer.fr.cloud.gov/pages/docApi)]
- FBI Supplementary Homicide Reports, Jacob Kaplan (1976 - 2021) [[link](https://www.openicpsr.org/openicpsr/project/100699/version/V11/view)]
- DOJ Bureau of Justice Assistance grants [[link](https://data.ojp.usdoj.gov/Funding-API/Funding/a7v8-ei2f)]

# Files of note in this repo

* **[data/grants.csv](data)** - slice of DOJ grants data specific to UCR and identified police departments (must be joined to DOJ [grant data](https://data.ojp.usdoj.gov/Funding-API/Funding/a7v8-ei2f))
* **[data/shr.csv](data)** - summarized Supplementary Homicide Reports data showing total homicide counts and total police-involved homicides between 2015 and 2021
* **[data/State_Laws.xlsx](data)** - categorization of state laws as well as links compiled by Marisa Iati and Claire Healy

# Notebook on how to analyze with our data

* [Analysis](http://wpinvestigative.github.io/fatal_force_unreported/analysis.html) - Analyzing your own police department


### Staff involved

Reporters: [Andrew Ba Tran](https://www.washingtonpost.com/people/andrew-ba-tran/), [Marisa Iati](https://www.washingtonpost.com/people/marisa-iati/), [Claire Healy](https://www.washingtonpost.com/people/claire-healy/)

Editors: Meghan Hoyer and Sarah Childress

Jennifer Jenkins, Paige Moody, Julie Tate, Steven Rich, Monika Mathur and Razzan Nakhlawi contributed to this report.

