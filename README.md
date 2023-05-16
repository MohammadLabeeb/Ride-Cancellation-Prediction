# Booking Cancellation Prediction

## Objective
The objective of this project is to improve customer service for YourCabs.com, a cab company in Bangalore. The aim is to create a predictive model that can classify new bookings as to whether they will eventually get cancelled due to car unavailability. By identifying potential cancellations in advance, the company can minimize passenger inconvenience and optimize their operations.

## Dataset
The dataset used for this project contains the following features:

- `id`: Booking ID
- `user_id`: Customer ID (based on mobile number)
- `vehicle_model_id`: Vehicle model type
- `package_id`: Type of package (1=4hrs & 40kms, 2=8hrs & 80kms, etc.)
- `travel_type_id`: Type of travel (1=long distance, 2=point to point, etc.)
- `from_area_id`: Unique identifier of the pickup area (applicable for point-to-point travel and packages)
- `to_area_id`: Unique identifier of the drop-off area (applicable for point-to-point travel)
- `from_city_id`: Unique identifier of the pickup city
- `to_city_id`: Unique identifier of the drop-off city (only for intercity)
- `from_date`: Timestamp of the requested trip start
- `to_date`: Timestamp of the trip end
- `online_booking`: Binary flag indicating if the booking was done on the desktop website
- `mobile_site_booking`: Binary flag indicating if the booking was done on the mobile website
- `booking_created`: Timestamp of the booking
- `from_lat`: Latitude of the pickup area
- `from_long`: Longitude of the pickup area
- `to_lat`: Latitude of the drop-off area
- `to_long`: Longitude of the drop-off area
- `Car_Cancellation`: Target variable indicating whether the booking was cancelled (1) or not (0) due to car unavailability

## Project Steps
1. Importing Libraries
2. Data Preprocessing
   - Extracting new features
3. Exploratory Data Analysis (EDA)
4. Checking for Outliers
5. Train Test Split
6. Missing Value Treatment
7. Data Encoding
8. Base Predictive Model
9. Feature Selection
10. Imbalance Treatment
11. Exploring Different ML Algorithms
    - Logistic Regression (with Hyperparameter Tuning)
    - Decision Tree (with Hyperparameter Tuning)
    - K-Nearest Neighbors (KNN)
    - Naive Bayes
    - Support Vector Machines (SVM)
    - Random Forest (with Hyperparameter Tuning)
    - XGBoost (with Hyperparameter Tuning)
12. Model Selection and Evaluation
    - Cross Validation on the Training Set
    - Comparing Metrics of ML Models on the Test Set
    - ROC Curve Analysis
