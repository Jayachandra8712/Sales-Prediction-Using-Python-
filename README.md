# Sales Prediction Using Python 📊

##  Project Overview

This project uses machine learning to predict product sales based on advertising expenditure across three media channels: TV, Radio, and Newspaper.

The goal is to analyze the relationship between advertising spending and sales, build regression models, and identify which advertising channel is most important for sales prediction.

##  Objectives

* Analyze advertising expenditure and sales data.
* Perform exploratory data analysis (EDA).
* Visualize relationships between advertising channels and sales.
* Build and compare regression models.
* Evaluate model performance using MAE, RMSE, and R² score.
* Identify important advertising channels using feature importance.

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

##  Dataset

The project uses the classic Advertising dataset containing the following features:

| Feature   | Description                          |
| --------- | ------------------------------------ |
| TV        | Advertising expenditure on TV        |
| Radio     | Advertising expenditure on Radio     |
| Newspaper | Advertising expenditure on Newspaper |
| Sales     | Product sales (target variable)      |

##  Project Workflow

1. Loaded and inspected the dataset.
2. Checked missing values and descriptive statistics.
3. Performed exploratory data analysis.
4. Created a pairplot and scatter plots.
5. Generated a correlation heatmap.
6. Split the dataset into training and testing sets (80:20).
7. Trained Linear Regression and Random Forest Regressor models.
8. Evaluated both models using regression metrics.
9. Analyzed residuals and feature importance.

##  Machine Learning Models

### 1. Linear Regression

Used as the baseline model to predict sales from advertising expenditure.

### 2. Random Forest Regressor

Used as a second model to capture potentially nonlinear relationships and compare prediction performance.

##  Model Evaluation

The models were evaluated on the test dataset.

| Metric   | Linear Regression | Random Forest |
| -------- | ----------------: | ------------: |
| MAE      |            1.4608 |        0.6201 |
| RMSE     |            1.7816 |        0.7686 |
| R² Score |            0.8994 |        0.9813 |

**Best-performing model:** Random Forest Regressor

The Random Forest model achieved an R² score of approximately 98.13% on the test set and lower MAE and RMSE than Linear Regression.

## 📊 Feature Importance

The Random Forest model produced the following feature-importance scores:

| Advertising Channel | Importance |
| ------------------- | ---------: |
| TV                  |     62.48% |
| Radio               |     36.22% |
| Newspaper           |      1.30% |

TV advertising had the highest feature importance, followed by Radio and Newspaper.

These values indicate relative importance within this model; they do not prove that a channel directly causes an increase in sales.

## 📉 Visualizations

The notebook includes:

* Pairplot of dataset features
* Sales vs. TV advertising scatter plot
* Sales vs. Radio advertising scatter plot
* Sales vs. Newspaper advertising scatter plot
* Correlation heatmap
* Residual plot for the selected model
* Feature-importance bar chart

## 🚀 How to Run This Project

1. Clone or download this repository.

2. Ensure Python and Jupyter Notebook are installed.

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Place the dataset file in the project directory.

5. Open `Sales_Prediction.ipynb` in Jupyter Notebook.

6. Run the notebook cells in order.

## 💡 Key Learnings

* Performing exploratory data analysis on advertising data.
* Understanding relationships between advertising expenditure and sales.
* Building regression models using scikit-learn.
* Evaluating models with MAE, RMSE, and R² score.
* Interpreting residual plots and feature importance.
* Comparing baseline and ensemble regression models.

## 🏁 Conclusion

This project demonstrates how machine learning can be applied to sales prediction using advertising data.

Random Forest Regressor performed better than Linear Regression on the selected test split. Feature-importance analysis identified TV as the most important predictor, followed by Radio and Newspaper.

Model performance may vary with different data splits or new datasets. Further validation would help assess how well the model generalizes to unseen data.

## 👨‍💻 Author

**Jayachandra Abbannagari**

Aspiring Data Scientist interested in Python, SQL, Machine Learning, and Data Analytics.

## 📄 License

This project is intended for educational and learning purposes. Refer to the dataset provider's license and terms when redistributing the dataset.
