# EG-GeniusLeague
My solution to the Genius League Data Scientist Internship Takehome Challenge. 

Goal is to predict a player’s rank using the information provided in the dataset like Age, HoursPerWeek, ActionLatency, etc.


## Techniques and Technologies used:

1. Imbalanced-Learn for SMOTE and skewness handling
2. Scipy for Outlier Detection and handling
3. PyCaret, Scikit-Learn, PyTorch for training models
4. Seaborn and Matplotlib for plots and visualizations


## Installation

These instructions assume a working installation of [Anaconda](https://www.anaconda.com/).

```bash
git clone git@github.com:shreayan98c/EG-GeniusLeague.git
cd EG-GeniusLeague
pip install -r requirements.txt
```

Depending on your desired configuration, you may need to install the
[PyTorch](https://pytorch.org/get-started/locally/) package separately. This can be done following
the instructions on the PyTorch website, in an empty conda environment.

## Usage

```bash
jupyter notebook
starcraft.ipynb
```
Run all cells.

## Approach

Approach to solve the problem:
Predicting a player’s rank using the information provided in the dataset:

1. Exploratory Data Analysis (EDA): <br>
Perform an initial exploration of the dataset to understand its structure, features, and relationships. Helps in gaining insights and identifying any data quality issues or missing values. Tasks to perform during EDA: <br>
a. Identify missing values. <br>
b. Generate descriptive statistics of the data. <br>
c. Visualize the distribution of target variable and features using plots (histograms, box plots, etc.) from libraries like matplotlib and seaborn.

2. Data Preprocessing: <br>
a. Handle missing values: Depending on the extent of missing data, we can choose to drop rows or columns with missing values or impute them using techniques like mean, median, or mode. <br>
b. Encode categorical variables: If there are categorical variables in the dataset, encode them using techniques like one-hot encoding or label encoding, depending on the nature of the variables. <br>
c. Detect and handle outliers. <br>
d. Split the data: Divide the dataset into training and testing sets.

3. Feature Selection or Engineering: <br>
Based on the insights gained during EDA, we might need to perform feature selection or engineering to improve the model's performance. This can involve removing irrelevant or highly correlated features, creating new features, or transforming existing ones.

4. Model Training and Evaluation: <br>
a. Experiment with different machine learning algorithms for classification like logistic regression, decision trees, random forest, or support vector machines, since predicting rank is a classification problem. <br>
b. Train the model using the training data. <br>
c. Evaluate the model's performance using appropriate evaluation metrics such as accuracy, precision, recall, and F1 score. Use the testing data for evaluation.

5. Model Improvement and Tuning: <br>
If the model's performance is not satisfactory, try different algorithms or tune hyperparameters to improve it using techniques like grid search or random search.

6. Model Deployment and Communication: <br>
Once we have a satisfactory model, we can deploy it to make predictions on new data. Document our findings, methodology, and evaluation results in a clear and concise manner, suitable for non-technical stakeholders. Communicate the findings to stakeholders using visualizations and data story based explanations that are easily understandable.
