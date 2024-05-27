![jessica-ruscello-OQSCtabGkSY-unsplash](https://github.com/sarahprusaitis/Library_Inventory_Management/assets/146799617/d996ea72-bb9a-4f2b-bf32-16131986d268)

# Library Inventory Management Analysis
Author: Sarah Prusaitis | Flatiron School Capstone Project May 2024 

## Overview
This project aims to enhance inventory management at the Seattle Public Library by leveraging historical checkout data of both physical and digital books. By analyzing trends and patterns in the dataset spanning 2022-2023, the project seeks to provide actionable recommendations for optimizing the library's collection. Through predictive modeling, it aims to forecast future demand for various titles, enabling the library to better allocate resources and meet the needs of its patrons efficiently.

## Business Understanding
The primary objective of this project is to assist the Seattle Public Library in optimizing its inventory management system. By analyzing historical checkout data, the project aims to address the challenge of efficiently allocating resources for physical and digital book collections. The library's stakeholders seek insights into trends and preferences among its patrons to anticipate future demand accurately. Through predictive analytics, the project will deliver actionable recommendations to optimize library inventory.

## Data Understanding
The dataset provided by The Seattle Public Library comprises 5.21 million rows and 12 columns, documenting the checkout records of both physical and electronic items over the years 2022 and 2023. Each row represents the number of checkouts for a specific title in a given month of the year. With this rich dataset, the project endeavors to understand the borrowing patterns of library users and identify key factors influencing the demand for books in both formats.

## Exploratory Data Analysis
insert images here of EDA, working on Tableau

## Preprocessing
The dataset was filtered to include on physical books and digital books (eBooks). The 'CheckoutYear' and 'CheckoutMonth' columns were combined into a datetime column, and unnecessary columns were dropped. Additionally any rows where the author was missing was dropped as it was not a substantial number. Standardization of author names in the 'Creator' column was performed followed by the cleaning of the 'Title' column by removing redundent phrases and punctuatio. This was all done to ensure consistency and cleanliness of the data for subsequent EDA and modeling. 

## Conclusion
In this project, I explored various time series forecasting models to assist the Seattle Public Library in optimizing its inventory management system. The models analyzed include the Shift(1) baseline model, the Simple Exponential Smoothing (SES) model, the ARIMA model, and the Prophet Model. The Shift(1) model provided a simple benchmark with an MAE of 3.42 and RMSE of 12.31, indicating significant prediction errors. The SES model demonstrated improved accuracy with an MAE of 2.65 and RMSE of 8.73, making it a more reliable choice for forecasting demand. The ARIMA model, despite its complexity and optimization efforts, resulted in an MAE of 3.07 and RMSE of 8.74, slightly underperforming compared to the SES model. However, the Prophet Model, with its robust approach integrating trend estimation and seasonality modeling, presented the most comprehensive forecasting capabilities and achieved reasonably accurate predictions.

Based on these findings, I recommend the Seattle Public Library adopt the Prophet model for its predictive analytics needs. The Prophet model's superior performance in terms of lower error metrics suggests it is more effective in capturing demand patterns and trends in the library's checkout data. By implementing this model, the library can gain valuable insights into patron preferences, enabling more accurate anticipation of future demand. This will facilitate better resource allocation for both physical and digital collections, ultimately enhancing the efficiency of inventory management and ensuring the library meets the needs of its patrons effectively.


## Future Steps
User feedback incorporation, to validate and help refine the predictive models. 

## Sources:
[data.seattle.gov/Community/Checkouts-by-Title-2022-2023/yw4z-3dsr/about_data 
](https://data.seattle.gov/Community/Checkouts-by-Title-2022-2023/yw4z-3dsr/about_data)
