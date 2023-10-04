Working Records 
As we known we use rera dataset for model prediction and rera play very important role in our model prediction 

 
Rera is stand For :-

A RERA portal is a website that is maintained by a Real Estate Regulatory Authority (RERA). RERA is a statutory body that was established by the Real Estate (Regulation and Development) Act, 2016. The purpose of RERA is to protect the interests of homebuyers and to promote transparency and accountability in the real estate sector.
Rera store the all the information regarding construction industry which means in every state and city how many project are register , running and completed and data store along with their project category every project behave  in a different way and different pattern and trends .project category such as Residential/Group Housing, Commercial, Mixed Building(means in ground floor is build for shopping area or office and in  upper portion are build for staying)
The dataset appears to contain information about various real estate projects in India that are registered under RERA (Real Estate (Regulation and Development) Act). Here's a brief overview of some of the columns:


sheet: The source or region of the data.
conditional_formatting: Some kind of formatting or label, possibly related to the project's status or location.
project: Name of the real estate project.
project_res_no: A unique identifier or registration number for the project.
project_category: Category of the project (e.g., Mixed, Commercial).
estimated_commencement_date: Expected start date of the project.
actual_commencement_date: Actual start date of the project.
estimated_finish_date: Expected finish or completion date of the project.
total_built_up_area_saleable_area: Total saleable area of the project.
project_state: The state in India where the project is located.
Currently we have multiple state rera dataset which have multiple column and column details are:-Here are some of the columns in the dataset:
Here are some of the columns in the dataset:
sheet
conditional_formatting
unicode
project
project_res_no
project_category
estimated_commencement_date
actual_commencement_date
estimated_finish_date
total_built_up_area_saleable_area
project_state
Extended End Date
total_number_of_proposed_building
number_of_sanctioned_building
proposed_but_not_sanctioned_buildings_count
built_up_area_as_per_proposed_fsi
permissible_built_up_area
number_of_sanctioned_floors
number_of_basements
number_of_stilts




 In construction industry every Building and their  life cycle of making are  different which each category are behave are different and their life cycle is vary on the various factor such area of project , built_up area, floor , duration of project , builder details, these details are store on the rera 
Construction  industry is variable in nature 
For creating any type of model we should do data analysis firstly. Data Show pattern and trends 
Data speaks in its own way if we dive into the data it shows the pattern. Data show different patterns and combinations of behaviour 
Data analysis means:-
Data analysis is important for model prediction because it helps to ensure that the model is trained on high-quality data and is able to generalize well to new data.
Here are some specific ways that data analysis can improve model prediction:
Identify and remove outliers. Outliers are data points that are significantly different from the rest of the data. They can skew the results of a model and lead to inaccurate predictions. Data analysis can help to identify and remove outliers from the training data.
Feature engineering. Feature engineering is the process of transforming raw data into features that are more informative and useful for the model. Data analysis can help to identify which features are most important for the model and to transform the data into these features.


In data analysis we use handle missing value which create very big impact on the data quality because if  data have missing value its  can not show any patterns and for machine learning prediction we have provide  good quality data for better prediction.
Here's the number of missing values present in each column:
sheet: 0
conditional_formatting: 9,412
unicode: 13,616
project: 19
project_res_no: 20
project_category: 1,144
estimated_commencement_date: 13,724
actual_commencement_date: 265
estimated_finish_date: 23
total_built_up_area_saleable_area: 82
phase_area: 13,618
open_area: 13,618
proposed_but_not_sanctioned_number_of_apartments_plots: 13,618
total_area_of_project: 12
floor: 14,696
project_state: 345
Extended End Date: 16,265
total_number_of_proposed_building: 16,265
number_of_sanctioned_building: 16,265
proposed_but_not_sanctioned_buildings_count: 16,265
built_up_area_as_per_proposed_fsi: 16,265
permissible_built_up_area: 16,265
number_of_sanctioned_floors: 16,265
number_of_basements: 16,265
number_of_stilts: 16,265
Several columns have a significant amount of missing data. Depending on your objective, you might want to consider strategies for handling these missing values. This could involve imputation, removal of certain rows or columns, or simply acknowledging the missing data in your analysis.




The method to fill missing values in the estimated_commencement_date column depends on the nature of the data and the context. Here are some common strategies:
Forward Fill or Backward Fill: Fill missing values with the previous (or next) non-missing value. This is useful when data is sequential.
Using Other Columns: If there's a relationship between estimated_commencement_date and other columns, we can use those columns to estimate the missing values.
Median or Mode: Fill missing values with the median or mode of the column.
Interpolation: Useful for time series data where you want to fill in gaps.
External Data: If there's another data source that can provide the missing dates, it can be used to fill the gaps.
Machine Learning: Train a model to predict the missing values based on other features.
Project which have in the our Rera Dataset:


This bar chart provides a clear visual representation of the distribution of projects across these states.
Gujarat has the highest number of projects, followed by Uttar Pradesh, Rajasthan, and then Haryana.

Here's the number of projects for each state from the reloaded dataset:
Gujarat: 9,392 projects
Uttar Pradesh: 3,079 projects
Rajasthan: 2,330 projects
Haryana: 1,119 projects




We check the pattern of last 3 years upcoming and running project its shows us more reliable pattern of project details and there pattern to analyze on the dataset 
There are 1,934 projects that commenced in 2021. 
Distribution of Project Durations: A histogram or density plot to show how long most projects take from commencement to estimated completion.




The histogram above displays the distribution of project durations for projects that started in 2021. Here are some observations:
A significant number of projects have shorter durations, roughly between 0 to 500 days.
There's a noticeable peak around 1,400 days, suggesting several projects have an estimated duration of roughly 4 years.
Fewer projects have very long durations beyond 2,000 days.
As we see the above graph show the most of the project 4 years to complete the project its avg time time duration of project around 1500 days 
Yearly completion patterns.
This will help understand in which years and months the maximum projects are slated for completion.



The bar chart displays the yearly completion pattern for projects that started in 2021. Here are some observations:


A significant number of projects are expected to be completed in 2022, followed by a gradual decrease in the subsequent years.
By 2026 and beyond, the number of projects expected to be completed becomes relatively low.
It's interesting to note that some projects even extend into 2030 and 2031, suggesting they have long durations.






Monthly Completion














































The line chart above displays the monthly completion pattern for projects that began in 2021. Here are some observations:
There are peaks in project completions at certain months, such as mid-2022, late 2023, and early 2024.
After 2024, there's a more even spread, with smaller peaks occurring at regular intervals.
Towards the end of the timeline (late 2030 and 2031), fewer projects are slated for completion.
The visualization provides a granular view of when projects are expected to be completed on a monthly basis over the coming years.









The scatter plot illustrates the relationship between the project duration (in days) and the total built-up area (saleable area):
A bulk of the projects, regardless of their size, tend to have durations clustered between 0 to around 2,000 days.
There doesn't appear to be a strong linear correlation between the project size and its duration. This means that larger projects don't necessarily take longer, and smaller projects don't always finish quicker.
However, there are some outliers, especially in the built-up area, suggesting a few significantly large projects in terms of saleable area.

