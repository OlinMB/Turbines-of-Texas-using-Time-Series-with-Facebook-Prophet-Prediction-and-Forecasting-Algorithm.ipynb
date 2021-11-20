# Turbines-of-Texas-using-Time-Series-with-Facebook-Prophet-Prediction-and-Forecasting-Algorithm.ipynb

The features analyzed in this dataset: 
1. System_power_generated_kW
2. Wind_speed_m/s
3. Wind_direction_deg
4. Pressure_atm
5. Air_temperature_C

All the features are highly correlated with each other, giving a value of 1. Also, each feature gives an almost perfect Gaussian distribution.

Since the data is a multivariate dataset, but neither of the features follow a comon pattersn. this means that none of the variables are dependent on each other, which eliminates the possibility of using Vector AutoRegression (VAR) model for forecasting. Also, the data, when plotted, also does not exhibit any repititive patterns, which makes the data non-seasonal and eliminates the possibility of using the SARIMAX and LightGBM models. Hence, we have chosen to exhibit the forecasting of each feature in the dataset by using Facebook's Prophet model.

Through the Prophet algorithm, we have plotted the forecasting for the consecutive year of each individual feature, as well as broken down the components of each graph to display the trends by days and months. In all the cases, the forecasting shows that the values increase over time, whereas the rends of days show that the trends decrease on weekdays but rise on weekends.
