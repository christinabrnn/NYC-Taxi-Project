## NYC Taxi Fare Analysis

This project analyzes New York City taxi fare pricing patterns using unsupervised machine learning techniques, including K-Means clustering, hierarchical clustering, and anomaly detection. The goal is to identify fare discrepancies, assess the impact of congestion pricing, and detect unfair pricing trends across different neighborhoods.

### Dataset  
We use the NYC Yellow Taxi Trip Dataset from [NYC Open Data](https://data.cityofnewyork.us/Transportation/2023-Yellow-Taxi-Trip-Data/4b4i-vvec/about_data), which includes:  
- Trip Details: `tpep_pickup_datetime`, `tpep_dropoff_datetime`, `trip_distance`, `passenger_count`  
- Location Identifiers: `PULocationID`, `DOLocationID`  
- Fare Breakdown: `fare_amount`, `extra`, `mta_tax`, `tip_amount`, `tolls_amount`, `total_amount`, `congestion_surcharge`, `airport_fee`  
- Additional Information: `VendorID`, `RatecodeID`, `store_and_fwd_flag`, `payment_type`, `improvement_surcharge`

### Methodology  
We apply Principal Component Analysis (PCA to reduce dataset dimensionality while preserving over 90% of variance, ensuring more efficient clustering. The key PCA components are then used for K-Means clustering to classify taxi trips based on fare patterns. The optimal number of clusters is determined using the Elbow Method and Silhouette Score, allowing for well-defined groupings. This approach minimizes noise, enhances clustering accuracy, and uncovers fare trends, particularly the impact of congestion pricing.

### Contributors  
- Jooyeon Lee
- Crystal Leatvanich 
- Courtney Vincent 
- Christina Son
