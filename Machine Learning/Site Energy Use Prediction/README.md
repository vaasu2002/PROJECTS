# Site Energy Use Prediction

### About:- 

According to a [report](https://www.iea.org/reports/tracking-buildings-2021) issued by the International Energy Agency (IEA), the lifecycle of buildings from construction to demolition were responsible for 37% of global energy-related and process-related CO2 emissions in 2020. Yet it is possible to drastically reduce the energy consumption of buildings by a combination of easy-to-implement fixes and state-of-the-art strategies. 

### Dataset
The dataset consists of building characteristics, weather data for the location of the building, as well as the energy usage for the building and the given year, measured as Site Energy Usage Intensity (Site EUI). Each row in the data corresponds to a single building observed in a given year.

### **Problem Statement:**
 You are provided with two datasets: (1) the train\_dataset where the observed values of the Site EUI for each row are provided and (2) the x\_test dataset the observed values of the Site EUI for each row are removed and provided separately in y\_test. Your task is to predict the Site EUI for each row (using the complete training dataset), given the characteristics of the building and the weather data for the location of the building. Use the test sets for validation and testing. 

The target variable is **site\_eui** and the evaluation metric is **RMSE** score.

[**ALL THE FILES OF THIS PROJECT**](https://drive.google.com/drive/folders/1-0qvfb9NkcHkxBwyYooPgPEnkSaumbHO?usp=sharing)
