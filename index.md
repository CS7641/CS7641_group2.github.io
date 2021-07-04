## Introduction/background
Hurricanes are thermally driven, rapidly rotating storm systems characterized by a low-pressure center whose wind speed exceeds 74 miles per hour. In 2005, Hurricane Katrina, a large Category 5 Atlantic hurricane, caused over 1,800 deaths and $125 billion in damage. The top 10 costliest hurricanes in the United States occurred in 21st century. According to real estate analytics firm CoreLogic Inc, at-risk properties have a combined value of $8.5 trillion and more than 32 million homes are at risk of hurricane damage on the Atlantic and Gulf Coasts.

### Top 5 Costliest Hurricanes in the United States
($ millions)

|Year|Hurricane|Dollars when occured|In 2020 dollars|
|----|---------|--------------------|---------------|
|2005| Katrina |       $65,000      |    $86,570    |
|2012| Sandy   |       $30,000      |    $33,930    |
|2017| Harvey  |       $30,000      |    $31,960    |
|2017| Irma    |       $29,900      |    $31,850    |
|2017| Maria   |       $29,670      |    $31,270    |

The proposed prediction model will identify whether a storm will hit certain locations. A timely warning or preliminary relief can be issued to at-risk communities. Additionally, this information can be used by responders to plan and prepare for upcoming disasters.

## Problem definition
The goal of this project is to accurately predict the hurricane trajectories or track forecasting which will identify the location and the intensity of the hurricane by utilizing diverse data sources to reduce economic damages and save lives. A set of predicted models can lower errors and forecast a few days ahead.

## Methods
### Data Collection
The dataset used for this project is the Atlantic Hurricane Database obtained by the National Hurricane Center (NHC) after a post-storm analysis of all available storm observations. The database includes entries dating as far back as 1851 and include numerous features including longitude, latitude, and windspeed of the storm at given times. The data was cleaned of cyclones with missing feature data (this was common for storms that occurred before modern instrumentation was introduced) then formatted in order to visualize hurricane trajectory.

<p align="center">
  <img width="460" height="300" src="/hurricane_trajectories.jpg">
</p>
<p align="center", font=8pt>
  <b>Figure 1:</b> Trajectories of five recent Atlantic hurricanes based on data provided by the NHC.
</p>

### Feature Analysis
Large datasets will be costly to operate and therefore needs filtering. In order to determine the importance of each feature, Principle Component Analysis was used to determine which components are most directly correlated with the hurricane's trajectory. The goal is to find the minimum number of components which captures at least 90% of the variance in the dataset. Given a set of moving cylcone trajectories and a query trajectory, we hope to use the K Nearest Neighbors (KNN) technique to find the next point to which the cyclone will travel. 

<p align="center", style="font-size:8px">
  <img width="500" height="320" src="/corr_features.jpg"> 
</p>
<p align="center", font=8px>
  <b>Figure 2:</b> Correlation of features from the NHC dataset.
</p>

<p align="center", style="font-size:8px">
  <img width="400" height="260" src="/pca_analysis.jpg"> 
</p>
<p align="center", style="font-size:8px">
  <b>Figure 3:</b> Results of PCA Analysis. PC1 explains > 60% of data variance.
</p>

Clustering methods will be utilized to visualize and understand each feature. Clustering will also be helpful to remove any noise or unrelated feature in addition to PCA or UMAP.

### Neural Network
Non-linear Neural Network(NN) is a dynamic model to present sequential relationship between variables. Due to the nature of forecasting hurricane trajectories, dynamical spatiotemporal processes, NN will be beneficial and effective. Hyperparameters such as number of hidden layers and learning rate will be tuned via a different method (e.g. Grid Search).

## Potential results and discussion
The model will provide the useful features from the data set and clusters of each feature which the group will analyze. More importantly, it will provide the intensity and the trajectories of hurricanes. However, there will certainly be room for an improvement. The model will not predict the precise damages a hurricane will inflict on certain communities in terms of property damage and loss of life. It will be challenging to produce those results with the same dataset. Additional data will be required to model certain outcomes.

## Reference
1. Alemany, S., Beltran, J., Perez, A., &amp; Ganzfried, S. (2019). Predicting Hurricane Trajectories Using a Recurrent Neural Network. Proceedings of the AAAI Conference on Artificial Intelligence, 33, 468–475. https://doi.org/10.1609/aaai.v33i01.3301468 
2. Facts + Statistics: Hurricanes. III. (n.d.). https://www.iii.org/fact-statistic/facts-statistics-hurricanes.
3. Frank, T. (2021, June 2). Hurricanes Threaten 32 Million U.S. Homes. Scientific American. https://www.scientificamerican.com/article/hurricanes-threaten-32-million-u-s-homes/.
4. Hartono, N. (2020, September 2). A Machine-Learning Assist to Predicting Hurricane Intensity. NASA. https://www.nasa.gov/feature/jpl/a-machine-learning-assist-to-predicting-hurricane-intensity.
