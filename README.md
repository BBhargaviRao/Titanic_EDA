# Titanic_EDA
Exploratory Data Analysis on the Titanic Dataset

Author: Bhargavi Rao

What is Exploratory Data Analysis (EDA)?

Exploratory Data Analysis (EDA) is a fundamental step in the data science process. It involves analyzing datasets to summarize their main characteristics, often with visual methods, before applying more advanced techniques like machine learning models. In this project, I conducted EDA on the Titanic dataset to explore the relationships between passenger characteristics (age, class, gender, etc.) and their survival during the disaster.

How do we explore the Titanic dataset?

Step 1: Dataset Overview
The Titanic dataset provides detailed records of 418 passengers. It includes key features such as:

PassengerId: Unique identifier for each passenger.
Survived: Indicator of whether the passenger survived (1) or not (0).
Pclass: Passenger class (1st, 2nd, or 3rd).
Name, Sex, and Age: Personal information of each passenger.
SibSp and Parch: Number of siblings/spouses and parents/children aboard.
Fare: Fare paid by the passenger.
Embarked: The port from which the passenger boarded.
By examining this data, we aim to understand patterns in survival and make data-driven inferences.

Step 2: Understanding the Data

Before analyzing the data, we first inspect its structure to identify any missing or inconsistent values. The dataset has several features that require careful handling, such as missing values in the 'Age' and 'Fare' columns, and categorical data like 'Embarked' and 'Sex' that need to be transformed for analysis.

We also look at descriptive statistics and distributions to get a sense of the data's overall trends, such as average age, class distribution, and survival rate.

Step 3: Cleaning the Data

Data cleaning is essential to ensure that the analysis is accurate and reliable. Here, we handle missing values in the following ways:

Age: Filled missing values with the median age.
Embarked: Filled missing values with the most common port of embarkation.
Fare: Missing fare values are filled with the median fare.
By addressing these issues, we ensure that the dataset is ready for further analysis and that no biases arise from incomplete data.

Step 4: Data Visualizations

Visualization is a powerful tool in EDA, as it allows us to see patterns and relationships in the data that are not immediately obvious from raw numbers. Below are some of the key visualizations performed:

Age Distribution: A histogram of passengers' ages reveals a broad range, with a concentration of passengers in their 20s and 30s. This visualization helps us see which age groups were more common aboard the Titanic.
Survival Rate by Gender: A bar plot comparing survival rates between males and females shows a clear pattern — females had a much higher survival rate than males, likely due to the prioritization of "women and children first."
Survival Rate by Class: A bar plot showing survival rates across 1st, 2nd, and 3rd class passengers highlights that passengers in 1st class had the highest survival rate, while those in 3rd class were less likely to survive.
Correlation Heatmap: This heatmap shows the correlation between numerical features such as fare, class, and age. We can observe that passenger class is negatively correlated with survival, indicating that those in higher classes had better chances of surviving.


Step 5: Key Insights and Observations

Through this EDA process, several important patterns were uncovered:

Survival and Gender: Females had a significantly higher survival rate than males. This is consistent with the "women and children first" evacuation protocol followed during the disaster.
Survival and Class: Passengers in 1st class were more likely to survive than those in 3rd class. This could be due to their proximity to lifeboats and other factors associated with socioeconomic status.
Age and Survival: While passengers of all ages were aboard, children and younger passengers had slightly higher survival rates, suggesting that age might have played a role in the evacuation prioritization.
Fare and Survival: Higher fare-paying passengers (mostly from 1st class) had better survival chances. Fare can be seen as a proxy for socioeconomic status, which correlates with survival.
Missing Data: The dataset has significant missing data in the 'Cabin' feature. While 'Cabin' could provide interesting insights, it was dropped from the analysis due to the large proportion of missing values.

Conclusion

This Exploratory Data Analysis has revealed significant relationships between passenger characteristics and their chances of survival on the Titanic. The analysis shows that gender, class, and age were critical factors influencing survival rates, with women, children, and 1st class passengers having the highest likelihood of survival.

This EDA lays the groundwork for further analysis, such as building predictive models to estimate survival based on the identified features.


Future Work

In future steps, we could implement predictive models like logistic regression or decision trees to predict survival based on the features explored during this EDA. Additionally, it would be interesting to explore other potential factors, such as family size and their impact on survival rates.

