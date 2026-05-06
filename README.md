# Student Performance Regression Analysis

## Project Overview

This project uses a Student Performance Dataset from Kaggle to analyze the factors that influence academic performance and to predict the student's **Performance Index** using regression.

The project includes data preprocessing, encoding, missing value handling, correlation analysis, outlier checking, model training, and prediction comparison.

## Dataset

The dataset was obtained from Kaggle:

[Student Performance - Multiple Linear Regression Dataset](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)

The dataset contains **10,000 student records** and is synthetic, meaning it was created for illustrative and educational purposes.

## Features

- **Hours Studied**: Total number of hours spent studying by the student.
- **Previous Scores**: Scores obtained by the student in previous tests.
- **Extracurricular Activities**: Whether the student participates in extracurricular activities.
- **Sleep Hours**: Average number of hours of sleep per day.
- **Sample Question Papers Practiced**: Number of sample question papers practiced by the student.

## Target Variable

- **Performance Index**: A score representing the overall academic performance of the student.

The Performance Index ranges from **10 to 100**, where higher values indicate better performance.

## Preprocessing

The following preprocessing steps were applied:

- The dataset was split into independent variables `X` and target variable `y`.
- The **Extracurricular Activities** column was encoded:
  - `Yes` → `1`
  - `No` → `0`
- Missing values were handled using `SimpleImputer`.
- Correlation between features and the target variable was checked.
- Outliers were checked using boxplots.

## Visualization

The relationship between features and the target variable was analyzed using:

- Correlation values
- Correlation bar plot
- Boxplots for outlier detection

## Model

A regression model was trained to predict the **Performance Index**.

After training, predictions were made on the test set and compared with the actual values.

Example output:

| Predicted | Actual |
|----------:|-------:|
| 50.45 | 53.00 |
| 53.09 | 50.00 |
| 78.25 | 80.00 |

## Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Conclusion

The project shows how student-related features can be used to predict academic performance. Correlation analysis helped identify which features were more strongly related to the **Performance Index**, and the regression model was used to estimate student performance based on the selected predictors.

Since the dataset is synthetic, the results should be interpreted as an educational machine learning example rather than a real-world academic performance study.

## License

The dataset is stated to be free to share and use by the original Kaggle dataset provider.
