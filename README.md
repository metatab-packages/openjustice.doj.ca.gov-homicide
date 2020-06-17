# Homicide in California

The Homicides in California file is publilshed by the California Department of Justices's [Open Justice](https://openjustice.doj.ca.gov) site. It collects reports from local law enformcement. From the website: 

> Information on homicides in California are reported by various LEAs as part of
> the reporting requirements for the Federal Uniform Crime Reporting (UCR)
> Program. These data provide detailed information about the circumstances of
> each homicide in addition to personal characteristics of the victim.

## Processing

The value label files were manually extracted from the data dictionary PDF. These files can be merged with the main homicide files to add human readable
labels to the values for these columns: 

* precipitating_event
* means_of_death
* location
* gender
* relationship
* race_ethnicity

The `race_ethnicity` column has two codes that map to the same race label for many race labels. For instance, both '1' and 'W' are codes for the label 'White'. These duplicate numeric codes have been replaced with the associated alpha code. 