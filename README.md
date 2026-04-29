Group Project
Project creation date: 04/05/26

Overview
Group Project is a data science notebook project about how everyday habits relate to sleep duration. We use a sleep time prediction dataset from Kaggle and look at variables like workout time, reading time, phone time, work hours, caffeine intake, and relaxation time.

The project starts with data loading and visual analysis, then uses a simple KNN regression model to predict sleep time. The goal is to keep the work clear and connected to what we learned in an intro DSCI course.

Background and Motivation
Sleep matters a lot for student health and school performance, but daily routines can make it hard to get enough rest. Things like work hours, phone time, caffeine, exercise, and relaxation may all connect to how much someone sleeps.

This project uses the dataset to practice these skills:

1. Loading and checking tabular data with pandas.
2. Making visualizations with Altair.
3. Looking at correlations between lifestyle variables and sleep duration.
4. Building a KNN regression model with scaled predictors.
5. Checking prediction error on test data.

Dataset
The dataset has 2,000 observations with seven numerical columns.

WorkoutTime: Time spent working out
ReadingTime: Time spent reading
PhoneTime: Time spent on the phone
WorkHours: Number of hours worked
CaffeineIntake: Daily caffeine intake
RelaxationTime: Time spent relaxing
SleepTime: Total sleep duration

The data was obtained from Kaggle:
https://www.kaggle.com/datasets/govindaramsriram/sleep-time-prediction/data

Analysis and Modeling
The main notebook is `Project/Group Project/sleep_data.ipynb`.

The completed workflow includes:

1. Loading the sleep time prediction dataset from the data folder.
2. Previewing the dataset and checking the lifestyle variables.
3. Using a correlation heatmap to compare each variable with `SleepTime`.
4. Splitting the data into training and test sets.
5. Building a KNN regression model with scaling.
6. Tuning `k` with cross validation.
7. Evaluating prediction error with RMSPE on test data.

The main research questions are:

1. Which daily lifestyle habits have the strongest relationship with sleep duration?
2. Can these daily lifestyle habits predict sleep duration reasonably well?

Requirements
Python 3.8 or newer
pandas
altair
jupyter or jupyterlab
scikit learn

Install the dependencies with pip:

```bash
pip install pandas altair jupyter scikit-learn
```

Or with conda:

```bash
conda install pandas altair jupyter scikit-learn
```

How to Run
Open the repository in VS Code or navigate to the project folder.

Launch Jupyter:

```bash
jupyter notebook
# or
jupyter lab
```

Open `Project/Group Project/sleep_data.ipynb` and run the notebook cells in order.

The notebook loads the dataset from the data folder, shows the lifestyle variables, makes a correlation heatmap, trains the KNN regression model, and reports test set RMSPE.

Key Takeaway
This project uses exploratory analysis and KNN regression to study how common lifestyle habits relate to sleep duration. Phone time and work hours show the strongest negative relationships with sleep duration in the dataset. The final model predicts sleep duration better than a simple average sleep baseline, but the remaining error shows that sleep is influenced by several factors and cannot be predicted perfectly from these lifestyle variables alone.

License
This project is intended for educational use in a data science course.
