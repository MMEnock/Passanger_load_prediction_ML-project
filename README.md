# Plane Passenger Load Ratio Prediction

This machine learning project aims to predict the passenger load ratio (PAr) of a plane. The goal is to develop a model that accurately forecasts this ratio based on a variety of features related to the flight, temporal information, and other contextual data. The output of the model, the PAr, helps airlines optimize their operations by anticipating the load factor of their flights.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Features](#features)
4. [Project Structure](#project-structure)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Model Used](#model-used)
8. [Evaluation](#evaluation)
9. [Results](#results)
10. [Conclusion](#conclusion)
11. [Contributing](#contributing)
12. [License](#license)

## Introduction
This project aims to predict the passenger load ratio (PAr) using the Random Forest Regressor. The model analyzes various features such as flight details, temporal information, and contextual data to make predictions.

## Dataset
The dataset includes information about flights, such as dates, times, passenger numbers, and other related features.

## Features
The dataset includes the following features:
- **Day of week:** The day of the week when the flight occurs (e.g., Monday, Tuesday).
- **Weekend (0/1):** A binary feature indicating if the flight is on a weekend (1) or not (0).
- **Holiday (0/1):** A binary feature indicating if the flight day is a holiday (1) or not (0).
- **Festival:** Indicates whether the flight day coincides with a festival.
- **Overlap with Weekend:** Indicates if the flight overlaps with a weekend.
- **Extended weekend:** Indicates if the flight is part of an extended weekend period.
- **1day_after:** Indicates the day after a significant event or holiday.
- **2day_after:** Indicates two days after a significant event or holiday.
- **3day_after:** Indicates three days after a significant event or holiday.
- **1day_before:** Indicates the day before a significant event or holiday.
- **2day_before:** Indicates two days before a significant event or holiday.
- **3day_before:** Indicates three days before a significant event or holiday.
- **4day_before:** Indicates four days before a significant event or holiday.
- **4day_after:** Indicates four days after a significant event or holiday.
- **Boarded pax:** Number of passengers who boarded the plane.
- **Original Airport:** The airport from which the flight originated.
- **Arrival Datetime:** The date and time of the flight's arrival.
- **Seat Capacity:** The seating capacity of the plane.
- **Traffic_type:** The type of traffic (e.g., domestic, international).
- **Terminal:** The terminal from which the flight departs.
- **Airline Code:** The code of the airline operating the flight.
- **PAr:** Passenger load ratio, which is the target variable.
- **Month:** The month of the year when the flight occurs.
- **WN:** Indicates whether the flight is operated by Southwest Airlines.
- **Year:** The year when the flight occurs.

## Project Structure
The project directory is structured as follows:
- `data/`: Contains the dataset files
- `notebooks/`: Jupyter notebooks for different stages of the project:
  - `1_Cleaning.ipynb`: Data cleaning
  - `2_Data_Preparation_and_Exploration.ipynb`: Data preparation and exploration
  - `3_Machine_Learning_Script.ipynb`: Machine learning model implementation
- `src/`: Source code for data processing, feature engineering, and model implementation
- `models/`: Saved models
- `results/`: Evaluation results and visualizations
- `README.md`: Project documentation

## Installation
To run this project, you need Python 3.x and the following libraries:
- numpy
- pandas
- matplotlib
- seaborn
- dateutil
- datetime
- re
- plotly
- scikit-learn

You can install the required libraries using pip:
```bash
pip install numpy pandas matplotlib seaborn python-dateutil scikit-learn plotly
```

## Usage
1. Clone the repository:
```bash
git clone https://github.com/yourusername/plane-passenger-load-ratio-prediction.git
cd plane-passenger-load-ratio-prediction
```

2. Navigate to the `notebooks/` directory and open the Jupyter notebooks to explore data cleaning, preparation, exploration, and model training:
```bash
jupyter notebook
```

3. Run the scripts in the `src/` directory to preprocess data, train models, and evaluate results.

## Model Used
The primary model used in this project is the **Random Forest Regressor**, which is effective for handling complex datasets and capturing non-linear relationships.

## Evaluation
The model was evaluated using the following metrics:
- R2 Score
- Mean Absolute Error (MAE)

## Results
The Random Forest Regressor achieved an R2 score of XX and a mean absolute error of XX on the test set. Detailed results and evaluation metrics can be found in the `results/` directory.

## Conclusion
This project aims to accurately predict the passenger load ratio (PAr) using a variety of features. By utilizing machine learning models, the project can help optimize airline operations and improve decision-making based on predicted load factors.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to modify the above README file as per your specific project details and requirements.


