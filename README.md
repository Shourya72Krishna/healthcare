# Healthcare Data Cleaning and BMI Analysis

## Overview
This project involves cleaning a healthcare dataset, calculating **Body Mass Index (BMI)** for each patient, and categorizing them into different **BMI categories** (Underweight, Normal weight, Overweight, Obese). The dataset includes important features like **Age**, **Blood Pressure**, **Sugar Level**, and **Weight**. After the data cleaning and calculations, a **bar graph** is created to visualize the distribution of patients across different BMI categories.

## Project Structure
The project contains the following files:

- `healthcare_data.csv`: The raw dataset containing patient data.
- `cleaned_healthcare_data_with_bmi.csv`: The cleaned dataset with BMI and BMI categories added.
- `healthcare_bmi_analysis.ipynb`: The Jupyter Notebook containing the code for data cleaning, BMI calculation, categorization, and visualization.
- `README.md`: This file, providing a description of the project.

## Steps in the Project

1. **Data Cleaning**:  
   - Missing values are filled with the median of the respective columns.
   - Duplicate rows are removed.
   - Outliers (like age > 100) are removed.

2. **BMI Calculation**:  
   The **Body Mass Index (BMI)** is calculated using the formula:  
   \[
   BMI = \frac{\text{Weight (kg)}}{(\text{Height (m)})^2}
   \]  
   Here, an assumed **average height** of **1.7 meters** is used.

3. **BMI Categorization**:  
   Patients are categorized into the following BMI groups:  
   - **Underweight**: BMI < 18.5  
   - **Normal weight**: 18.5 ≤ BMI < 24.9  
   - **Overweight**: 25 ≤ BMI < 29.9  
   - **Obese**: BMI ≥ 30

4. **Data Visualization**:  
   A **bar graph** is generated to show the distribution of patients in each BMI category.

## Requirements

- **Python 3.x**
- **Libraries**: 
  - `pandas`
  - `matplotlib`
  - `seaborn`
  
  You can install the required libraries using `pip`:
  ```bash
  pip install pandas matplotlib seaborn
