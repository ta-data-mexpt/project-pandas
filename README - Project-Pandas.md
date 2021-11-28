
# Process

## Importing

there were 3 libraries that were used in this project 

import pandas as pd	 		### the main one for this project in order to manipulate information
import re 					### To manipulate strings in a easy way 
from dateutil import parser ### to check if one date is valid or it is not

## Cleaning

### Date

As our lab lab-String-Operations, I will have a bag of words where all trash information should be containded there. this step was thought if one day business people decide some of that information is useful for the analysis. to populate this bad of words, i have checked if replacing a space to '-' is a valid date in a new varaible, if it is,the process can continue (this part had been though like this since previous analysis of the column), if it is not, will check if every token previously splitted is a valid date, if it is not, it should be saved in our bag of words.

after all information had been saved, I started checking again each record of that column and then removing all information that is contained in bag of words.

Regarding year information, the one that is considered as the real one is Date column, so if there is a discrepancy between Date and Year column, Year column would be used as the correct one

NOE: will take all records that contains a valid date as real one, unless it will be checked with business

### Year

this column has strong relation with Date, so, the first column cleaned was Date, that is my base to clean Year Column, valid Year mentioned in Date can be considered as a good one if Year column does not have value, if this is the case, Year should be equal to Year mentioned in Date column and Date value is set as "No date"

if Year is equal to 0 and Date is equal to 'No Date' value, records will be removed, since there is no relevant information for us.

### Type

This column does not have a lot of information to clean, so values changed are:
	Boating -> Boat
	Invalid -> Unknown

### Species

First of all name of the column should be changed since there is a space in there, then I checked whichs shark's species are present in our column and put all of them in a list (the rule followed here is find all substrings that cointans one word with at least 3 letters and "Shark" or "shark" word), after doing that analysis was started with lots of types of sharks. All of them have been investigated in Google in order to know which ones are a valid ones.

in this moment we were able to use apply method with a function as a parameter which is going to help us to clean this data.

### Fatal(Y/N)

I can see there are some values that are very similar, some of them have spaces in there, or lowercase instead of an standard one. As first step have applied a uppercase function with a strip then all "nan" have been populated with "UNKNOWN", all strange characters have populated in same way. the only special case to be populated was an "F" value which can be considered as "Fatal" so it has bene populated with 'Y'

### Sex

Have previously checked this column doing a head(40) function and realized there are some sex name in name colum like 'Male, Female, Girl, Boy', so to get over this, a new column had been defined (Sex_in_name) which is going to contain all sex values that appear in name column. Doing that, I was able to fill na values in sex column with that value, if there were Null value, those should be set as "Unknown", in the previouls analysis I could see there are some characters as ill,.,N which basically do not know exactly how to consider them, so they were excluded remplacing them by 'Unknown' word.   






