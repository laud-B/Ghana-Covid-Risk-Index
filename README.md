# Ghana-Covid-Risk-Index

# **Summary**  

>On March 11 2020, the World Health Organization declared Covid-19 a pandemic. My project 1.analysis flu trends in Ghana for the year 2019, 2.construct a disease risk index for Ghana and 3.Provides in sights on Ghana's Flu season for 2019 (May to July) and Oct- Nov.The data is sourced from the DHIMS-2 Health information database of the Ghana Health Service. The Ghana Covid Risk Index project will provide summary statistics and use data visualization tools describe the disease and risk burden in Ghana.


#  **Instructions**


## **script.py**


### **Data Collection**
Two datasets saved as as csv files serve as the datasets for the analysis. Dataset
1. Flu data by month, details the monthly reported cases of Upper Respiratory Tract Infections in 2019 by the districts and regional organizational region. The columns in data set are the organizational units (districts in Ghana) and the flu=Upper Respiratory Tract Infections cases by month.

2. Dataset 2, Ghana Disease Trend 2017-2019, details the monthly reported cases for 2017,2018 and 2019 by districts. Five diseases conditions, namely 1. anemia diagnosed at out patient department(OPD),2 suspected malaria cases, 3. Upper Respiratory Tract Infections, 4. Diabetes Mellitus, and 5. Hypertension. The 2019 data on Diabetes Mellitus is not available in this dataset.



### **Data Cleaning and Preprocessing**
1.The Flu data had four empty columns and 320 empty rows which were dropped.

2.The Ghana Disease Trend dataset had 320 empty rows which were dropped.

3.The Flu data columns was then reorganized to reflect the headings 'org_unit_name','District_GIS','region','Jan19','Feb19','Mar19','Apr'....'Dec'.

4.To assess national trends total cases on each month was computed of monthly columns and a bar chart created. Bar chart saved as Ghana Flu Trends 2019.

5.To assess contribution of each district to total flu cases reported per year, the ratio of monthly reported cases/total yearly cases was computed. The new columns were labeled Jan19ratio', 'Feb19ratio', 'Mar19ratio',....'Dec19ratio were grouped together. Flu season is trimodal in Ghana, I further compute the contribution of districts to May-July flu season and 3 Oct-Nov flu season by adding ratios up and saving us flu_data.

6.Regional monthly Heatmps was then created using seaborn and picture saved as "Heat map of Flu cases by region Ghana". Figure size used was (10,5) and scale (2, 3, 4,5, 6, 7 , 8, 9, 10, 11, 12 , 13,14, 15]}, vmin = 2, vmax = 15).

7.To develop the Ghana Covid Risk Index, dataset Ghana Disease trends was used. The Covid Risk index is calculated using 2019 cases as Ghana Covid Risk Index= (0.5 * Anemeia cases/distrist/month) + (1 * Hypertension cases/distrist/month) + (1 * Diabetes cases/distrist/month) +(0.5 * Upper Respiratory Tract Infection Cases /distrist/month) + (0.5 * Malaria cases/distrist/month), and saved as Ghana_disease_trend. The total score was used to develope GIS maps of risk.

8.GIS Maps created by joined datasets with variables or columns District_edit/Districts/QGIS_District on data set and shape file. 

9.GIS maps was then created for Ghana Covid Risk Index, Proportion of cases between May and July, and Oct/ Nov.

7.Resulting ouput was saved as sort_data which included elements 'District','Region','QGIS_District','COVID_Risk_index'.

8.GIS maps were created using shape files store in folder Ghana Shape files. 

9.Develop a power point presentation and save as APA-2020.pdf




 
