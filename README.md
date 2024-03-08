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
- ! Interesting to read: https://www.wiwi.uni-muenster.de/ivm/sites/ivm/files/documents/forschung/diskussionspapiere/workingpaper33v2.pdf 

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