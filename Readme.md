COVID_19 CAPSTONE PROJECT OVERVIEW



The project objective of this project is to basically analyze the effect and impact of COVID-19 pandemic on Nigeria. 
Data science and python skills and techniques  was used to coalate, explore, analyze and visualize these data sets to generate insights.
This analysis basically shows:
Top 10 confirmed states including the state with the highest number of infected patients
Top 10 death states including the state with the highest number of patients casuality
Top 10 discharged states including the state with the highest number of discharged patients
Shows the rate of infection, death, and discharged.
Explpored the relationship between number of lab confirmed cases with the vulnerabilty index and fragility of these states
Explored relationship between confirmed cases with population density, Age index and Healthcare index
Explored the effect of the pandemic on GDP and Budget of each states




	DATA COLLECTION AND METHODOLOGY

Data used for this analysis was sourced from different channels using various data collection skills like web scrapping and directly reading CSV files. 
The Nigeria Centre for Diseases Control (NCDC) monitors the country’s COVID-19 situation and releases data on metrics across all 37 states in the country. Data could not be scrapped from NCDC COVID-19 official website, because at the time of this analysis, the web page was down. I downloaded it from the provided GitHub repository into my local drive and loaded the data from there.

o	COVIDNG = pd.read_csv("covidnig.csv")

Data was collected from Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE) publishes daily data on confirmed, death, and recovered cases across different countries. Nigeria’s daily data was accessed from its repository , Nigeria’s data was extracted from the global data and derived 
o	related insights.  (details in the submitted code notebook)
o	(DF_CONFIMED_DAILY = pd.read_csv("https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv")

o	DF_RECOVERED_DAILY =pd.read_csv ('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_recovered_global.csv')

o	DF_DAILY_DEATHS = pd.read_csv("https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_deaths_global.csv")

Nigeria Community Vulnerability Index data
The vulnerability index was computed by considering several factors such as socio-economic status, population density, housing type, transportation, epidemiological, health system, etc, these factors are known as themes. Each theme was broken into subthemes, and data was gathered from them to compute the overall vulnerability index score by weighing equally each theme. This data was got from the COVID-19 external data.

Real Domestic Gross Product Data
was used for this analysis and this data was on the Real Domestic Gross Product(GDP) data for Nigeria
State Budget Data was used in this analysis as the data provides information on the reduced subsequent budget because of the impact of COVID-19 on the economy. The percentage difference in the budget was computed and used to visualize the effects of COVID-19 on the budget of the affected states.






	CONCLUSIONS/SUMMARY

Lagos state has the highest confirmed cases followed by the FCT and Kaduna, Plateau, Oyo, Rivers, Edo, Ogun, Kano, and Delta State. 
Lagos state has the highest death cases followed by Edo, FCT, Rivers, Kano, Delta, Kaduna, Oyo, Ondo, Borno.
Lagos state has the maximum discharged cases, followed by FCT, Plateau, Kaduna, Oyo, Rivers, Edo, Ogun, Kano, Delta.
Daily maximum infection was on 2023-03-08 with 93 cases.
There is no direct correlation between the vulnerability index and confirmed cases. Factors like age index, and population density affected the rate of infection more compared to the vulnerability index.
There were waves of infection observed between February 2020 to March 2022. It is evident in the recovery rate marching up with the rate of infection and low death rate that the pandemic was properly managed and curtailed. 
The economy was visibly affected as seen in the GDP, especially in the 2nd quarter of 2020.






	FURTHER WORK TO BE DONE
More reliable data sources could be researched, and I personally will want to employ the knowledge of Machine learning and artificial intelligence to further make accurate guesses and proffer predictions on the data and the probability of using such predictions to combat similar futuristic occurrences.		

