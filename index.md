## Introduction/background
Hurricanes are thermally driven, rapidly rotating storm systems characterized by a low-pressure center whose wind speed exceeds 74 miles per hour. In 2005, Hurricane Katrina, a large Category 5 Atlantic hurricane, caused over 1,800 deaths and $125 billion in damage[4]. The top 10 costliest hurricanes in the United States occurred in 21st century[2]. According to real estate analytics firm CoreLogic Inc, at-risk properties have a combined value of $8.5 trillion and more than 32 million homes are at risk of hurricane damage on the Atlantic and Gulf Coasts[3].

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
### Feature Analysis
Large datasets will be costly to operate so data will be filtered first. Removal or data replacement will be considered; interpolation or extrapolation will be used for data replacement. The correlation of the features will be analyzed and dimensions will be reduced by either Principal Component Analysis(PCA) or Uniform Manifold Approximation and Projection(UMAP). Clustering methods will be utilized to visualize and understand each feature. Clustering will also be helpful to remove any noise or unrelated feature in addition to PCA or UMAP.

### Neural Network
Non-linear Neural Network(NN) is a dynamic model to present sequential relationship between variables. Due to the nature of forecasting hurricane trajectories, dynamical spatiotemporal processes, NN will be beneficial and effective[1]. Hyperparameters such as number of hidden layers and learning rate will be tuned via a different method (e.g. Grid Search).

## Potential results and discussion
The model will provide the useful features from the data set and clusters of each feature which the group will analyze. More importantly, it will provide the intensity and the trajectories of hurricanes. However, there will certainly be room for an improvement. The model will not predict the precise damages a hurricane will inflict on certain communities in terms of property damage and loss of life. It will be challenging to produce those results with the same dataset. Additional data will be required to model certain outcomes.

## Reference
1. Alemany, S., Beltran, J., Perez, A., &amp; Ganzfried, S. (2019). Predicting Hurricane Trajectories Using a Recurrent Neural Network. Proceedings of the AAAI Conference on Artificial Intelligence, 33, 468–475. https://doi.org/10.1609/aaai.v33i01.3301468 
2. Facts + Statistics: Hurricanes. III. (n.d.). https://www.iii.org/fact-statistic/facts-statistics-hurricanes.
3. Frank, T. (2021, June 2). Hurricanes Threaten 32 Million U.S. Homes. Scientific American. https://www.scientificamerican.com/article/hurricanes-threaten-32-million-u-s-homes/.
4. Hartono, N. (2020, September 2). A Machine-Learning Assist to Predicting Hurricane Intensity. NASA. https://www.nasa.gov/feature/jpl/a-machine-learning-assist-to-predicting-hurricane-intensity.
