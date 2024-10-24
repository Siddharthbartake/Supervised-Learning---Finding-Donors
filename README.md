# Finding Donors for CharityML

This project involves building a machine learning model to predict potential donors for CharityML, a fictional non-profit organization. The goal is to improve the process of identifying individuals who are likely to donate, using features from the U.S. Census dataset.

## Project Overview

CharityML is looking for ways to optimize its donation efforts by focusing on individuals who are more likely to donate. In this project, various supervised learning techniques were implemented to analyze the census data and predict whether a person makes over $50,000 per year. The classification model helps target individuals who are likely to be more generous in their donations.

## Dataset

The dataset used for this project is the U.S. Census data, consisting of the following features:

- Age
- Workclass
- Education level
- Marital status
- Occupation
- Relationship
- Race
- Sex
- Capital gain
- Capital loss
- Hours per week
- Native country

The target variable indicates whether the individual's income exceeds $50,000.

## Project Structure

The project follows these main steps:

1. **Exploratory Data Analysis (EDA):** Analysis of the dataset to understand the distribution and relationships among features.
2. **Data Preprocessing:** Handling missing values, encoding categorical variables, scaling numerical features, and splitting the data into training and testing sets.
3. **Model Training and Evaluation:** Training different classification models, including Decision Trees, AdaBoost, Random Forest, and Logistic Regression, and evaluating their performance using accuracy and F-scores.
4. **Model Tuning:** Using Grid Search to optimize the hyperparameters of the best-performing model.
5. **Feature Importance Analysis:** Identifying the most important features that influence the model's predictions.
6. **Model Evaluation on Reduced Data:** Training the model on a reduced set of features to compare the performance with the full feature set.

## Key Findings

- The best-performing model was found to be an AdaBoost classifier with tuned hyperparameters.
- The final model's accuracy on the test data was significantly better than a naive predictor's baseline.
- Training on reduced features resulted in only a slight decrease in accuracy and F-score, indicating that feature selection could help reduce model complexity without significant performance loss.

## Dependencies

The project requires the following Python packages:

- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

You can install the required packages using:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd finding_donors
   ```

3. Open the Jupyter notebook:

   ```bash
   jupyter notebook finding_donors.ipynb
   ```

4. Run the cells in the notebook to see the analysis and results.

## Results and Evaluation

The final model achieved:

- **Accuracy on test data:** Approximately 87%
- **F-score on test data:** Approximately 75%

### Effects of Feature Selection

Training the model on a reduced feature set showed that while accuracy dropped by ~2.7% and the F-score by ~5%, it could be a feasible approach for faster training when handling larger datasets.

## Acknowledgments

The dataset used in this project was provided by the U.S. Census Bureau. This project is inspired by Udacity's Machine Learning Nanodegree program.
```

This `README.md` file covers the main aspects of the project, including setup, results, and instructions for running the code. Let me know if you'd like to customize it further.
