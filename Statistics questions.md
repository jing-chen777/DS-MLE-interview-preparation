# Statistics
## Most important concept ranking:
p-value: measures the likelihood of extreme results, assuming the null hypothesis is true.
Linear regression
t-test
correlation coefficient
type of errors (Type 1 false, type 2 false false)
## 1.	Assumptions of t-test: INE
•	Independence: Observations within each group should be independent.
•	Normality: Data in each group should follow a normal distribution. (flexible for large sample)
•	Equal variance: Variances of two groups should be approximately equal.
2.	Assumptions of z-test: INK
•	Independence
•	Normal distribution
•	Known population standard deviation
3.	Difference between t-test and z-test?
 
4.	What is hypothesis and p-value?
A hypothesis in statistics is a claim or assumption about a population parameter (like the mean or proportion) that you want to test using data.
Null hypothesis vs. alternative hypothesis
The p-value is the probability of obtaining test results at least as extreme as the observed results, assuming the null hypothesis is true.
Example: If you get a p-value of 0.03, it means there is a 3% chance of observing your results (or more extreme) if H₀ were true. Since 0.03 < 0.05, you would reject H₀.
5.	How to avoid sampling bias?
Using probability selection methods: random sampling, systematic sampling, stratified sampling, and cluster sampling.
6.	What are the differences between correlation and covariance?
Covariance measures the degree to which two variables change together. A positive covariance indicates that as one variable increases, the other tends to increase, and vice versa for negative covariance. (Note: no range constrain for covariance)
Correlation is a standardized measure of the strength and direction of the linear relationship between two variables. It ranges from -1 to 1, with -1 indicating a perfect negative linear relationship, 1 indicating a perfect positive linear relationship, and 0 indicating no linear relationship.
7.	How to fix imbalance data?
1.	Resampling:
o	Oversampling: Increase the number of instances in the minority class by duplicating or generating synthetic samples. (Method: SMOTE)
o	Undersampling: Decrease the number of instances in the majority class by randomly removing samples or using more sophisticated techniques.
2.	Weighted Models:
o	Adjust the weights of classes in the algorithm to give more importance to the minority class. This is applicable in machine learning algorithms that allow for class weights.
3.	Model Selection:
o	Use ensemble methods like Random Forest or AdaBoost, which can be effective for imbalanced datasets. These methods combine predictions from multiple models, which can help mitigate the impact of imbalanced classes.
o	Choose fewer sensitive models to class imbalance. For example, decision trees and support vector machines can handle imbalanced datasets well.
4.	Evaluation Metrics:
o	Using confusion matrix instead of only accuracy score.
5.	Stratified Sampling:
o	When splitting the dataset into training and testing sets, use stratified sampling to ensure that both sets maintain the same class distribution as the original dataset.
8.	What is the difference between descriptive and inferential statistics?
Inferential statistics involve making predictions or inferences about a population based on a random sample of data taken from that population. It uses various methods to estimate population parameters, test hypotheses, and make predictions. While descriptive statistics summarize and describe the features of a dataset, inferential statistics use the data to make generalizations and draw conclusions about a larger population.
9.	What are the different types of sampling methods?
•	Simple random sampling gives every member of the population an equal chance of being selected. 
•	Systematic sampling involves selecting every k-th member of the population, starting from a randomly chosen point. 
•	Stratified sampling divides the population into strata or subgroups, with random samples taken from each stratum. 
•	Cluster sampling divides the population into clusters, randomly selecting some clusters and sampling all members within them.
10.	What is the central limit theorem?
The central limit theorem states that the distribution of the sample mean will approach a normal distribution as the sample size increases, regardless of the population's distribution, provided the samples are independent and identically distributed.
11.	What is probability distribution?
A probability distribution describes how the values of a random variable are distributed.  
•	Discrete probability distribution: binomial distribution or poisson distribution. 
•	Continuous probability distribution: normal distribution or exponential distribution.
12.	Binomial distribution
E(x) = n*p
13.	Poisson distribution
It models the number of events occurring within a fixed interval of time or space, where the events occur independently and at a constant average rate. It is appropriate to use when you want to model the count of rare events, such as the number of emails received in an hour or the number of earthquakes in a year.
14.	Type 1 error and type 2 error?
•	Healthy people wrongly predict sickness. (False positive)
•	Sick people wrongly predict as healthy. (False negative)
15.	What is the difference between parametric and non-parametric tests?
Parametric tests, like the t-test, Z-test, and ANOVA, assume a specific distribution (e.g., normal) and require known population parameters. When these assumptions aren't met—especially with small samples—non-parametric tests like the Chi-Square test, Mann-Whitney U test, Wilcoxon Signed-Rank Test, and Kruskal-Wallis test are more appropriate.
16.	What are residuals?
Residuals are the differences between the observed values and the predicted values from a regression model.
17.	What is confidence interval?
A confidence interval is a range of values, derived from sample data, that is likely to contain the true population parameter (like a mean or proportion) with a specified level of confidence. It is the range of values explaining the uncertainty surrounding an estimate.
For example, a 95% confidence interval means that if you repeated the experiment many times, 95% of the calculated intervals would contain the true value.
18.	In what situations do we not use p-value = 0.05?
•	General situations are large sample size (smaller p-value) or small sample size(larger p-value).
•	In fields like medicine and engineering, smaller thresholds are often used to minimize the risk of false positives, avoiding sever consequences caused by errors.
•	In exploratory studies or early-stage research, a higher threshold might be used to avoid dismissing potentially important findings that require further investigation.
19.	What is the bias-variance tradeoff?
The bias-variance tradeoff in machine learning involves balancing two error sources. Bias is an error from overly simplistic model assumptions, causing underfitting and missing data patterns. Variance is the error from excessive sensitivity to training data fluctuations, causing overfitting and capturing noise instead of true patterns.
20.	What are the advantages of different imputation methods?
Each imputation method has its pros and cons. For example, mean/median/mode imputation is easy to implement but can introduce bias and distort relationships between variables. K-nearest neighbors (KNN) imputation considers relationships between variables and can lead to more accurate results, but it can be computationally expensive.
21.	What is the difference between exponential smoothing and ARIMA models?
Exponential Smoothing models use weighted averages of past observations for simple, short-term forecasting. ARIMA models combine autoregression, differencing, and moving average components, making them more complex but suitable for both short-term and long-term forecasting, especially with complex patterns and significant autocorrelations.
