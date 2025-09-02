 **Hotel Booking Cancellation Prediction**

A small machine learning project to predict whether a hotel booking will be canceled or not.

 **Project Overview**
The goal of this project is to help hotels identify bookings that are likely to be canceled. By predicting cancellations, hotels can optimize room allocation, reduce revenue loss, and improve overall planning.

**Dataset**
The dataset contains historical hotel booking information including:

- Booking details (e.g., hotel type, lead time, arrival date)
- Customer information (e.g., number of adults, children, babies)
- Booking changes and previous cancellations
- Deposit type and customer type
- Special requests and other relevant features



## Features Used
- `lead_time`
- `arrival_date`
- `adults`, `children`, `babies`
- `previous_cancellations`
- `booking_changes`
- `deposit_type`
- `customer_type`
- `market_segment`, `distribution_channel`
- Special requests

## Model
 **Algorithms Used:** Logistic Regression, Decision Tree, Random Forest, XGBoost  
 **Evaluation Metrics:** Accuracy, Classification Report  
 **Best Model:** Random Forest (after tuning)  



## Model Performance

The following table shows the accuracy of different machine learning models **before and after hyperparameter tuning** for predicting hotel booking cancellations:

| Model                | Train Acc Before | Test Acc Before | Status Before | Train Acc After | Test Acc After | Status After  |
|----------------------|-----------------|----------------|---------------|----------------|----------------|---------------|
| Logistic Regression  | 0.808           | 0.805          | Good Fit      | 0.808           | 0.805          | Good Fit      |
| Decision Tree        | 0.923           | 0.811          | Overfitting   | 0.851           | 0.822          | Good Fit      |
| Random Forest        | 0.923           | 0.820          | Overfitting   | 0.871           | 0.830          | Good Fit      |
| XGBoost              | 0.837           | 0.829          | Good Fit      | 0.838           | 0.828          | Good Fit      |

 After tuning, **Random Forest** gave the best test accuracy (0.830) and was selected as the final model for this project.



## How to Run
1. Clone the repository:

```bash
git clone https://github.com/Tejasri-2005/Hotel-Booking-Cancellation-Prediction-Project-.git
