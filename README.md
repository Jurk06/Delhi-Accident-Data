# Delhi-Accident-Data

CONTENT
	Dataset description
	Missing values
	EDA
	District
	Victims
	TYPE OF ACCIDENT
	# INJURED
	# KILLED
	Chi-Square test for Independence  
	Model
	Assumptions
	Cocnlusion















INTRODUCTION:
Delhi accident data has been collected on the year 2008 to 2017. Since this dataset contains the following feature mentioned below across the different districts of DELHI.
Dataset Overview : 
The following feature of the dataset is collected and each feature are defined below.

Features	Description	Scale
YEAR	year when data was recorded	Interval
DISTRICT	Districts of Delhi	NOMINAL
VEHICLE AT FAULT	vehicle which is responsible for the accidents	NOMINAL
VICTIM	who were hit	NOMINAL
TYPE OF ACCIDENT	Accident is fatal or not	NOMINAL
# INJURED	Number of injuries during the accident	Ratio
# KILLED	Number of persons were killed after the accidents	Ratio

Here we will list the explanatory and response variables of the Delhi Accident Dataset.

Features	Respense / Explanatory
Variable
YEAR	Explanatory
DISTRICT	Explanatory
VEHICLE AT FAULT	Explanatory
VICTIM	Explanatory
TYPE OF ACCIDENT	Response
# INJURED	
# KILLED	

Response variable: 
Since the type of accident is response variable in this dataset.  The frequency counts of the fatal, simple and non-fatal accidents are given below. From the chart we can interpret that the SIMPLE ACCIDENTS is maximum which is 73%, FATAL ACCIDENTS is almost 24% and rest is NON-INJURY which is very less. 

 
Fig-1 









Table-1 Contingency table (For Given Districts & across the different year)
	District	NEW DELHI			
Year	Fatal	Non-fatal	Total	Probability of fatalities	Odd's ratio
2008	302	784	1086	0.2780847145	0.3852040816
2009	267	687	954	0.2798742138	0.3886462882
2010	292	641	933	0.3129689175	0.4555382215
2011	281	602	883	0.3182332956	0.4667774086
2012	239	603	842	0.283847981	0.3963515755
2013	214	604	818	0.2616136919	0.3543046358
2014	202	821	1023	0.1974584555	0.2460414129
2015	184	807	991	0.1856710394	0.2280049566
2016	199	672	871	0.2284730195	0.2961309524
2017	171	572	743	0.2301480485	0.298951049

The hypothesis is to be tested are
Ho: For a given district given the year, the probability of Fatalities and non-fatalities accident are independent.
H1: They are not independent.
Chi-Square test-
  Chi-square calculated value is more than critical value. Hence we reject our null hypothesis and conclude that district the proportion of Fatal and non-fatal accidents are not equal for a given district of given year.
Probability Model:-                   P(Y=1|x_1=District,x_2=Year)
Features	Category
Districts	Explanatory
Year	Explanatory
Probability of 
fatalities	Response



Random Variables:
Response variable is random variables,
Distribution:- 
The response variable follow binomial distribution with parameter 1) number of observation, 2) probabilities of fatalities.
Conclusion:
 Here response variable is probability of fatality , districts and years are explanatory variables. Since response variable has binary outcome, hence the probability follows the binomial distribution.
 
Fig-2
Observation:
	We plot the variation of fatalities across the time line.
	We see the variation of the fatalities rate is not constant.
	Since the districts can be an important features while calculating the response variables.





Table-2 Contingency table (For Given Vehicle at fault & across the different year)
				Vehicle At Fault	PVT CAR
Year	Fatal	Non-fatal	Total	Probability of fatalities	Odd's ratio
2008	209	1782	1991	0.1049723757	0.1172839506
2009	234	1591	1825	0.1282191781	0.1470773099
2010	320	1560	1880	0.170212766	0.2051282051
2011	308	1719	2027	0.1519486926	0.1791739383
2012	277	1605	1882	0.147183847	0.1725856698
2013	265	2004	2269	0.1167915381	0.1322355289
2014	277	2338	2615	0.1059273423	0.1184773311
2015	305	2389	2694	0.1132145509	0.1276684805
2016	261	2027	2288	0.1140734266	0.1287617168
2017	280	1681	1961	0.1427842937	0.1665675193
Total	2736	16914	21432		

The hypothesis is to be tested are
Ho: For a given vehicle at fault given the year, the probability of Fatalities and non-fatalities accident are independent.
H1: They are not independent.
Chi-Square test-
 Chi-square calculated value is more than critical value. Hence we reject our null hypothesis and conclude that district the proportion of Fatal and non-fatal accidents are not equal for a given district of given year
Probability Model:-       P(Y=1|x_1=Vehicle at fault,x_2=Year)
Features	Category
Vehicle at 
Fault 	Explanatory
Year	Explanatory
Probability of 
fatalities	Response


