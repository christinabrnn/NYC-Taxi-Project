## NYC Taxi Fare Analysis

This project analyzes New York City taxi fare pricing patterns using unsupervised machine learning techniques, including K-Means clustering and association rule mining. The goal is to identify fare discrepancies, assess the impact of congestion pricing, and uncover potential pricing inconsistencies across different trip types. After clustering trips based on fare structures and travel patterns, association rules are applied to reveal underlying relationships between trip attributes, such as congestion surcharges and interborough travel.

### Dataset  

We use the NYC Yellow Taxi Trip Dataset from [NYC Open Data](https://data.cityofnewyork.us/Transportation/2023-Yellow-Taxi-Trip-Data/4b4i-vvec/about_data), which includes:  
- Trip Details: `tpep_pickup_datetime`, `tpep_dropoff_datetime`, `trip_distance`, `passenger_count`  
- Location Identifiers: `PULocationID`, `DOLocationID`  
- Fare Breakdown: `fare_amount`, `extra`, `mta_tax`, `tip_amount`, `tolls_amount`, `total_amount`, `congestion_surcharge`, `airport_fee`  
- Additional Information: `VendorID`, `RatecodeID`, `store_and_fwd_flag`, `payment_type`, `improvement_surcharge`

### Methodology  

We apply Principal Component Analysis (PCA) to reduce dataset dimensionality while preserving over 90% of the variance, ensuring more efficient clustering. The key PCA components are then used for K-Means clustering to classify taxi trips based on fare patterns. Based on the clusters, we further analyzed the root causes of congestion pricing using association rules. This approach helps identify key pricing trends, customer behavior, and potential improvements for taxi fare transparency.

### Contributors  

- Jooyeon Lee
- Crystal Leatvanich 
- Courtney Vincent 
- Christina Son
