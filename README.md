# Udemy Courses Data Analysis

# Introduction:
This project analyzes Udemy course data to uncover key insights about pricing, popularity, and course structure. 
The dataset contains 3,670 courses, including attributes such as price, number of lectures, content duration, subscribers, reviews, and subject categories.
Through data cleaning, exploration, and visualization, we examine patterns in course pricing, the relationship between lectures and content duration, and the impact of pricing on subscriber count. 
This analysis is performed in Python (Jupyter Notebook) and Tableau to provide interactive and visual insights.


## Dataset Overview
The dataset includes the following key attributes:
- course_id – Unique identifier for each course
- course_title – Title of the course
- is_paid – Indicates if the course is free or paid
- price – Course price in USD
- num_subscribers – Total number of enrolled students
- num_reviews – Number of course reviews
- num_lectures – Total number of lectures in the course
- content_duration – Total length of the course (in hours)
- published_timestamp – Date when the course was published
- subject – Subject category of the course
- duration_per_lecture – Newly calculated feature: average duration per lecture
- price_category – Newly categorized variable: groups courses into pricing segments


## Data Cleaning & Processing:
Before analysis, several cleaning steps were applied to ensure accurate results:

## Handling Outliers:
- Courses with excessively high lecture counts (outliers) were flagged and examined.
- Courses with many lectures but very short content duration were removed.
- Courses with 0 lectures and 0 content duration were eliminated.

## Feature Engineering:
- duration_per_lecture was calculated to check how long each lecture lasts on average.
- price_category was introduced to classify courses into different pricing tiers.

## Key Explorations & Visualizations
The project uses Python (Matplotlib & Seaborn) and Tableau for insightful visualizations:
- Course Pricing Analysis
- Distribution of course prices
- Comparison of free vs. paid courses
- Impact of pricing on subscriber count
- Subscriber Trends
- Which price category has the most subscribers
- Relationship between price and number of students
- Course Structure Analysis
- How num_lectures correlates with content_duration
- Identifying suspicious courses with unrealistic lecture-to-duration ratios
- Subject-Based Analysis
- Which subjects are the most popular (highest subscribers)?
- How pricing differs across subjects?
- Time-Based Trends
- Number of courses published over time
- How Udemy’s course offerings have evolved over the years

## Tools & Technologies
- Python (Jupyter Notebook) – For data cleaning and analysis
- Pandas & NumPy – Data manipulation and processing
- Matplotlib & Seaborn – Data visualization
- Tableau – Interactive visual dashboards

## How to Use This Project
- Open df_cleaned.csv in Tableau to explore visual insights.
- Run [udemy_analysis.ipynb](https://github.com/Mae-Shahvirdi/Udemy-Courses-Data-Analysis/blob/main/Udemy-Course.ipynb) in Jupyter Notebook for deeper analysis and Python-based visualizations.
- Modify price_category or duration_per_lecture logic if needed for more refined insights.

## Future Work
- Further analyze course engagement metrics (e.g., review ratings).
- Compare Udemy courses with other e-learning platforms (e.g., Coursera, Skillshare).
- Predict course success based on features using machine learning.
