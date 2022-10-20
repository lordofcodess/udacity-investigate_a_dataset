# Project: No Show Appointment Data Analysis


## Introduction
### Dataset Description 

>In this project,the dataset shows information collected from 100k medical appointments in Brazil and analyzes whether or not patients show up for their appointment. A number of attributes about the patient are available in each row.

‘ScheduledDay’ - what day the patient set up their appointment.
‘Neighborhood’ - the location of the hospital.
‘Scholarship’ - shows if the patient is enrolled in Brasilian welfare program Bolsa Família or not.
The meaning of the other column names are also literal.

### Question(s) for Analysis
> What factors determine whether a patient will show up for a scheduled appointment or not?

## Data Wrangling
### Data Wrangling Summary
The data wrangling section contains code that displays general information about the loaded dataset. The number of rows and columns, some statistical data, etc. This is all to ascertain which parts of the data need to be cleaned. 

### Data cleaning summary
The dataset had to be modified for analysis to be more determinate. 
>##### The columns 'PatientId' and 'AppointmentID' were eliminated as they had no further use for analysis.
>##### The columns 'ScheduledDay' and 'AppointmentDay' which were stored as strings were converted to datetimes for easier working.
>##### Some columns with incorrect names were also corrected.
>##### Additionally, a new column was created using data from 'ScheduledDay' and 'AppointmentDay' to work with called 'WaitDays'.

## Exploratory Data Analysis 
From the explorative data analysis done, we can ascertain that sms received and waitdays play a large part in patients not showing up for appointments. The variables for each of the research questions were compared with other variables to see the correlation.

## Conclusions
There are no definite values to determine how much WaitDays, SMS_received and Age affected Noshows. But the exploratory analysis shows that WaitDays, and SMS_received affected whether patients showed up or not.
### Limitations
There were some limitations in the analysis. The datatype of the dates was a problem that I had to correct in order to create the column WaitDays. Also, the noshow column which was an important variable if it had been numerical would have been easier to detect trends between other variables.