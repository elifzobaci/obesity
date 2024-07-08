
# Obesity -Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/de4fb756-2088-4d11-be63-91aa4e36bc9d?ctid=81ac3fcb-0e34-42f5-be8e-7b8d22860e1b&pbi_source=linkShare

## Problem Statement

This dashboard helps the understand which key elements cause the Obesity. This dataset includes information of obesity levels in individuals from Mexico, Peru, and Colombia, based on their dietary habits and physical condition. The data contains 17 attributes and 2111 records, which are labeled with the class variable NObesity (Obesity Level), allowing classification using the values Underweight, Normal Weight, Overweight Level I, Overweight Level II, Obesity Type I, Obesity Type II, and Obesity Type III. 77% of the data was synthetically generated using the Weka tool and the SMOTE filter, while 23% of the data was collected directly from users through a web platform.  

Column Names :

- Gender  
- Age 
- Height 
- Weight
- family_history_with_overweight 
- FAVC (Frequent consumption of high caloric food) 
- FCVC (Frequency of consumption of vegetables)
-  NCP (Number of main meals)
- CAEC (Consumption of food between meals)
- SMOKE
- CH2O (Consumption of water daily)
- SCC (Calories consumption monitoring)
- FAF (Physical Activity Frequency)
- TUE (Time using technology devices)
- CALC (Consumption of alcohol)
- MTRANS (Transportation Used)
- NObesity (Obesity level)

Our goal at this project how we can decrase the obesity? How we can prevent it? 

### Steps followed 

- Step 1 : Load data into MS SQL Server.
- Step 2 : Delete the null values of columns Age, FCVC, NCP, CH2O, FAF, TUE.
- Step 3 : Delete the Insufficient_Weight datas from the NObeyesdad column.
- Step 4 : The column of NCP Values was 1,2,3. Updated 1 values to 0.33, 2 values to 0.66, 3 values 1.
- Step 5 : Step 4 repeated for columns CH2O, FAF, TUE columns. 
- Step 6 : By filtering the Normal Weight level data in the NObesity column, the ratio of smokers was found and this was called smokers ratio. By filtering data other than the Normal Weight level in the NObesity column, the ratio of smokers to all data was found and this was called smokers ratio. 
- Step 7 : When people of normal weight and other weight groups were examined, it was seen that smoking had no effect on obesity.
- Step 8 : Step 6 and Step 7 repeated for family_history_with_overweight and as a result Those with a family history of obesity were more likely to be overweight and obese than those without a family history of obesity.
- Step 9 : Step 6 and Step 7 repeated for FAVC Frequent consumption of high caloric food and as a result hhen people of normal weight and other weight groups were examined, it was seen that  FAVC Frequent consumption of high caloric food had big effect on obesity.
- Step 10 : Step 6 and Step 7 repeated for  NCP (Number of main meals),  CAEC (Consumption of food between meals), CH2O (Consumption of water daily), SCC (Calories consumption monitoring), FAF (Physical Activity Frequency), TUE (Time using technology devices), CALC (Consumption of alcohol),  MTRANS (Transportation Used) and Gender.
- Step 11 : It has been observed that obesity decreases as FAF (Physical Activity Frequency) increases. For the SCC (Calories consumption monitoring) criterion, the SCC (Calories consumption monitoring) rate decreases as the obesity level increases, namely obesity level 1, obesity level 2 and obesity level 3. Considering the CH2O (Consumption of water daily) criterion, people of normal weight consume water in the range of 1-2 L. This rate generally decreases as the obesity level increases.

- There is no significant value relationship recorded for the other criteria.


STAR METHOD :
Situation : We have the data from Latin American countries 

Snap of Obesity Power BI Dashboard

![Obesity_Power_BI](https://github.com/elifzobaci/obesity/assets/153128702/f241415f-3e1c-4dd7-9527-b8e557157ad1)


![Obesity_Power_BI_2](https://github.com/elifzobaci/obesity/assets/153128702/96f4a1cd-3bc6-4c6e-b002-ac6ddc3d124d)
