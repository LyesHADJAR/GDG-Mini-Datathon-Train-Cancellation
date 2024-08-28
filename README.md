# Overview:

Train operators face significant challenges due to frequent ticket cancellations and no-shows, driven by factors like changing travel plans, scheduling conflicts, and flexible cancellation policies. These disruptions lead to empty seats and financial losses, affecting operational efficiency and revenue management. Predicting these cancellations accurately is crucial for optimizing seat occupancy, managing resources effectively, and ensuring better service for passengers.

# Description : 
In this competition, your task is to analyze a train reservation dataset and build predictive models to forecast cancellations. By understanding booking patterns and customer behaviors, your models will help train operators anticipate no-shows and cancellations, enabling better seat management and resource allocation. Your challenge is to create solutions that can accurately predict these disruptions, minimizing revenue loss and enhancing the overall efficiency of train services.

#Evaluation :
Participants are required to submit a CSV file with two columns: ID and STATUS. The ID column should contain the unique identifiers of each reservation, and the STATUS column should indicate the predicted outcome (0 for no cancellation, 1 for cancellation).

# Evaluation Metric : 

This challenge is a binary classification task evaluated using the **F1 Score**, which balances precision and recall, providing a robust measure of the model’s performance on imbalanced classes. The F1 Score is calculated using the formula:

**F1 Score** = 2 × (Precision × Recall) / (Precision + Recall)

- **Precision**: Measures how many of the predicted cancellations were correct.
- **Recall**: Measures how many of the actual cancellations were correctly predicted.

# Dataset Description :

The dataset contains information about train reservations, including customer details, trip characteristics, and reservation outcomes. Participants are required to analyze this data to predict whether a reservation will be canceled or not. The data includes a mix of categorical and numerical features that describe the booking context, passenger details, and trip specifics.

The dataset is divided into the following files:

**train.csv** - The training set used to build and train the predictive model. It contains reservations along with their cancellation status.
**test.csv** - The test set without the status column, used to evaluate model performance.
**sample_submission.csv** - A sample submission file showing the required format for the output, with *ID* and predicted *STATUS*.

## Column Descriptions

- **ID**: Unique identifier for each reservation.
- **direct_trip**: Indicates whether the trip is direct (Yes/No).
- **number_of_adults**: Number of adults included in the reservation.
- **number_of_children**: Number of children included in the reservation.
- **type_of_meal_plan**: The type of meal plan selected (e.g., plan 1, not selected).
- **people_with_disabilities**: Number of people with disabilities in the reservation.
- **class**: Class of the train ticket (e.g., Type 1).
- **year**: The year of the reservation.
- **month**: The month of the reservation.
- **date**: The specific date of the reservation.
- **repeated_guest**: Indicates if the passenger is a repeated guest (Yes/No).
- **np_cancellations**: Number of past cancellations by the guest.
- **np_not_canceled**: Number of past bookings that were not canceled.
- **price**: The total price of the reservation.
- **status**: The outcome of the reservation (Canceled/Not_Canceled).