Random Variables:
Response variable is random variables,  
Distribution:
The response variable follow binomial distribution with parameter 1) number of observation, 2) probabilities of fatalities. 

Conclusion:
 Here response variable is probability of fatality , vehicle at fault and years are explanatory variables. Since response variable has binary outcome, hence the probability follows the binomial distribution.
 

Observation: 
	As it can be seen that the fatalities rate has great variation for the given condition vehicle at fault and given year.
	Since the fatalities rate is greatly impacted by the UNKNOWN and HTV/GDS.
	Beside that we can see that the rates of fatalities are quite low due to PVT car and Motor cycle. This is quite good figure
	As it can be seen that UNKNOWN and HTV/GDS are important features for the further analysis,.



Table-3 Contingency table (For Given VICTIM & across the different year)
				VICTIM	PEDESTRIAN
Year	Fatal 	Non-fatal	Total	Probability of fatalities	Odd's ratio
2008	1033	2797	3830	0.2697127937	0.369324276
2009	1157	2322	3479	0.3325668295	0.4982773471
2010	945	2178	3123	0.3025936599	0.4338842975
2011	951	2078	3029	0.313965005	0.4576515881
2012	820	2085	2905	0.2822719449	0.3932853717
2013	744	2278	3022	0.2461945731	0.3266022827
2014	742	2738	3480	0.2132183908	0.2710007305
2015	672	2569	3241	0.2073434125	0.2615803815
2016	678	2346	3024	0.2242063492	0.2890025575
2017	701	2038	2739	0.2559328222	0.3439646712
TOtal	8443	20632	31872
The hypothesis is to be tested are
Ho: For a given victim given the year, the probability of Fatalities and non-fatalities accident are independent.
H1: They are not independent.
Chi-Square test
 Chi-square calculated value is more than critical value. Hence we reject our null hypothesis and conclude that district the proportion of Fatal and non-fatal accidents are not equal for a given district of given year
. Probability Model:-                   P(Y=1|x_1=VICTIM,x_2=Year)
Features	Category
Victim	Explanatory
Year	Explanatory
Probability of
fatalities	Response

Random Variables
 Response variable is random variables,  

Distribution
The response variable follows binomial distribution with parameter 1) number of observation, 2) probabilities of fatalities. 
Conclusion
 Here response variable is probability of fatality , Victim and years are explanatory variables. Since response variable has binary outcome, hence the probability follows the binomial distribution.
 
Observation 
	We can see that we have taken the 3 type of victim as the fatalities rate is statistically significant in this case. 
	We see that variation of the fatalities rate across the year for the given condition Victim
	The trend is quite common for the fatalities rate of Pedestrians and S/C &M/C.
	While the fatalities due to car has variation. 







 
Observation:
	As we can see that rate of fatalities of accidents vary greatly when the condition is given districts i.e. New Delhi given years. 
	Since the variation of the fatalities varies significantly when the condition is Victim i.e. Pedestrians for the given year.
	 The fatalities rate is very less in case of given condition is Vehicle at fault i.e. Pvt-car for the given year. 
	As we can see that overall observation we can say that District and Vehicle at fault are two most important features. Though 










 

Observation
	As we can see that putting the two condition District and different vehicle types. 
	It can be seen that the variation in probability of fatalities is more.
	Since there are no trends we can observe here. 











 

Observation:
	As we can see the variation of fatalities rate is varying 
	There are no such trends


 



 

Observation
	We can see that the variation in fatalities is great.
	We can say that probabilities of fatalities is greatly impacted by the given condition i.e. district, year and vehicle at fault.





















Modelling 
As we can see that it is some sort of classification problem based on this we need to find out 
	For a particular district on given year when an accident occurred, it is a fatal or simple. I have ignored the effect of Non-fatal accident. 
	To do the above we will have to perform some sort of features transformation, as most of the features in this dataset are categorical type. 
	As we can see that the response variable is binary and categorical type. 
	The explanatory variable are most of them are categorical one.
	 I think for binary Logistic Regression will perform very well. 
Assumption for Logistic Regression:
	Logistic Regression model requires the dependent variable to be binary, multinomial or ordinal in nature. In our case it is binary.
	It requires the observations to be independent of each other. So, the observations should not come from repeated measurements.
	Logistic Regression algorithm requires little or no multicollinearity among the independent variables. It means that the independent variables should not be too highly correlated with each other.
	Logistic Regression model assumes linearity of independent variables and log odds.
	The success of Logistic Regression model depends on the sample sizes. Typically, it requires a large sample size to achieve the high accuracy.

