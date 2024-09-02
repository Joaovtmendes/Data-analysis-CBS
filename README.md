# Data-analysis-CBS

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16qMk8a7tQysTQ0qg7DJyQ2-zGp73vqTp?usp=sharing)


## Introduction:

CBS Dance Factory is a dance school located in São José dos Campos, SP, with a long history of success and prestige in Brazil. The school implemented a recurring payment model starting in January 2023, and the data forecast aims to optimize cash flow and better understand variations in the number of students and revenue. Company 

## Expectation: 

The project was created to organize CBS Dance Factory's cash flow, avoiding major fluctuations in the months with the highest and lowest student influx. The objective is to analyze the impact of the change to the recurring model on revenue and identify patterns that can help with financial management.
  
## Project's goal:
- Viewing the number of students enrolled in 2023 and 2024;
- Viewing revenue per month;
- Analysis of the sales funnel;
- Creating a forecast model to predict revenue for the next 4 months.

## Technologies Used:
<p align="left">  
  <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> 
  <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> 
  <a href="https://numpy.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="numpy" width="40" height="40"/> 
  <a href="https://matplotlib.org/" target="_blank" rel="noreferrer"> <img src="https://seeklogo.com/images/M/matplotlib-logo-7676870AC0-seeklogo.com.png" alt="matplotlib" width="40" height="40"/> 
 <a href="https://powerbi.microsoft.com/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/New_Power_BI_Logo.svg/630px-New_Power_BI_Logo.svg.png" alt="powerbi" width="40" height="40"/> 
  <a href="https://www.microsoft.com/pt-br/microsoft-365/excel" target="_blank" rel="noreferrer"> <img src="https://seeklogo.com/images/E/excel-logo-974BFF9CB9-seeklogo.com.png" alt="excel" width="40" height="40"/> 
  
## Data collection:

At this stage, the data was extracted from the CRM spreadsheets and the company's revenue and registration report.

## Data Preparation:

To prepare the data, the Pandas libraries were used to perform the following functions:
Pandas: https://pandas.pydata.org/docs/user_guide/index.html#user-guidefunções:
- Duplicate Analysis: Identification and removal of duplicate records to ensure data integrity.
- Null Value Analysis: Identification and exclusion of null values ​​that may compromise the analysis.
- Column Cleaning: Removal of the unnecessary "Unnamed" column to simplify the data set.
- Customer Filtering: Creation of a new column called is_cliente with True and False values. Deletion of rows where is_cliente = False.

## Modeling techniques:

For the exploratory analysis stage, the Plotly libraries was used to perform a graphical analysis to understand the number of students enrolled per month between 2023 and 2024. It was employed to aggregate the enrollment values monthly and to analyze variations in revenue. Additionally, Plotly was used to develop the sales funnel based on the contacts made, including students who scheduled a trial class, those who inquired about enrollment, and ultimately, the acquisition of new clients.

- Plotly: https://plotly.com/python-api-reference/

For the Forecast model stage, the States model library was used.
- States Model: https://www.statsmodels.org/stable/api.html

## Results:

- From the bar graph showing the number of students per month, we can observe a seasonal pattern in enrollments. The months of August and January are when the enrollment numbers tend to rise, coinciding with the back-to-school period. Our recommendation is to capitalize on this back-to-school period by increasing investment in marketing to attract even more customers.
<p align="center">
<img  width="60%" src="https://github.com/user-attachments/assets/e735dd37-3096-4029-a2fd-1daea1fd82a9">
</p>

-The same pattern was observed in the revenue graph; revenue increases in tandem with the number of students. Our suggestion is that, given the highly seasonal nature of the business, the ideal approach is to focus on incentives during peak enrollment months. This strategy should aim to convert new students into recurring ones and retain them in the following months when enrollment is lower.
<p align="center">
<img  width="60%" src="https://github.com/user-attachments/assets/0512df9b-abeb-4e86-b2d5-fdebfebf1425">
</p>

  - When analyzing the CRM, we observed that through direct and indirect marketing campaigns, a substantial number of leads were generated and converted into trial classes. Following these classes, some individuals sought additional information, such as pricing and availability. Ultimately, we reached the final stage of the funnel, where those who completed the enrollment are found. We found that only 6.95% of the leads who engaged actually completed the enrollment. This indicates a need for greater focus on the enrollment closing process. Once a customer has participated in a trial class, the company must present the best options to facilitate enrollment. Therefore, it is important to collaborate with the sales team to understand why the conversion rate is so low.
<p align="center">
<img  width="80%" src="https://github.com/user-attachments/assets/f01209ee-1f73-4d8c-bd19-53fc5df409ac">
</p>

- In addition, we used Power BI to perform a more in-depth analysis of the company's expenses to determine if there were opportunities to reduce costs and increase revenue per collection. One factor that stood out was the increase in personal withdrawals and salaries over the months, which was in line with revenue growth but could be detrimental to the company. Our recommendation was to separate personal accounts from business accounts to ensure that the director's personal expenses do not affect the analysis and financial health of the company. We also suggested reviewing the staffing to determine if we could reduce or optimize class hours, thereby involving fewer professionals.
<p align="center">
<img  width="80%" src="https://github.com/user-attachments/assets/66d7b5f1-0fc3-4ea7-87ae-68af362b1da5">
</p>


## Solution:

Using the pdmarima and statsmodels models, we performed a forecast analysis to predict revenue for the next 4 months based on the current scenario. We suggest monitoring these 4 months to evaluate whether the improvement suggestions we made will maintain the same results or if we can achieve even better outcomes.

The recommendations were:

Capitalize on the back-to-school period by increasing investment in marketing to attract more customers.
Focus on converting new students into recurring ones and retaining them in the following months when enrollment tends to be lower.
Enhance the enrollment closing process. Once a customer has participated in a trial class, the company should offer the best options to facilitate enrollment. It is crucial to work with the sales team to understand why the conversion rate is low.

<p align="center">
<img  width="80%" src="https://github.com/user-attachments/assets/84540db8-a53e-47b7-a7ed-a43200cadc59">
</p>
