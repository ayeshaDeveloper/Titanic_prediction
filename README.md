# Titanic Dataset Analysis

## Overview
This project analyzes the Titanic dataset to explore the survival probability of passengers during the RMS Titanic disaster. Using machine learning techniques and extensive data visualization, we uncover key variables that significantly impact survival rates. The dataset includes passenger details such as age, sex, class, fare paid, and survival, which are crucial in understanding the demographic and socioeconomic factors influencing survival.

## Dataset
The dataset, sourced from Kaggle, comprises 891 records, each representing a Titanic passenger. It includes various attributes such as:
- Passenger ID
- Survival Status (Survived)
- Passenger Class (Pclass)
- Name, Sex, Age
- Number of Siblings/Spouses Aboard (SibSp)
- Number of Parents/Children Aboard (Parch)
- Ticket Number, Fare Paid
- Cabin Number
- Port of Embarkation (Embarked)

## Dataset Preparation
### Data Pre-Processing
- **Handling Missing Values**: Null values in 'Age', 'Cabin', and 'Embarked' were handled using the median and mode to prepare the data for analysis.

### Data Transformation
- **Encoding Categorical Variables**: Features like 'Sex' and 'Embarked' were transformed into numeric formats to facilitate the use of the Random Forest classification model.

## Visualization
Utilizing Python libraries, matplotlib and seaborn, we created scatter plots, bar charts, and histograms to display the distribution of critical variables and their correlations effectively. The visualizations include:
- Kernel Density Estimate (KDE) plots for smooth distribution estimations
- Histograms and bar charts showcasing the distribution of age, fare, passenger class, and survival counts

## Machine Learning Model
### Random Forest Classifier
This model is known for its high accuracy and flexibility. It constructs several decision trees during training and outputs the class that is the mode of the classes of the individual trees. It was trained to predict passenger survival based on features like class, age, sex, fare, cabin, among others.

### Training and Testing
- **Data Splitting**: The dataset was divided into training and testing sets to train the model and evaluate its performance on unseen data.

## Findings / Results and Evaluation
- **Model Performance**: Achieved an accuracy of 82.1%.
- **Classification Report**:
  - Precision: 82.8% for class 0, 80.8% for class 1
  - Recall: 87.6% for class 0, 74.3% for class 1
  - F1-score: 85% for class 0, 77.4% for class 1
  - Support: 105 for class 0, 74 for class 1
  - Macro Average: 81.88% Precision, 80.9% Recall, 81.32% F1-score
  - Weighted Average: 82% Precision, Recall, and F1-score

## Conclusion
This project successfully leveraged both visualization and machine learning to analyze the Titanic dataset, providing deep insights into passenger survival rates. The analysis not only enhances our understanding of the Titanic disaster but also highlights the importance of data-driven historical studies.