Decision Boundary
Since we know about sigmoid function and decision boundary in logistic regression. We can use our knowledge of sigmoid function and decision boundary to write a prediction function. A prediction function in logistic regression returns the probability of the observation being positive, Fatal accident or simple. We call this as class 1 and it is denoted by P(class = 1). If the probability inches closer to one, then we will be more confident about our model that the observation is in class 1, otherwise it is in class 0.

Steps 1:  The dependent variable is Binary  
As we can see that we have response variables or dependent variables is binary as it has two outcome i.e. Fatal or simple accident. Hence one of the assumptions is true
Steps 2:  Observation to be independent 
    We can see that we need to find out, if the features are independent or not. To do this we have found out the Pearson’s correlation with respect to response variables.
 
       Since we see that the correlation is almost zero i.e. we can say that the features are independent to each other. 
Step 3: Little or no multicollinearity among the independent variables
   From the above diagram we can say that there is no correlation among the features, beside that VIF is almost 1. Hence we can say that there is no multicollinearity among the features.
Step 4:- Model assumes linearity of independent variables and log odds.
    We have calculated the log-odds in the Table-1 and it is independent. Hence we can say that this is assumption is true.
  Hence all the required assumption is true. 

 

Explanatory variables:
   To train the model we have taken only two explanatory variables. Those variables are 1) District & 2) Year. The dependent variable is Type of accidents.
Splitting the dataset
  To train and test the models I have split the dataset into train and test. As we can see that training dataset contain 70% and test dataset contains 30%.  The train will be fed into the model and test data will be used to calculate the accuracy of the model by using the respective metrics
Model
   As we have two features that we are using and feeding into the model. Logistic Regression is parametric approach to classify the binary class. It has two coefficients, one for districts and one for year and one is intercept
f(x)=b_0+b_1*x+b_2*x
Where b0 is intercept
And b1 is coefficients for district
And b1 is the coefficients for year

Calculation 
  Feeding the training dataset into the model we evaluates the coefficients as
Intercepts (b0)        - 0.561992
DISTRICT (b1)           1.1698
YEAR (b2)               -12.1282





To Test of Individual Regression Coefficients
Hypothesis is stated as
H_0: bj=0  (coefficients are zeo)
H1:- bj !=0 
The test statistic for testing above hypothesis is t-test
t_0=bj/(SE(bj))

  After performing the test we observe that following results  
 
Conclusion
	As we can see that both the coefficients are quite significant.
	P-value is less than 0.05 which mean we reject our null hypothesis.
	Both the coefficients are significant to the log regression.
	Beside that we can get the confidence interval of both the coefficients.
	We ll have the confidence interval of the each of the coefficients.
	We ll have the standard error as well. 







Using Dummy variables
  Since we can see that above result is not up to the marks, so I have tried using the dummy variables for each of the districts and years as well and have performed the separate analysis in order to obtains the importance of the features among the districts and the years.
Districts
  Here I have taken each districts as dummy variables and tried to find out which districts performs as most significant and most insignificant ones. 
 
To Test of Individual Regression Coefficients
Hypothesis is stated as
       Ho:- bj=0
H1:- bj !=0
The test statistic for testing above hypothesis is t-test
𝑡0 =(bj-0)/s.e(bj) * s.e is standard error
Conclusion: 
  As we can see that we have 11 districts which work as features to the datasets. We can make some conclusion on that basis
	P-value of the districts’ UNK and OUTER are greater than the significance levels, on the basis of that we can say that these two districts is not useful anymore i.e. these districts are statistically insignificant. Since the coefficient of the OUTER district is very large which affect our models and not taking into the account.
	The most significant district is SHARDANA as its coefficient is higher among the other districts.
	Beside that confidence interval for each of the districts has been found out. 
ROC-AUC
   To measure accuracy of the models we have one of the good metrics is ROC-AUC. It is drawn between True positive rate and false positive rate. For dummy model AUC value is 0.5, so for any model AUC is less than 0.5 we can conclude that the model is not performing well. 
   In our case here the ROC-AUC curve 
 
Observation
	We can see that dotted line is representing the dummy model and continuous curve is representing the Logistic Regression.
	It can be seen that our model is performing little better than he dummy models. 
Conclusion
   We can conclude that all the districts except the OUTER and UNK, all the districts are statistically significant.  
Year
   Taking year as one of the features and computing the coefficients of each of the years and get the details of statistically significant years. After performing the feature engineering and feeding into the model and here is what I have arrived at 
 
Observation
	Since there are ten features as we can see that P-values of each of the year is less than significant level and we can conclude that we can say that all the years are statistically significant.
	We can see that the coefficients of most of the features are almost equal. We can conclude that these features are most important features. 
	Beside that confidence interval of each of the features are calculated.
ROC-AUC
  We can see that still the model is performing better than the dummy variables. 
 
Conclusion 
  After the analysis and using the right metrics we can conclude that all the year are statistically significant
