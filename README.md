# SAS_Airplane_Case_Study
In this case study, you solve a real-world business problem by applying concepts that you learned in the SAS Programming 1: Essentials course. Be aware that there are numerous solutions to this problem, and some can include concepts that are outside the scope of the SAS Programming 1 course.

# Background Information
You are a SAS programmer with six months of experience who is in charge of creating basic reports and maintaining SAS programs. Recently, you completed a SAS Programming course, and your supervisor gives you your first SAS programming project.

# Business Problem
Your first project is to prepare and analyze Transportation Security Administration (TSA) Airport Claims data from 2002 through 2017. The TSA is an agency of the United States Department of Homeland Security that has authority over the security of the traveling public. A claim is filed if you are injured or your property is lost or damaged during the screening process at an airport. To complete your project, you follow your supervisor's requirements, which are in Section 1.3 of this document. Here is what you need to do
• Prepare the data.
• Create one PDF report that analyzes the overall data as well as the data for a dynamically specified state.


To prepare and analyze the data, you follow the requirements given to you by your supervisor. Be aware that these requirements are only assumed for this case study. They are not an accurate representation of TSA requirements.

# Data Requirements
• Import the raw data file TSAClaims2002_2017.csv. 

• The final data should be in the permanent library tsa, and the data set should be named claims_cleaned. 

• Entirely duplicated records need to be removed from the data set.

• All missing and “-“ values in the columns Claim_Type, Claim_Site, and Disposition must be changed to Unknown. 

• Values in the columns Claim_Type, Claim_Site, and Disposition must follow the requirements in the data layout.

• All StateName values should be in proper case.

• All State values should be in uppercase.

• You create a new column named Date_Issues with a value of Needs Review to indicate that a row has a date issue. Date issues consist of the following:
 – a missing value for Incident_Date or Date_Received
 
 – an Incident_Date or Date_Received value out of the predefined year range of 2002 through 2017
 
 – an Incident_Date value that occurs after the Date_Received value
 
• Remove the County and City columns.

• Currency should be permanently formatted with a dollar sign and include two decimal points.

• All dates should be permanently formatted in the style 01JAN2000.

• Permanent labels should be assigned columns by replacing the underscores with a space. 

• Final data should be sorted in ascending order by Incident_Date.

# Report Requirements
The final single PDF report needs to exclude all rows with date issues in the analysis and answer the following questions:
1. How many date issues are in the overall data?
2. How many claims per year of Incident_Date are in the overall data? Be sure to include a plot.
3. Lastly, a user should be able to dynamically input a specific state value and answer the following:

 a. What are the frequency values for Claim_Type for the selected state?
 
 b. What are the frequency values for Claim_Site for the selected state?
 
 c. What are the frequency values for Disposition for the selected state?
 
 d. What is the mean, minimum, maximum, and sum of Close_Amount for the selected state? Round to the nearest integer.
