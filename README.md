Group Project
Project creation date: 04/05/26

Overview
Group Project is a data science notebook project focused on exploring how everyday lifestyle habits relate to sleep duration. Using a sleep-time prediction dataset from Kaggle, the project examines whether variables such as workout time, reading time, phone time, work hours, caffeine intake, and relaxation time show clear relationships with total sleep time.

The project is designed as an introductory exploratory analysis and supervised regression workflow. It combines data loading, visual analysis, correlation-based exploration, K-nearest neighbors regression, and test-set model evaluation using sleep duration as the target variable.

Background & Motivation
Sleep is a major part of student health and academic performance, but daily routines often affect how much rest people actually get. Study time, work hours, caffeine consumption, exercise, and screen time can all influence sleep in different ways. This project uses a structured dataset to investigate those patterns and identify which habits appear most strongly associated with sleep duration.

This project uses the dataset as a practical setting to:

Practice loading and inspecting tabular data with pandas.
Build repeated scatter plots and other visualizations with Altair.
Explore relationships between lifestyle variables and sleep duration.
Prepare the data for correlation analysis and KNN regression.
Evaluate prediction error on held-out test data.

Dataset

It contains 2,000 observations with seven numerical columns:

Column | Description
--- | ---
WorkoutTime | Time spent working out
ReadingTime | Time spent reading
PhoneTime | Time spent on the phone
WorkHours | Number of hours worked
CaffeineIntake | Daily caffeine intake
RelaxationTime | Time spent relaxing
SleepTime | Total sleep duration

The data was obtained from Kaggle:
https://www.kaggle.com/datasets/govindaramsriram/sleep-time-prediction/data

Analysis & Modeling
The main notebook, sleep_data.ipynb, completes the following workflow:

Loading the sleep-time prediction dataset from the data folder.
Previewing the dataset and separating lifestyle variables from the sleep-duration target.
Using a correlation heatmap to compare lifestyle variables with SleepTime.
Interpreting which habits are most strongly associated with sleep duration.
Splitting the data into training and testing sets.
Training and tuning a scaled KNN regression model.
Evaluating prediction error with RMSPE on held-out test data.

The main research questions guiding the notebook are:

- Which daily lifestyle habits have the strongest relationship with sleep duration?
- Which daily lifestyle habits best predict sleep duration?

Requirements
Package | Purpose
--- | ---
Python >= 3.8 | Runtime
pandas | Data loading and wrangling
altair | Declarative visualization
jupyter / jupyterlab | Running the notebook
scikit-learn | Regression modeling support

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

Open Project/Group Project/sleep_data.ipynb and run the notebook cells in order.

The notebook loads the dataset from the data folder, displays the lifestyle variables, and generates repeated Altair plots comparing each habit against SleepTime.

Key Takeaway

This project uses exploratory analysis and KNN regression to study how common lifestyle habits relate to sleep duration. Phone time and work hours show the strongest negative relationships with sleep duration in the dataset. The final model predicts sleep duration better than a simple average-sleep baseline, but the remaining error shows that sleep is influenced by several factors and cannot be predicted perfectly from these lifestyle variables alone.

License

This project is intended for educational use in a data science course.
