Motivation behind the Problem:
Diabetes is a global health concern with significant societal and economic implications. Early prediction can identify individuals at risk of developing diabetes and allows for early intervention and lifestyle modifications. Predictive models enable targeted screening and preventive measures for high-risk individuals, leading to more efficient resource allocation in healthcare settings.  It can also inform public health policies and interventions aimed at reducing the prevalence of diabetes and its associated complications on a population level. 

The Approach:
This project explores the application of machine learning techniques to predict the onset of diabetes based on diagnostic data. The dataset contains various medical attributes such as,
•	Pregnancies: Number of times a woman has been pregnant
•	Glucose: Blood glucose level
•	BloodPressure: Blood pressure measurement in mm Hg
•	SkinThickness: Skin thickness (mm)
•	Insulin: Blood insulin level (μU/mL)
•	BMI: Body mass index (calculated from weight and height)
•	DiabetesPedigreeFunction: Function score based on family history of diabetes
•	Age: Patient's age (years)
•	Outcome: Indicates presence of diabetes (1 - Yes, 0 - No)
I employed various supervised machine learning algorithms e.g. KNN, decision tree, random forest, logistic regression etc to develop predictive models. Through rigorous evaluation and comparison of multiple algorithms, I achieved promising results in identifying individuals at risks of developing diabetes. This findings can highlight the potential of machine learning in assisting healthcare professionals in early detection and intervention strategies for diabetes prevention.

Tools and technologies used:
Python: Programming language used for model development, data preprocessing.
Scikit-learn: Machine learning library used for model training, evaluation and prediction.
Pandas: Data manipulation library used for data preprocessing and analysis.
Numpy: Library for numerical computing used for handling arrays and mathematical operations.
Seaborn: For plotting and visualization.
Jupyter Notebook: Coding environment for Python.

Installation and Usage:
Download and unzip the project folder.
Open Jupyter Notebook and run ‘EDA and Model building-diabetes.ipynb’
For any queries, please contact me at sadh8004@gmail.com.

Key Features:
Input Data Collection: The dataset is downloaded from Kaggle.com(Pima Indians Diabetes Database) and then imported to Jupyter Notebook via pandas library using ‘read_csv’ command.
Data Preprocessing: The input data is preprocessed to check for missing values or duplicates. However the data was already clean.
Data Normalization: Normalization using MinMaxScaler and StandardScaler has been done from sklearn library.
Machine Learning Models: Various machine learning algorithms are employed, including decision trees, random forests, KNN, and logistic regression, to build predictive models.
Model Training and Evaluation: The models are trained on historical data and evaluated using appropriate performance metrics to ensure accuracy and reliability.
Prediction of diabetes: Based on the trained models, the system recommends which patients are more likely to have diabetes with ~80% accuracy.

Outlier Treatment: 
The features of the dataset have been checked for outliers using histograms and boxplots and corresponding outlier treatment has been done using IQR method.
Conclusion:
I have applied logistic regression, KNN, decision tree classifier and random forest classification for model building. Also I have done outlier treatment of the dataset to eliminate outliers. However the treatment has procured mixed results and not always have improved the accuracy. In case of logistic regression, KNN and decision tree, the accuracies have decreased after outlier treatment, but for Random forest model it has improved. This can be due to reduced number of training data which can in turn result in poor accuracy.
Also after feature scaling the accuracy has improved for three classes: KNN, Decision tree and Random forest but accuracy has decreased for logistic regression. In general, it is expected that feature scaling enhances the accuracy by standardizing the data.
