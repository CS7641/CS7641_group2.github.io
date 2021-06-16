## Introduction/background
Hurricanes are thermally driven, a rapidly rotating storm system characterized by a low-pressure center whose wind speed exceeds 74 miles per hour. In 2005, Hurricane Katrina, a large Category 5 Atlantic hurricane, caused over 1,800 deaths and $125 billion in damage. In fact, the top 10 costliest hurricanes in the United States occurred in 21st century. According to real estate analytics firm CoreLogic Inc, the at-risk properties have a combined value of $8.5 trillion. Additionally, more than 32 million homes are at risk of hurricane damage on the Atlantic and Gulf Coasts.

### Top 5 Costliest Hurricanes in the United States
($ millions)
|Year|Hurricane|Dollars when occured|In 2020 dollars|
|----|---------|--------------------|---------------|
|2005| Katrina |       $65,000      |    $86,570    |
|2012| Sandy   |       $30,000      |    $33,930    |
|2017| Harvey  |       $30,000      |    $31,960    |
|2017| Irma    |       $29,900      |    $31,850    |
|2017| Maria   |       $29,670      |    $31,270    |

This prediction model would identify if the storm will hit certain locations. A timely warning can be issued to the at-risk communities and a preliminary relief can be sent to those locations.

## Problem definition
The goal of the project is to accurately predict the hurricane trajectories or track forecasting which will identify the location and the intensity of the hurricane by utilizing diverse data sources to reduce any economic damages and save lives. A set of predicted models can lower any errors and forecast a few days ahead.

## Methods
### Feature Analysis
Large datasets will be costly to operate. Data will be filtered first. Removal or data replacement will be considered; interpolation or extrapolation will be used for data replacement. The correlation of the features will be analyzed and dimensions will be reduced by either Principal Component Analysis(PCA) or Uniform Manifold Approximation and Projection(UMAP). Clustering methods will be utilized to visualize and understand each feature. Clustering will also be helpful to remove any noise or unrelated feature in addition to PCA or UMAP.

### Neural Network
Non-linear Neural Network(NN) is a dynamic model to present sequential relationship between variables. Due to the nature of forecasting hurricane trajectories, dynamical spatiotemporal processes, NN will be beneficial and effective. Hyperparameters such as number of hidden layers and learning rate will be tuned via a different method (e.g. Grid Search).

## Potential results and discussion
The model will provide the useful features from the data set and clusters of each feature which the group will analyze. More importantly, it will provide the intensity and the trajectories of hurricanes. However, there is going to be room for an improvement. The model will not predict how much the hurricane will damage certain communities in terms of properties and lives. It will be challenging to produce those results with the same dataset. Additional data will be required to model certain outcomes.

## Reference
1. Facts + Statistics: Hurricanes. III. (n.d.). https://www.iii.org/fact-statistic/facts-statistics-hurricanes.
2. Frank, T. (2021, June 2). Hurricanes Threaten 32 Million U.S. Homes. Scientific American. https://www.scientificamerican.com/article/hurricanes-threaten-32-million-u-s-homes/.
3. Hartono, N. (2020, September 2). A Machine-Learning Assist to Predicting Hurricane Intensity. NASA. https://www.nasa.gov/feature/jpl/a-machine-learning-assist-to-predicting-hurricane-intensity.
4. Maier, H. R., and Dandy, G. C. 2000. Neural networks for the prediction and forecasting of water resources variables: a
review of modelling issues and applications. Environmental modelling & software 15(1):101–124
