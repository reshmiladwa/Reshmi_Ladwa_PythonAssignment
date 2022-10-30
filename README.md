[Assignment File.docx](https://github.com/reshmiladwa/Reshmi_Ladwa_PythonAssignment/files/9895458/Assignment.File.docx)
# Reshmi_Ladwa_PythonAssignment
Assignment file for Data Analysis with Python 


#Import pandas. 
import pandas as pd

#Import numpy. 
import numpy as np

# Read the CSV file.
# Assign a variable.
# Use the pd.read_csv() function.
# Specify the name of the CSV file
import pandas as pd
ad = pd.read_csv('actual_duration.csv')

# Print the DataFrame for actual duration.
print (ad) 

# Read the CSV file.
# Assign a variable.
# Use the pd.read_csv() function.
# Specify the name of the CSV file.
ar = pd.read_csv('appointments_regional.csv')

# Print the DataFrame for appointments regional.
print (ar) 

# Read the CSV file.
# Assign a variable.
# Use the pd.read_excel() function.
# Specify the name of the Excel file.
nc = pd.read_excel('national_categories.xlsx')

# Print the DataFrame for national categories.
print (nc) 

#Print column names for ad
print (ad.columns)

#Print column names for ar
print (ar.columns)

#Print column names for nc
print (nc.columns)

#Descriptive statistics for ad
ad.describe()

#Meta data for ad
ad.info()

#Descriptive statistics for ar
ar.describe()

#Meta data for ar
ar.info()

#Descriptive statistics for nc
nc.describe()

#Meta data for nc
nc.info()

#Count number of different locations in data set
nc["sub_icb_location_name"].count()

#List of the different locations in the data set
nc["sub_icb_location_name"].value_counts( )

#Number of different locations 
print ("Count of locations:nc['sub_icb_location_name'].counts( )")

#List of different service settings
nc["service_setting"].value_counts()

#List of different context types
nc["context_type"].value_counts()

#List of national categories
nc["national_category"].value_counts()

#List of appointment statuses
ar["appointment_status"].value_counts()
