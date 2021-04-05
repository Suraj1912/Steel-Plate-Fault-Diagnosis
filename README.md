# Steel-Plate-Fault-Diagnosis
ML model to classify steel plate faults into seven categories.

## About Dataset ->

Dataset is taken from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Steel+Plates+Faults). The original aim of the research was to correctly classify the type of surface defects in stainless steel plates, with six types of possible defects (plus "other"). The Input vector was made up of 27 indicators that approximately the geometric shape of the defect and its outline.

#### 27 independent variables:

X_Minimum

X_Maximum

Y_Minimum

Y_Maximum

Pixels_Areas

X_Perimeter

Y_Perimeter

Sum_of_Luminosity

Minimum_of_Luminosity

Maximum_of_Luminosity

Length_of_Conveyer

TypeOfSteel_A300

TypeOfSteel_A400

Steel_Plate_Thickness

Edges_Index

Empty_Index

Square_Index

Outside_X_Index

Edges_X_Index

Edges_Y_Index

Outside_Global_Index

LogOfAreas

Log_X_Index

Log_Y_Index

Orientation_Index

Luminosity_Index

SigmoidOfAreas

#### Type of dependent variables (7 Types of Steel Plates Faults):

1.Pastry

2.Z_Scratch

3.K_Scatch

4.Stains

5.Dirtiness

6.Bumps

7.Other_Faults

## Steps to Classify ->

**1. Load Dataset :** dataset was loaded from UCI Machine Learning Repository.

**2. Exploratory Data Analysis :** checked for null values, examined distribution of each attribute, plot histograms, boxplots, scaterplots for looked into outliers if any. Correlation matrix for collinearity check in dataset.

**3. Standardization :** To keep data on same scale we require to standardize the data. By doing this model can efficiently do better job and give higher accuracy for same.

**4. Dimensionality Reduction :** Dataset contains collinear attributes so features reduction technique was used. Principal Component Analysis(PCA) one of the feature extraction method was used in this study.

**5. Model Building :** This study evaluates the performances of four of the popular and effective ml models include Logistic Regression, Support Vector Machines(SVM), K-Nearest Neighbor(KNN), Decision Tree Classifier and Ensemble technique such as Random Forest Classifier.

## Libraries

Python libraries are used
```
1. numpy  # For arrays manipulation
2. Pandas  # For data manipulation
3. Matplotlib # For plots
4. Seaborn  # For plots
5. Scikit-learn  # For python pre-defined libraries
```

## Requirements

To run the this program once need to install required libraries. For that simply run command in terminal
```
pip install -r requirements.txt
```
