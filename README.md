🎈🎈# ENSEMBLE METHODS🎈🎈

❤️❤️##BUSINESS PROBLEM❤️❤️

Recruiting and retaining drivers is seen by industry watchers as a tough battle for Ola. Churn among drivers is high and it’s very easy for drivers to stop working for the service on the fly or jump to Uber depending on the rates.

As the companies get bigger, the high churn could become a bigger problem. To find new drivers, Ola is casting a wide net, including people who don’t have cars for jobs. But this acquisition is really costly. Losing drivers frequently impacts the morale of the organization and acquiring new drivers is more expensive than retaining existing ones.

You are working as a data scientist with the Analytics Department of Ola, focused on driver team attrition. You are provided with the monthly information for a segment of drivers for 2019 and 2020 and tasked to predict whether a driver will be leaving the company or not based on their attributes like

  1.Demographics (city, age, gender etc.)
  2.Tenure information (joining date, Last Date)
  3.Historical data regarding the performance of the driver (Quarterly rating, Monthly business acquired, grade, Income)
  
❤️❤️##MY ANALYSIS❤️❤️

1. I imported the data set and did some basic pre-processing on data.
2. I checked this Dataset has 145063 rows and 551 columns.
3. I have seen null values for some websites after some days. I concluded that new websites are created.
4. I dropped the columns which has all null values that means the website not at all visited.
5. I also dropped that websites which has more than 300 null values as they are newly created.
6. After dropping off rows which has some null values there are some null values for existing rows so I filled them using backward fill method.
7. I splitted the Page column as I need to do modelling for only english websites
8. By plotting the graphs I concluded that among all languges English website has more no. of views and Access origin whith all_agents are visited more. Websites with access_type all_acccess are vistied more. Desktop and mobiles websites are vistied equally.
9. Then I grouped the data for each language.
10. Checked for stationarity using ADfuller test.
11. As data is non stationary I removed trend and seasonality by differentaiting.
12. ACF and PACF plots are plotted.
13. I ran ARIMA model and selected best p and q values which has less MAPE.
14. By using obtained best p and q values from ARIMA model I ran SARIMAX model and got best P and Q values.
15. By using the best obtained p,q,P,Q values I ran SARIMAX model and calculated MAPE.




