# Water-level-prediction

# 6510742569 Worayot Liamkaew CN240 Project

### Problem and Objective

Water from water station "E98" and water station "M182" flows to water station "M7", which takes 2-3 days, causes it to raise its water level, which can lead to flood. The problem is to find out what is the relationship of water volume of water station "E98", water station "M182" and water station "M7" and the objective is trying to predict water volume at water station "M7" from the relationship.

### Data source

Data is obtained from website "Lower Northeastern Region Hydrological Irrigation Center" (Link: http://hydro-4.rid.go.th/) can be found in "Hourly data" section (Red button below the title). The data was collected since 1st of August, 2561 which contains hourly data (most consistently collected at specific time at '6.00', '9.00', '12.00', '15.00' and '18.00' until now).

The received data will be trimmed since it takes at most 3 days for the water to flow from water station "E98" and water station "M182" to water station "M7", the data of water station "E98" and water station "M182" will be shifted down 3 days to correctly match the data. The unused data will then be deleted and save the new data as csv file named "trimmed_hourly_data.csv" and use it for training the model where "M7" is value to be predicted or target variable and the features are "E98" and "M182".
