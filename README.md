# CSE6242_Crime_Prediction

# Project Overview: Crime Hot Spot Prediction and Risk Assessment in Atlanta

## 1. Problem
Our project aims to predict crime hot spots in Atlanta, assign risk scores to each neighborhood, and visualize the results using an interactive map. The main components of our project are:
- Basic exploration of the data (EDA)
- Clustering of crimes using the GMM algorithm based on the latitude and longitude of the crime
- Geographical clusters assigned a risk score reflecting crime severity, providing a monthly and yearly risk profile for each area
- Time series model, Exponential Smoothing, used to forecast geographical crime risk scores from 2019 to 2020, utilizing data from 2009 to 2018
- Visualize this result on an Interactive map of Atlanta

## 2. Clustering Crimes by Location
- The clustering model, a Gaussian Mixture with a K value of 30, successfully distinguished the airport as a unique cluster due to its distinct crime distribution.
- For our crime prediction project, GMM proved superior to K-means due to its ability to handle clusters of varied shapes and densities, crucial for accurately mapping the complex and irregular distribution of crime data.

![Example Image](https://github.com/karan2909/CSE6242_Crime_Prediction/tree/main/Images/Clustering_.png)


## 3. Forecasting Geographical Crime Risk Scores
For predicting risk scores/crime ratings of each cluster, an exponential smoothing time series model was employed, incorporating both trend and annual seasonality. The model was trained on data from 2009 to 2018 and tested on the last 24 months of data (2019 and 2020).

![Example Image](https://github.com/karan2909/CSE6242_Crime_Prediction/blob/main/Images/Risk_Score_Cluster_29.png)


## 4. Results
- This approach provides a reliable method for predicting crime trends in different clusters, which is essential for proactive crime management and resource allocation in community safety initiatives.
- The averaged low SSE of 0.06 and MAPE of 31% across clusters provide a comprehensive measure of the model's efficacy on the test dataset, underlining its practical utility for crime prediction.

![Example Image](https://github.com/karan2909/CSE6242_Crime_Prediction/blob/main/Images/vis3.jpeg)

## 5. Conclusion
In conclusion, our analysis reveals a consistent pattern in crime distribution across Atlanta.
- Notably, neighborhoods near Five Points and the Hotel District consistently exhibit the highest risk scores or crime ratings, while areas such as Carey Park, Kirkwood, and East Lake Highlands, further from the city center, show the least.
- The central zones, including Home Park/Atlantic Station and Midtown, are identified as common crime hotspots, predominantly for vehicular larceny and auto theft. This suggests a targeted need for increased policing of these specific crime types within these regions. Additionally, an encouraging trend observed is the general reduction in crime ratings over the years, indicating the potential effectiveness of current crime prevention strategies.
