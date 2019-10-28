# The Data

Every year, the U.S. Consumer Product Safety Commission tracks emergency rooms visits to approximately 100 hospitals. The commission uses the resulting National Electronic Injury Surveillance System data to estimate national injury statistics, but it also publishes anonymized information for each consumer product–related visit, including the associated product code (e.g., 1701: “Artificial Christmas trees”) and a short narrative (“71 YO WM FRACTURED HIP WHEN GOT DIZZY AND FELL TAKING DOWN CHRISTMAS TREE AT HOME”). Here we are going to explore this data and see if we can find some interesting trends.

The NEISS injury data is gathered from the emergency departments (ED) of approximately 100 hospitals selected as a probability sample of all 5,000+ U.S. hospitals with emergency departments. The data set is large, it is long data with almost 7.5 million observations over 20 years. The data contains 19 variables, these include a unique identifier, the date of the incident, the patients age, gender, race, codes designating the event and a short text description. 

You can find more about the data here:
https://www.cpsc.gov/Research--Statistics/NEISS-Injury-Data

Each row is an individual case of a patient coming in to the emergency room. For the purpose of our exploration we will be focusing on the data from 1999

The data set contains the following columns:



| Column      | Data Type | Description |
| ----------- | ----------- |----------- |
| cpsc_case_number      | char       | unique identifier |
| treatment_date   | Posix ct        | date of the incident |
| age    | char       | age of the patient |
| sex   | num        | numeric sex identifier |
| race      | num       | numeric race identifier|
| body_part   | num        | numeric body part identifier |
| diagnosis| num       | numeric diagnosis identifier |
| other_diagnosis  | num        | numeric diagnosis identifier |
| disposition      | num      |numeric disposition identifier |
| location   | num       | numeric location identifier |
| fire_involvement      | num       | numeric fire involvement identifier |
| product 1   | num       | numeric product identifier |
| product_2      | num       | numeric product identifier |
| weight   | num    | patients weight |


For all of the columns labeled with 'identifier' can be found in the misc folder. The all of the data is encoded in there. I opted not to include it here as it is quite long.