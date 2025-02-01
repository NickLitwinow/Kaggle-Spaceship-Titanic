![download](https://user-images.githubusercontent.com/44932745/209876580-0b54a4b4-a903-4ca1-842a-224dab9bbbb7.png)


# Kaggle Spaceship Titanic

(https://www.kaggle.com/code/nicklitwinow/spaceship-titanic-max-accuracy-0-80102)

This project addresses the Kaggle Spaceship Titanic challenge. A mysterious spacetime anomaly has caused nearly half of the passengers to be transported to an alternate dimension. The objective is to predict which passengers were affected using the available onboard data.

## Project Overview

The challenge involves analyzing passenger data from the Spaceship Titanic, including information such as the passenger's cabin details, age, onboard spending, and more. The project focuses on:
- **Data Preprocessing:** Handling missing values, extracting cabin details (deck, number, side), aggregating onboard expenditures, and categorizing passengers by age groups.
- **Exploratory Data Analysis (EDA):** Visualizing distributions of numerical and categorical features, examining the target variable, and assessing correlations among features.
- **Modeling:** Implementing a LightGBM classifier with stratified K-fold cross-validation to predict the 'Transported' status of passengers. The final model’s predictions are averaged across folds to generate a robust submission.

## Data

The dataset consists of three CSV files:
- **train.csv**: Contains data for approximately 8,700 passengers used to train the model.
- **test.csv**: Contains data for approximately 4,300 passengers for which predictions need to be made.
- **sample_submission.csv**: A template for the final submission.

Key features include:
- **PassengerId:** Unique identifier for each passenger.
- **HomePlanet & Destination:** Origin and destination planets.
- **CryoSleep:** Indicates if a passenger was in cryogenic sleep.
- **Cabin:** Cabin details (which are split into deck, number, and side during preprocessing).
- **Age:** Passenger age.
- **Onboard Services Spending:** Amounts spent on services like RoomService, FoodCourt, ShoppingMall, Spa, and VRDeck.
- **Transported:** The target variable indicating if the passenger was transported to an alternate dimension.
