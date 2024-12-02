# Project 2 Crowdfunding_ETL: Patrick Zhou and Natasha Elliott

**This mini project was divided into the following subsections:**
- Create the Category and Subcategory DataFrames
- Create the Campaign DataFrame
- Create the Contacts DataFrame
- Create the Crowdfunding Database

**Create the Category and Subcategory DataFrames**: Natasha

The Crowdfunding.xlsx data was extracted and transformed into a DataFrame with two columns “category_id” and “category”. This was then exported into a CSV titled “category”. The same was done again by creating another DataFrame with the columns “subcategory_id” and “subcategory” which was exported into a CSV titled “subcategory”.

**Create the Campaign DataFrame**: Patrick

Using the Crowndfunding.xlsc data again, another DataFrame was created with the following columns:
-	The "cf_id" column
-	The "contact_id" column
-	The "company_name" column
-	The "blurb" column, renamed to "description"
-	The "goal" column, converted to the float data type
-	The "pledged" column, converted to the float data type
-	The "outcome" column
-	The "backers_count" column
-	The "country" column
-	The "currency" column
-	The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
-	The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
-	The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
-	The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame

This DataFrame was exported into a CSV file titled “campaign”.

**Create the Contacts DataFrame**: Natasha

Using Python dictionary methods, the contacts.xlsx data was extracted and transformed into a DataFrame. Each row within the DataFrame was converted into a dictionary, splitting the name column into a "first_name" column and "last_name" column. The DataFrame was cleaned and exported into a CSV titled "contacts".

**Create the Crowdfunding Database**: Patrick

The four CSV files created were used to sketch an ERD of the tables. A table schema was created for each CSV file using the information from the ERD. A database was created using the table schema and each CSV file was imported into its corresponding SQL table and then verified the data. 

**Credits:** All code written by Patrick Zhou and Natasha Elliott.
