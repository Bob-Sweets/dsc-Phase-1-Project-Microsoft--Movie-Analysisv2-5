# 1.1 Overview
The project's primary purpose is to generate insights that can assist Microsoft in entering and succeeding in the movie industry. We will utilize exploratory data analysis to get actionable insights to assist Microsoft determine what kind of films to develop. This project will leverage existing movie data to analyze box office trends, genre performance, and financial metrics to recommend strategic directions for Microsoft's new movie studio.

# 1.2 General Objectives
1. Identify Successful Film Genres: Determine which movie genres are performing best at the box office, both domestically and internationally.

2. Analyze Budgets versus Returns: Examine the relationship between film budgets and their financial success to identify optimal investment levels.

3. Understand Market Trends: Capture current trends in movie genres and preferences, including the most popular genre

4. Provide Strategic Recommendations: Translate findings into actionable strategies for genre selection, and budget allocation for Microsoft's studio.

# 1.3 Key Questions 
1. Which movie genres yield the highest box office earnings and ROI?
Aims to identify genres that consistently perform well, offering a safer investment for Microsoft.
2. What is the optimal budget range for producing a profitable movie?
Seeks to find a budget sweet spot that maximizes earnings without unnecessarily inflating costs.
3. How do movie budgets correlate with box office success?
Investigates whether higher budgets lead to higher gross earnings or if diminishing returns set in beyond a certain point.

# 2. Data Sets
The data sets are stored in the 'zippedData' folder which were sourced from:

- Box Office MojoLinks
    - bom.movie_gross.csv
- TheMovieDBLinks
    - tmdb.movies.csv
- The Numbers
    - tn.movie_budgets.csv

# Importing the relevant libraries

# Your code here - remember to use markdown cells for comments as well!
# importing libraries to load the data sets
   -import pandas as pd # Imports the pandas library, used for data manipulation and analysis, and aliases it as `pd`.
   -import matplotlib.pyplot as plt # Imports the pyplot module from matplotlib, a plotting library, and aliases it as `plt`.
   -import seaborn as sns # Imports seaborn, a statistical data visualization library based on matplotlib, and aliases it as `sns`.
   -import ast # For converting string representations of lists into actual lists in the 'tmdb.movies.csv'

%matplotlib inline

# Data Visualization
![alt text](<Screenshot 2024-03-22 at 3.19.01 AM.jpg>)

This bar graph shows Average Worldwide Gross by Primary Genre. The genres are listed on the y-axis, and their corresponding average worldwide gross earnings are on the x-axis. 

![alt text](<Screenshot 2024-03-22 at 3.19.21 AM 2.jpg>)
This is a bar graph that shows the Average ROI by Budget Tier. indicated by the tallest bar. As the budget tiers increase to 'Medium', 'High', and 'Very High', the ROI decreases. This pattern implies that investing in lower-budget movies might offer the best return on investment, while higher-budget movies may not always yield proportionally higher returns.

![alt text](<Screenshot 2024-03-22 at 3.19.26 AM 2.jpg>)
This is a scatter plot for production budget vs. ROI (Return on Investment). This shows the correlation between the two. The correlation suggests that there is a very weak negative linear relationship between the production budget and ROI. In practical terms, this means that as the production budget increases, there is a slight tendency for ROI to decrease.

# Conclusions 
From the findings we found that investing in lower-budget movies might offer the best return on investment, while higher-budget movies may not always yield proportionally higher returns.

We also found that some genres, typically those like Adventure, Action, or Fantasy, generate higher revenues on average compared to genres like Drama or Documentary. This suggests that movies in these high-grossing genres might be a safer bet for attracting a large audience and generating significant box office earnings.

# Reccomendations
Based on the insights gathered from the visualizations, here are some actionable recommendations for Microsoft's new movie studio:

-Focus on High-Grossing Genres:

   -Prioritize film production in genres that consistently show higher average worldwide gross, such as Animation, Adventure, and Action. These genres have proven market appeal and can lead to substantial box office earnings.
-Consider Moderate Budgets for Higher ROI:

   -Allocate investments in 'Low' and 'Medium' budget tiers where ROI is highest. While blockbuster budgets may attract attention, they do not necessarily guarantee a proportionally higher return on investment.
-Diverse Portfolio Approach: 
   -Since there's no strong correlation, it's advisable not to rely only on the budget as an indicator of profitability. The studio should consider a diverse portfolio of films, with a mix of budgets, to spread risk.
