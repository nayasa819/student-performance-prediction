Student Performance Index Prediction System
Course: B.Sc. (Hons.) Data Science — Semester I (AML002)
Domain: Education
Category: Data Science Capstone Project

1. About the Project
This project investigates how key academic and lifestyle factors relate to student academic performance and builds a supervised machine learning model to predict a student's overall Performance Index. Using a synthetic dataset of 10,000 student records (Student_Performance.csv), the analysis follows a structured 5-phase data science workflow: problem definition, data understanding, data preparation and exploration, predictive modelling, and evaluation.

2. Objective
=>Inspect, clean, and preprocess the 10,000-record dataset for duplicate entries and categorical encoding.
=>Explore the distribution of the Performance Index and measure linear correlations across student attributes.
=>Build and train a Multiple Linear Regression model to predict the Performance Index from behavioral and academic predictors.
=>Evaluate predictive accuracy using $R^2$, Mean Squared Error (MSE), and Mean Absolute Error (MAE).

3. Tools & Technologies Used
=>Python 3
=>pandas & NumPy (Data loading, duplicate removal, categorical encoding, and summary statistics)
=>Matplotlib & Seaborn (Distribution histograms, correlation heatmaps, and prediction scatter plots)
=>scikit-learn (Train-test splitting, Linear Regression modelling, and evaluation metrics)
=>Google Colab / Jupyter Notebook

4. Steps Performed
1)Data Acquisition: Loaded Student_Performance.csv (10,000 rows across 6 columns) using pandas.
2)Data Cleaning & Preprocessing: Verified zero missing values, removed 13 exact duplicate rows (retaining 9,987 clean records), and binary-encoded Extracurricular Activities (Yes = 1, No = 0).
3)Exploratory Data Analysis (EDA): Visualized the bell-shaped target distribution and generated a correlation matrix heatmap across all features.
4)Model Training: Split the data into an 80% training set and 20% testing set (random_state=42) and trained a Multiple Linear Regression model.
5)Model Evaluation: Measured test set error metrics and plotted Actual vs. Predicted Performance Index values.

5. Key Findings
=>Strongest Predictors: Previous Scores ($r = 0.92$) and Hours Studied ($r = 0.37$) have the strongest positive linear relationships with a student's Performance Index.
=>Model Performance: Evaluated on the unseen 20% test set, the Multiple Linear Regression model achieved:
     ->R^2$ Score: 0.9893 (explaining 98.93% of variance in the dataset)
     ->Mean Squared Error (MSE): 3.94
     ->Mean Absolute Error (MAE): 1.58 points
=>Regression Impact: Each additional daily study hour adds ~2.86 points, while each additional prior score point adds ~1.02 points.

6. Conclusion & Limitations
=>Conclusion: Supervised linear regression effectively captures the relationship between study habits, prior preparation, and academic performance within this dataset.
=>Limitations: The dataset is synthetic (computer-generated for academic demonstration) and does not capture unmeasured real-world factors such as teaching quality, classroom attendance, or exam stress.

7. Dataset Source & Repository Structure
=>Dataset: Student_Performance.csv — Synthetic educational dataset (10,000 records, generated with seed 42 for academic demonstration; contains no private or personally identifiable student data).
├── README.md                                        # Project overview, methodology, and findings
├── Nayasa_2601840005_student_performance_c.ipynb    # Executed Google Colab / Jupyter Notebook
├── Student_Performance.csv                          # Input dataset (10,000 student records)
└── project_report.docx











