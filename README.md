# SOLAR-AND-WIND-ENERGY-PREDICTION

SOLAR AND WIND ENERGY PREDICTION using Machine and Deep Learning models


   
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#salient-features">Salient Features</a></li>
       <li><a href="#built-with">Built With</a></li>
        <li><a href="#compatible-platforms">Compatible Platforms</a></li>    
      </ul>
    </li>
      <a href="#Description">Description</a>
      <ul>
        <li><a href="#dataset">dataset</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#navigating-through-the-app">Navigating through the App</a></li><ul>
      </ul>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About the project
* Solar energy is one of several sustainable sources that is becoming increasingly important in the energy sector due to its potential to cut carbon emissions and counteract growing electricity prices. The main issue with solar energy is that it cannot be used due to the constantly shifting and unpredictable weather, cloud cover, climate, and seasons. As a result, solar energy generation varies. Therefore, resource planners and businesses are looking for models that take these uncertainties into account for the daily design and management of solar energy production, which could enable them to meet consumer demand and supply regardless of weather conditions.
* Weather complexity makes accurate synthesis of wind output difficult, and commercial confidentiality means that historical data is frequently limited. We present and validate a model for simulating the hourly power output of wind farms located anywhere in the world.

### Salient Features
Predicts real-time solar and wind energy. Accuracy, mean square error, root mean square error, mean absolute error are calculated for each algorithm and different hyperparameters and the best one is chosen.

### Compatible Platforms
Laptops, Desktops and Tablet PCs

### Built With

### Tech stack used
* Frontend: HTML, CSS, Bootstrap
* Backend: JavaScript, Python
* Prediction models: ML/DL models
* ML Models: Lasso Regression, Ridge Regression, Decision Tree, SVM, Random Forest
* DL Model: LSTM
* Concordium Used


## Description
### Dataset 
Data was collected from https://open-power-system-data.org/ which is a free open source platform with data on power systems for 37 European countries. But we chose to focus on a specific country, Germany, due to having the highest proportion of renewable energy than any other country(about 46 percent of its energy come from solar, wind, biomass) and hence it is a good indicator of where the rest of the world is headed. The data file contained about 16 variables like utc_time stamp,solar capacity,wind capacity,solar profile, wind profile,wind_onshore, wind_offshore profile.

###Data Pre-processing 

A.Removing missing values in ground truth values (if any)
1. For solar generation actual, wherever there is a null value, it has been filled with the value for a day before.
2.For the first day of the month, since there is no previous day value, it has been filled with 0 assuming there is no solar generation before 6 am.
3.Replacing the leftover Nan with mean of the data of solar generation actual 
4. For wind generation actual, wherever there is a null value, it has been filled with the mean value of the entire wind generation actual column

B.Correlation analysis show that some features are more correlated to target variables. Solar profile is most correlated with solar generation output. In case
of wind energy, wind profile, wind onshore profile, wind onshore generation followed by wind offshore profile and wind offshore generation.
![image](https://user-images.githubusercontent.com/87893594/211166713-8d524bdd-aba9-44fb-bbbb-466499250238.png)


C.Feature Importance: Along with correlation analysis, feature importance was used to select the most appropriate features of our dataset for robust model training. Useless data must be removed for low bias. It is a technique that calculates the score of each input feature. The score indicates the importance of that feature. 



### Team
- Mehak Aggarwal
- Sonanshi Goel
- Shambhavi Rai
- Princy Singhal
