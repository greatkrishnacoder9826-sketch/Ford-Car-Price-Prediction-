Ford Car Price Prediction
Project Overview
This project analyzes a dataset of used Ford cars to predict their prices using machine learning techniques. The dataset contains information about various Ford models, including their specifications and market prices.

Dataset Information
Source: Ford car dataset

Size: 17,966 rows × 9 columns

Features:

model: Car model (Fiesta, Focus, Kuga, etc.)

year: Manufacturing year

price: Target variable (car price)

transmission: Manual/Automatic/Semi-Auto

mileage: Miles driven

fuelType: Petrol/Diesel/Hybrid/Electric

tax: Road tax

mpg: Miles per gallon

engineSize: Engine displacement (L)

Key Findings from EDA
Data Distribution
Most common models: Fiesta (~6,557), Focus (~4,588), Kuga (~2,225)

Fuel type distribution: Petrol (12,179), Diesel (5,762), Hybrid (22), Electric (2)

Price range: £495 - £54,995

Correlations
Feature	Correlation with Price
year	+0.636
engineSize	+0.411
tax	+0.407
mpg	-0.346
mileage	-0.531
Visual Insights
Price Distribution: Right-skewed, most cars priced between £8,000-£15,000

Price vs Year: Newer cars generally command higher prices

Price vs Mileage: Strong inverse relationship

Price vs Engine Size: Larger engines tend to cost more

Transmission: Automatic cars show higher price variance

Fuel Type: Diesel vehicles generally priced higher than petrol

Model Performance
Preprocessing
One-hot encoding for categorical variables (model, transmission, fuelType)

Train-test split: 67% train / 33% test

Model: Linear Regression
Performance Metrics:

R² Score: 0.848

Feature Engineering
The final model uses 34 features after one-hot encoding, including:

Numerical features (standardized)

Binary indicators for each car model

Transmission type indicators

Fuel type indicators

How to Use
Prerequisites
bash
pip install pandas numpy matplotlib seaborn scikit-learn
Run the Analysis
Load the Jupyter notebook ford.ipynb

Ensure the dataset ford.csv is in the correct path

Run cells sequentially to reproduce the analysis

Future Improvements
Try ensemble methods (Random Forest, XGBoost) for potentially better performance

Feature selection to reduce dimensionality

Hyperparameter tuning for improved accuracy

Handle outliers in price and mileage more robustly

Technologies Used
Python 3.13

Pandas & NumPy (Data manipulation)

Matplotlib & Seaborn (Visualization)

Scikit-learn (Machine Learning)

Author
[Krishna Great]

License
This project is open source and available for educational purposes.
