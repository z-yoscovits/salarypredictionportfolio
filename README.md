Salary Prediction Project(Python)
This purpose of this project is to use HR data about 1 million job salaries and information about the jobs to predict salary. This prediction can be used to ensure future job offers have a salary that is competitive with the market.

Methodology
    • Data Cleaning -Checked for null values and duplicates.  Checked outliers and removed data with zero salary
    • Exploratory Data Analysis - Analyzed the data and visualized the each column with graphs of distribution of the data, and plotted it against salary.  Also created a heat map showing correlation between each column.
    • Feature Engineering – Encoded categorical features using one hot encoding and ordinal encoding, also created target mean encoding column.
    • Machine Learning Algorithms Used -  Random Forest and Gradient Boosting.
    • Evaluation Metrics Used - Root Mean Squared Error(RMSE).
    
Technologies/Libraries Used
 - Python 3
 - Jupyter
 - Pandas
 - Numpy
 - Seaborn
 - Matplotlib
 - Scikit-Learn
 
 
Dataset Information
This dataset appears to have been previously cleaned as it has no missing or duplicate data.  The raw data consists of a training dataset with the features - jobType, degree, major, industry, yearsExperience and milesFromMetropolis and their corresponding salaries. 
There is also a testing dataset that does not have any salary information available and was used as a substitute for real-world data and used the model to predict it's values/salaries.

Information Used to Predict Salaries
    • Years Experience: How many years of experience
    • Job Type: The position held (CEO, CFO, CTO, Vice President, Manager, Janitor, and senior or junior position)
    • College Degree: Doctoral, Masters, Bachelors, High School, or None
    • College Major: Biology, Business, Chemistry, Computer Science, Engineering, Literature, Math, Physics, or None
    • Industry: Auto, Education, Finance, Health, Oil, Service, or Web
    • Miles From Metropolis: How many miles away from a major city
Summary
Using a Random Forest regressor without  target encoding resulted a model that performed very near the best, but in a much shorter time.   The result was a root mean squared error of 19.6.  This model can be used as a guide when determining salaries since it leads to reasonable predictions when given information on years of experience, miles from metropolis, job type, industry, and college degree and major.
