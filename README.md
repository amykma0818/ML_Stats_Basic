# ML & Stats Basic
### 1. What is standard error of mean, how to compute it, and how to interpret it?
* Standard error is the standard deviation of the sampling distribution of the mean, $`s = σ/\sqrt{n}`$. It refers to the standard deviation of the distribution of sample means
taken from a population. The smaller the standard error, the more representative the sample will be of the overall population (a measurement for the
spread, the smaller the spread, the more accurate the dataset). 

### 2. [How to compute standard error of median in a simple way?](https://towardsdatascience.com/how-to-estimate-the-standard-error-of-the-median-the-bootstrap-strategy-ed09cccb838a)
* Bootstrap. For example randomly select data with replacement from the dataset for 10000 times, so that we can get 10000 new datasets. Consider median as the resampling statistic, get median of each bootstrap dataset and
calculate the standard error from these 10000 median $`\sqrt{(Σ(x_i - \mu(median))^2/(n-1))}/\sqrt{n}`$.
While if the sample is drawn from a normal distribution with large sample size, $`se(median) = 1.2533*se(mean)`$.

### 3. Two-sample t-test vs. paired t-test, which one has higher statistical power?
* Depend on the degree of freedom. Degrees of freedom (DOF) equals your sample size minus the number of parameters you need to calculate during an analysis. Higher DOF generally mean larger sample sizes or fewer unknown parameters, a higher DOF means more power to reject a false null hypothesis and find a significant result.
* The DOF of (unpaired) two-sample t-test is ($`n_1+n_2-2`$)
* The DOF of paired t-test, which is equivalent to one-sample t-test, is ($`n-1`$).

### 4. What's the difference between t-test and z-test?

### 5. What is Analysis of Variance (ANOVA)? [What's the difference between F-test and ANOVA?](https://statisticsbyjim.com/anova/f-tests-anova/)

### 6. What's supervised algorithm? 
* Supervised learning is the use of examples of known correct answers to train the network. A process in which data and its one-to-one correspondence are known, a prediction model is trained, and input data is mapped to a label.
* Common application scenarios for supervised learning such as classification and regression.
* Common supervised machine learning algorithms include Support Vector Machine (SVM), Naive Bayes, Linear Regression, Logistic Regression, K-Nearest Neighborhood (KNN), Decision Tree (including Random Forest and AdaBoost), and Linear Discriminant Analysis (LDA). Deep Learning is also presented in the form of supervised learning.
