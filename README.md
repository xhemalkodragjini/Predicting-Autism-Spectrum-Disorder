# Predicting Autism Spectrum Disorder

This repository contains the code and data used to create a ML model for predicting Autism Spectrum Disorder. The model is implemented as part of my diploma thesis, titled "Predicting Autism Spectrum Disorder (ASD) with Machine Learning Classification Algorithms".

#### Data
The dataset was accessed through the UCI Machine Learning Repository and was originally created by Dr. Fadi Thabtah. He developed a mobile application where parents or caregivers could take several screening tests for toddlers (children of age 12-36 months old), among which was the famous AQ-10 Test. The dataset that will be used to create our model contains results from this test, and some other features, such as age of the child, gender, etc.

Features:

Q1-Q10                     -->  Answers to the questions of AQ-10 Test (0 or 1)
Age                        -->  Age of the participant/child (0-36 months old)
Gender                     -->  Gender (m- male, f- female)
Ethnicity                  -->  Ethnic group to which the participant/child belongs (White European, Asian, etc.)
Born with Jaundice         -->  Whether the child was born with Jaundice or not (Yes, No)
Family Member with ASD     -->  Whether any family member is diagnosed with ASD (Yes, No)


### Data Cleaning and Preprocessing
- The dataset did not contain any missing value.
- Three columns were removed since the information that they contain does not impact the results: the number of the case, who completed the test, and the total score in the test.
- Categorical values were preset, thus I had to convert them into numerical. I used lambda function for data that contained two labels (Male/Female or Yes/No) where the first label was converted to 0 and the second to 1. Also, Label Encoder was used for the Ethnicity feature values.
