![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Data Cleaning and Manipulation with Pandas

In this project I import the shark data base of the kaggle page https://www.kaggle.com/teajay/global-shark-attacks/version/1 , with the help of pandas I could see the database in a dataframe that I could manipulate and clean with the knowledge learned in class. In the end, the dimensions of the data frame were 5992 lines and 18 columns.Finally the data frame was saved to a csv file named clean_sharks.csv which is located in the output folder.


## Steps:

* First I import the libraries, pandas and numpy but also were useful the libraries requests and re, then pandas readed the csv file in a dataframe.

* Analyzed the dataframe content using .head(), .shape, .isnull().sum() to check the columns with the most null data.

* I looked at the data in the columns with the most null data ( Unnamed: 22 y Unnamed: 23) converting the columns into a set since they show us the different elements of the column this allowed me to see that they were not relevant columns and I decided to delete them using .drop() with axis=1

* Renamed the columns to make them easier to handle using .lower(), .strip(), .replace()

* I compared the contents of the href and href_formula columns and noticed that almost all the lines had both columns equal,so using a for loop and a .request() I could see which links in the href column serve and which do not, then change the links that do not serve the href column for the links in the column href_formula finally I was able to delete the column href_formula because i did not lose information. 

* Then I analyzed the sex column and saw that there were some different values of m and f (using .value_counts()) so I researched the data in those rows and was able to determine the type of sex and assign it(using .loc()), the same for fatal_(y/n) column. Also cleaned the data in the columns using .strip(), .lower() and .replace().

* I tried to delete duplicate lines with .drop_duplicates(), but I couldn't find.

* I checked if any of the numeric columns had little variability to be able to delete it but I did not find any with little variability.

* I analyzed the columns of case_number, case_numer.1 and case_number.2 and I saw that their content was repeated in almost all the lines, so I only analyzed and modified certain values of those lines and  I could delete the columns case_number.1 and case_number.2 with .drop().

* Then I went on to analyze the date column to see if I could delete the years column later, I modified various data to have the date format dd-month-yyyy to include the full year and most of the data have that format.But there are also other date formats like month-yyyy or yyyy or Before yyyy or Not date or yyyys or yyyy-yyyy these were the most common. Then I tried to clean up as much as I could the missing data, so that they adopted one of the formats mentioned, until there were very few, with different and more extensive formats.

* I decided not to delete the years column because it could be used to analyze the data later. But I decided to delete the original_order column because it didn't provide any information.

* I cleaned the data from the country, area, location, activity, type, time and species columns after analyzing their content taking a little more time with the species and time columns.

* I filled in the null data (in the columns that contained null data) with the word unknown.

* I renamed the name and species columns by victims and shark_information because the name column not only had names, also type of person/s that had attacked the shark, and the species column had a very detailed information of the shark that attacked.

* I checked the type of item that saved each column with .dytipes and changed the date column to string.

* Finally I saved the dataframe in a csv file in the output folder with .to_csv().
