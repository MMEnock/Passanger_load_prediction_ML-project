# Passanger_load_prediction_ML-project
## ML Project: Predicting Passenger Load of a Plane

## Project Description
This machine learning project aims to predict the passenger load ratio (PAr) of a plane. The goal is to develop a model that accurately forecasts this ratio based on a variety of features related to the flight, temporal information, and other contextual data. The output of the model, the PAr, helps airlines optimize their operations by anticipating the load factor of their flights. It contains three Jupyter notebooks. **1** is for `´Cleaning`´, **2** is for `´Data preprations and exploration`´ and the **Third**  contains the `´Machine learning script`´.

## Below is a list of features used in the model along with their descriptions:

**Day of week:** The day of the week when the flight occurs (e.g., Monday, Tuesday).

**Weekend (0/1):** A binary feature indicating if the flight is on a weekend (1) or not (0).

**Holiday (0/1):** A binary feature indicating if the flight day is a holiday (1) or not (0).

**Festival:** Indicates whether the flight day coincides with a festival.

**Overlap with Weekend:** Indicates if the flight overlaps with a weekend.

**Extended weekend:** Indicates if the flight is part of an extended weekend period.

**1day_after:** Indicates the day after a significant event or holiday.

**2day_after:** Indicates two days after a significant event or holiday.

**3day_after:** Indicates three days after a significant event or holiday.

**1day_before:** Indicates the day before a significant event or holiday.

**2day_before:** Indicates two days before a significant event or holiday.

**3day_before:** Indicates three days before a significant event or holiday.

**4day_before:** Indicates four days before a significant event or holiday.

**4day_after:** Indicates four days after a significant event or holiday.

**boarded pax:** Number of passengers who boarded the plane.

**Original Airport:** The airport from which the flight originated.

**Arrival Datetime:** The date and time of the flight's arrival.

**Seat Capacity:** The seating capacity of the plane.

**traffic_type:** The type of traffic (e.g., domestic, international).

**Terminal:** The terminal from which the flight departs.

**Airline Code:** The code of the airline operating the flight.

**PAr:** Passenger load ratio, which is the target variable.

**Month:** The month of the year when the flight occurs.

**WN:** Indicates whether the flight is operated by Southwest Airlines.

**Year:** The year when the flight occurs.

## Conclusion
This project aims to accurately predict the passenger load ratio (PAr) using a variety of features. By utilizing machine learning models, the project can help optimize airline operations and improve decision-making based on predicted load factors.

## Libraries Used
```python
# Importing Python Libraries to be used in this project
import numpy as np
import pandas as pd
from matplotlib import pyplot as plt
import seaborn as sns
import dateutil.parser as parser
from datetime import datetime, timedelta
import re  # Importing regular expressions, a powerful language for matching regular expressions
import matplotlib.pyplot as plt
%matplotlib inline
from pandas.tseries.offsets import *
from plotly import tools
from sklearn.model_selection import train_test_split, KFold
from sklearn.metrics import r2_score, mean_absolute_error
from sklearn.linear_model import LinearRegression, Lasso, ElasticNet
from sklearn.neighbors import KNeighborsRegressor
from sklearn.ensemble import RandomForestRegressor
from sklearn.tree import DecisionTreeRegressor
Features
