# The Data

Every year, the U.S. Consumer Product Safety Commission tracks emergency rooms visits to approximately 100 hospitals. The commission uses the resulting National Electronic Injury Surveillance System data to estimate national injury statistics, but it also publishes anonymized information for each consumer product–related visit, including the associated product code (e.g., 1701: “Artificial Christmas trees”) and a short narrative (“71 YO WM FRACTURED HIP WHEN GOT DIZZY AND FELL TAKING DOWN CHRISTMAS TREE AT HOME”). Here we are going to explore this data and see if we can find some interesting trends.

The NEISS injury data are gathered from the emergency departments (ED) of approximately 100 hospitals selected as a probability sample of all 5,000+ U.S. hospitals with emergency departments. The data set is large, it is long data with almost 7.5 million observations over 20 years. The data contains 19 variables, these include a unique identifier, the date of the incident, the patients age, gender, race, codes designating the event and a short text description. 

## Motivating Question

So! There is a lot of data regarding how people get injured. I'm really curious if the hospital emergency department could be more efficient if it could predict the types of injuries and individuals arriving on any given day. I think there is value in both staffing, supplies, etc. So here we will look at some data about hospital emergency room events and try to use it to generate a model that can be used to predict incoming patients.

The data set contains the following columns:

- cpsc_case_number char
- treatment_date   Posix xt
- age              char
- sex              num
- race             num
- body_part        num
- diagnosis        num
- other_diagnosis  num
- disposition      num
- location         num
- fire_involvement num
- product_1        num
- product_2        num
- weight           num