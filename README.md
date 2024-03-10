# CaroPeThesis
This repository is for me to store everything related to my Bachelor's thesis and keep a journal of what I am doing

# Journal
- Notes from email:
  -  First steps can be: 
  - Take one or two datasets  and upload the data in a Jupyter Notebook. 
  - Do a first visualization looking at the time and the number of bicycles on a day / per hour.
  - Think of data model (table) to store the data from different cities. 
- Jupyter Notebook was installed
- Jupyter Notebook created
- Downloaded different data sets
- Checking df.info() for each data set
- ! Interesting to read: https://www.wiwi.uni-muenster.de/ivm/sites/ivm/files/documents/forschung/diskussionspapiere/workingpaper33v2.pdf :
  - Cools et al. (2010) or Zhao et al. (2019) have shown that the trip type influences the response to adverse weather conditions, we minimize the bias that
- https://opendata.duesseldorf.de/dataset/jahresübersicht-der-dauerzählstellen-radverkehr-seit-2012

## Data Set Shapes - Preprocessing Stage
- ### Würzburg:
  - Rows: 231349
  - Total Columns: 15
  -    Column             Non-Null Count   Dtype  
  - 0   Id                 231349 non-null  int64
  - 1   Date               231349 non-null  object
  - 2   Counts             153916 non-null  float64
  - 3   Status             153916 non-null  object
  - 4   Name               217150 non-null  object
  - 5   Coordinates        217150 non-null  object
  - 6   User Type          217150 non-null  object
  - 7   TimeZone           217150 non-null  object
  - 8   Interval           217150 non-null  float64
  - 9   Sens               217150 non-null  object
  - 10  Installation Date  217150 non-null  object
  - 11  Counter            108553 non-null  object
  - 12  Photos             108553 non-null  object
  - 13  photourl           108553 non-null  object
  - 14  photo              108553 non-null  object 

- ### Munich
- ### Augsburg:
  - Rows: 2696 entries, ('Time', 'Dieselbrücke', 'Friedberger Straße östlich Afrabrücke', 'Friedrich-Ebert-Straße östlich Haltestelle Messe', 'Färberstraße/Gollwitzerstr.', 'Gögginger Straße südlich Rosenaustraße', 'Haunstetter Straße Höhe protestantischer Friedhof', 'Konrad Adenauer Allee Fahrradstraße', 'Postillionstraße südl. Roggenstraße', 'Rosenaustraße westlich Gögginger Straße', 'Südlich A8-Unterführung, Ostseite') 
        Column                                             Non-Null Count  Dtype  
     0   Zeitraum                                           2330 non-null   object 
     1   16. September 2016 00:00 -> 1. Februar 2024 08:30  2253 non-null   object 

- ### Stuttgart
- ### Berlin
- ### Köln

# Interesting Information To Check
## Yunex Traffic

Operide: Bike Sharing System

Bike sharing is the trend – but how can demand and supply be matched better and how can the bikes be protected from damage and loss? Traffic planners can now use our fleet management software Operide for this purpose. Operide’s AI algorithm uses historical trip and weather data to predict the demand for e-bikes or e-scooters at each station. The predictions then feed into a recommendations algorithm which looks at the current traffic situation to allow service providers to distribute bikes and scooters according to demand and improve maintenance efficiency.

# Some intro
Investigating bicycle traffic dynamics in urban environments, particularly in cities like Munich and Freiburg, offers a valuable opportunity to understand the complexities of sustainable transportation systems. The choice of these cities for our study is rooted in several factors:

- Bicycle-Friendly Infrastructure: Both Munich and Freiburg boast extensive networks of bike paths, lanes, and cycling-friendly infrastructure. This facilitates the smooth movement of cyclists and encourages active transportation.
- High Bicycle Utilization: These cities have a significant proportion of residents who use bicycles as a primary mode of transportation for daily commuting, recreational activities, and running errands. This high level of bicycle utilization reflects the cities' commitment to promoting sustainable transportation alternatives.
- Diverse Urban Environments: Munich and Freiburg represent diverse urban environments, with varying population densities, land use patterns, and urban layouts. Studying bicycle traffic in these cities allows us to explore how different urban contexts influence cycling behavior and traffic flow dynamics.
- Research Significance: By focusing on these cities, our study aims to provide valuable insights into the operational characteristics of bicycle traffic in urban settings. Understanding the factors that affect cycling patterns, such as infrastructure design, topography, weather conditions, and socio-cultural factors, is crucial for urban planners, policymakers, and transportation engineers seeking to enhance bicycle mobility and promote sustainable urban development.

Overall, our research endeavors to contribute to the growing body of knowledge on urban cycling by analyzing bicycle traffic data collected in Munich and Freiburg. By examining patterns, trends, and challenges related to bicycle traffic in these cities, we aim to inform evidence-based policy decisions and urban planning strategies aimed at creating more bike-friendly cities and fostering sustainable transportation systems.

## About the Sensors
These permanent monitoring stations, primarily installed for urban planning purposes, employ ground-based sensors to monitor the flow of bicycle traffic. These sensors operate continuously throughout the year, recording the passage of bicycles exclusively within designated bike lanes. Cyclists utilizing sidewalks are also detected by the sensors, although their data is not integrated into the overall count. Notably, near the Deutsches Museum, there is a publicly accessible display showcasing the daily and yearly influx of cyclists at that specific location. (Citation: https://stadt.muenchen.de/dam/jcr:9a65625e-952f-470f-b6a1-d4270f4526cb/mb190304.pdf)

## Machine Learning Models
### Bikes - Day of the year
Several machine learning models can be suitable for predicting bike counts based on historical data from previous years. Some of the commonly used models for such time-series prediction tasks include:

1. **Autoregressive Integrated Moving Average (ARIMA)**: ARIMA models are well-suited for time series data with trend and seasonality. They incorporate parameters to model auto-correlation, differencing, and moving averages.

2. **Seasonal Autoregressive Integrated Moving-Average (SARIMA)**: SARIMA extends ARIMA by incorporating seasonal components. It's useful when there are repeating patterns or seasonal trends in the data.

3. **Seasonal Decomposition of Time Series (STL)**: STL decomposes time series into trend, seasonality, and remainder components, making it easier to model and predict each component separately.

4. **Prophet**: Prophet is an open-source forecasting tool developed by Facebook. It handles daily, weekly, and yearly seasonality, as well as holiday effects, with flexibility and ease of use.

5. **Long Short-Term Memory (LSTM) networks**: LSTM networks, a type of recurrent neural network (RNN), are effective for capturing complex temporal dependencies. They excel at handling sequential data and can learn patterns over long sequences, making them suitable for time series forecasting.

6. **Gradient Boosting Machines (GBM)**: GBM models, such as XGBoost, LightGBM, and CatBoost, are powerful ensemble learning methods that can handle non-linear relationships and interactions between features. They perform well with large datasets and can capture complex patterns in the data.

7. **Random Forests**: Random Forests are another ensemble learning technique that works well for regression tasks. They are robust to overfitting and can handle both numerical and categorical features effectively.

8. **Gated Recurrent Units (GRU)**: GRU networks, similar to LSTM networks, are designed to capture long-term dependencies in sequential data. They are computationally more efficient than LSTM networks while achieving comparable performance.

The choice of model depends on various factors such as the size of the dataset, the presence of seasonality and trends, computational resources, and the interpretability of results. It's often a good practice to experiment with multiple models and select the one that performs best according to specific evaluation metrics and requirements.