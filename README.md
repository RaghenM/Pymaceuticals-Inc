# Pymaceuticals-Inc
Data Science Bootcamp Module 5 

# Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

# Prepare the Data
- Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

- Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

- Display the updated number of unique mice IDs.

# Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:

- A row for each drug regimen. These regimen names should be contained in the index column.

- A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

# Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

- Create the first bar chart with the Pandas DataFrame.plot() method.

- Create the second bar chart with Matplotlib's pyplot methods.
<img width="574" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/7db2f44f-4a4f-436c-af51-678d1d66d573">

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

- Create the first pie chart with the Pandas DataFrame.plot() method.

- Create the second pie chart with Matplotlib's pyplot methods.
<img width="575" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/9e202143-b659-43c2-8bfc-9a19bb306978">

# Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

- Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

- Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

- Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

- Determine outliers by using the upper and lower bounds, and then print the results.
<img width="430" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/a5c865ab-d703-41e7-a8ec-e7d7a04f5dfc">

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.
<img width="665" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/e48d382b-dfa8-4974-8852-ea762c46b9a3">

hint: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

# Create a Line Plot and a Scatter Plot
- Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
<img width="602" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/8c917ac1-0ce1-4f90-be7b-2663d2ca99f2">

- Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.
<img width="555" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/dc34beb4-b8f2-43d5-b847-4512a7e36fef">

# Calculate Correlation and Regression
- Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

- Plot the linear regression model on top of the previous scatter plot.
<img width="544" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/e781f1ab-4f0a-40d0-b4f1-3777023cd41c">

# Observations 
<img width="812" alt="image" src="https://github.com/RaghenM/Pymaceuticals-Inc/assets/91345190/f9d443c9-2407-41f5-b0bb-aa19aa2b763a">
