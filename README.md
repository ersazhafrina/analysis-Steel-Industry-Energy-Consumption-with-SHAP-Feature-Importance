# analysis-Steel-Industry-Energy-Consumption-with-SHAP-Feature-Importance-and-EDA
This portfolio is made for the Final Project of Bootcamp Data Science. The Source Code will explain in Bahasa. This Project is analyzing about What factors most influence the Type of Energy Load, What Factor which triggered an energy load that is classified as a maximum load, how effectively the energy load has been consumed.

# Dataset Information
This dataset is data on the energy load consumed by DAEWOO Steel Co. Ltd  for 1 year (2018)

# Objective
Energy consumption is one of the important aspects in the industrial world. The more effectively the energy is consumed, the more efficient the costs incurred. This project presents an analysis of what factors most influence the Type of Energy Load and What Factor which triggers an energy load that is classified as a maximum load also how effectively the energy load has been consumed

# Attribute Information
1. Date – datetime per 15 minutes
2. Usage_kWh = Industry Energy Consumption - Continuous (kWh)
3. Lagging_Current_Reactive.Power_kVarh = Lagging Current reactive power - Continuous (kVarh)
4. Leading_Current_Reactive_Power_kVarh = Leading Current reactive power - Continuous (kVarh)
5. CO2(tCO2) = rate of CO2(CO2) - Continuous (ppm)
6. Lagging_Current_Power_Factor = Lagging Current power factor -Continuous (%)
7. Leading_Current_Power_Factor = Leading Current Power factor Continuous - (%)
8. NSM  = Number of Seconds from midnight Continuous - (s)
9. WeekStatus= Week status - Categorical (Weekend (0) or a Weekday(1))
10. Day_of_week= Day of week - Categorical Monday to Sunday
11. Load_Type= Load Type - Categorical Light Load, Medium Load, Maximum Load

# Step
1. Make sure the csv file and the code in one folder
2. Place the csv in your google drive and change the path on the code to connect it, or place the csv file in one folder with the code and change the path
3. After the code connected with the dataset, run all the code, then you will see the result and you can conclude with your own word

# Insight
1. Sunday is the day with the lightest energy use
2. Light_load energy usage increases as the day progresses (closer to Sunday)

![image](https://user-images.githubusercontent.com/56376510/197701291-32920a6a-8e1a-4f93-83a6-e705dbfc4d4c.png)

3. From the three graphs above, usage_kWh, Lagging_Current_Reactive.Power_kVarh and CO2, have a tendency to increase at maximum load. It can be seen that these 3 factors have a fairly high graph at maximum load

![Capture](https://user-images.githubusercontent.com/56376510/197701686-f16f63a7-d178-4d69-a029-e701fa696b35.PNG)

4. From modeling, it can be seen that the NSM has the largest value, it means NSM has high contribution to prediction/target column

![download](https://user-images.githubusercontent.com/56376510/197702760-2982af65-62ee-4d11-ba9f-5e78057f4f53.png)

# Conclusion
1. NSM is the most influencing factor for the type of energy load
2. The closer to the weekend, the lighter the energy load
3. Usage_kWh, Lagging_Current_Reactive.Power_kVarh and CO2 triggered an energy load that is classified as a maximum load
4. SHAP Feature Importance where this method will provide SHAP (SHapley Additive ExPlanations) values which are based on cooperative game theory and are used to increase transparency and interpretation of machine learning models. From the 3 summary plots above, all of them show the same thing, so the conclusions from the modeling are considered the same as the conclusions from the EDA that has been done
5. When viewed from the energy load distribution plot, it can be seen that the light load has the highest number among the others. So, it can be said that energy consumption for 2018 is still considered effective

Article Link : https://medium.com/@ersazhafrina/analysis-steel-industry-energy-consumption-with-shap-feature-importance-and-eda-31491d1d672d
