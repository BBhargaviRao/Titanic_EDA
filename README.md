# **Exploratory Data Analysis on the Titanic Dataset**

**Author**: Bhargavi Rao

## **What is Exploratory Data Analysis (EDA)?**
Exploratory Data Analysis (EDA) is a fundamental step in the data science process. It involves analyzing datasets to summarize their main characteristics, often using visual methods and statistical techniques. In this project, I conducted EDA on the Titanic dataset to explore the relationships between passenger characteristics (age, class, gender, etc.) and their survival during the disaster.

## **Dataset Overview**
The Titanic dataset provides detailed records of 418 passengers, capturing various attributes such as age, class, gender, and survival status. By analyzing these features, our goal is to decipher the factors that determined survival rates during this historic maritime disaster.

## **Unique Approaches**

### **1. Feature Engineering and Interaction Terms**
One of the innovative approaches in this analysis is feature engineering, where we create new features to provide deeper insights beyond the raw data:

- **Family Size**: We computed the total number of family members aboard for each passenger by adding the SibSp (number of siblings/spouses) and Parch (number of parents/children) features. Larger family sizes might indicate more challenges during evacuation, potentially affecting survival rates.
  
- **Fare per Person**: We calculated the fare per person by dividing the fare paid by each passenger by their respective family size plus one. This metric provides a normalized view of the economic status of passengers relative to survival.

These engineered features enable a more nuanced analysis of survival factors, offering insights into the socio-economic dynamics aboard the Titanic.

### **2. Text Analysis of Passenger Names (NLP)**
Another innovative method employed in this project is Natural Language Processing (NLP) on passenger names:

- **Title Extraction**: Using NLTK (Natural Language Toolkit), we tokenized passenger names to extract titles such as "Mr.", "Mrs.", "Miss.", etc. These titles were then analyzed to understand social status and its impact on survival rates.

- **Insights from Titles**: Analyzing the distribution of titles among survivors and non-survivors provided insights into societal norms and their influence on rescue priorities.

This NLP approach adds a socio-cultural perspective to the analysis, revealing hidden patterns in how passenger identities shaped their survival probabilities.

## **Methodology**

### **Step-by-Step Analysis**

#### **Step 1: Loading and Cleaning the Dataset**
We started by loading the Titanic dataset and ensuring it was clean and ready for analysis. This involved handling missing values, converting categorical variables, and preparing the dataset for feature engineering and NLP tasks.

#### **Step 2: Feature Engineering**
- **Implementation**: We engineered features like Family Size and Fare per Person to enhance our understanding of survival patterns. These features were crucial in building predictive models and deriving meaningful insights from the data.

#### **Step 3: Text Analysis Using NLP**
- **Implementation**: Leveraging NLTK, we tokenized passenger names to extract titles. This allowed us to categorize passengers based on their social status and explore correlations between titles and survival rates.

#### **Step 4: Visualizations and Insights**
- **Visualization**: We visualized distributions of engineered features and analyzed survival rates based on these new insights. Visual representations such as histograms, bar plots, and correlation matrices were used to communicate findings effectively.

## **Key Findings**

### **Impact of Feature Engineering**
- **Family Size**: Larger families tended to have lower survival rates, suggesting challenges in evacuation coordination.
  
- **Fare per Person**: Passengers who paid higher fares per person had better survival chances, reflecting their priority in accessing lifeboats.

### **Insights from Text Analysis**
- **Titles**: Passengers with titles like "Mrs." and "Miss." had higher survival rates, indicating the prioritization of women and children in rescue efforts.

These findings provide a rich narrative of the human experience aboard the Titanic, illustrating the complex interplay of socio-economic factors and cultural norms during the disaster.

## **Conclusion**
In conclusion, this EDA on the Titanic dataset has demonstrated the power of feature engineering and NLP in uncovering hidden patterns and insights. By engineering new features and analyzing passenger names through NLP, we gained a deeper understanding of the factors that influenced survival rates. These approaches not only differentiate our analysis but also enrich our understanding of historical events through data-driven methodologies.

## **Next Steps**
- **Model Building**: Utilize the insights gained to build predictive models that estimate survival probabilities based on passenger attributes.
  
- **Further Analysis**: Explore additional variables such as cabin location or ticket class to enhance the predictive power of our models and uncover more insights into the Titanic disaster.
