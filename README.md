🎈🎈# ENSEMBLE METHODS🎈🎈

❤️❤️##BUSINESS PROBLEM❤️❤️

Recruiting and retaining drivers is seen by industry watchers as a tough battle for Ola. Churn among drivers is high and it’s very easy for drivers to stop working for the service on the fly or jump to Uber depending on the rates.

As the companies get bigger, the high churn could become a bigger problem. To find new drivers, Ola is casting a wide net, including people who don’t have cars for jobs. But this acquisition is really costly. Losing drivers frequently impacts the morale of the organization and acquiring new drivers is more expensive than retaining existing ones.

You are working as a data scientist with the Analytics Department of Ola, focused on driver team attrition. You are provided with the monthly information for a segment of drivers for 2019 and 2020 and tasked to predict whether a driver will be leaving the company or not based on their attributes like

  1.Demographics (city, age, gender etc.)
  2.Tenure information (joining date, Last Date)
  3.Historical data regarding the performance of the driver (Quarterly rating, Monthly business acquired, grade, Income)
  
❤️❤️##MY ANALYSIS❤️❤️

1. I imported the dataset and checked the no. of rows and no. of columns.
2. I dropped the non useful columns
3. I grouped the data by Driver_id
4. Calculated target by placing 0 if last working date is not null and 1 if last working date is mentioned.
5. Calculated Income_increase and Quaterly_income_increase columns.
6. Encoded City column using Target Encoding as it has more no. of values.
7. Splitted the data into training and test data.
8. By seeing the plots I concluded that 
        There are more males than females
        There are more employees from City C20
        There are almost equal employees from all education levels
        There are more people from Joining Designation with 1
        There are more drivers with grade 2 attime of reporting
        There are more drivers whose quaterly rating with 1
        Quaterly income and Monthly income increase are very less
9. By using HaetMap I concluded that there are some coulmns correlated but I didn't remove anything as there is less data.
10. No missing value treatment is required as there are no missing values.
11. I removed outliers using IQR method.
12. Scaled the data using Standard Scaling Method.
13. Here am Concentrating more on FN so am considering Recall as my parameter.
14. By training the model using Random Forest I got 0.92 as Recall_Score which is considered as good.
15. By training the model using Boostimg I got 0.85 as Recall_score.
16. ROC curves looks fine for both the models.
17. By calculating feature_importances of both these models I can say that Age, Total business value, City and Income are playing vital role for this business problem.
18. As I got good Recall_score I can consider any one of these columns.





