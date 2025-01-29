# ResponsibleAI_TabularDatasets
This is a collection of Tabular Dataset used in ResponsibleAI (eXplainable AI, fairness domain).
For a better visual experience, you can enter https://zhumumu0216.github.io/ResponsibleAI_TabularDatasets/. 

Because I am currently doing research in the field of fairness, and I am very anxious with the stage of finding suitable datasets for experiments, so I open this repository to record the current mainstream datasets and their download URLs. And I will continue updating.

### Dataset1: German Credit

1. **Description:** The dataset contains 1000 instances without any missing values and 20 features.
2. **URL:** https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data
3. **Sensitive features:** Age, Sex
4. **Features:**

| Attributes                           | Type         | Values              | Description                                                           |
|--------------------------------------|--------------|---------------------|-----------------------------------------------------------------------|
| checking-account                     | Categorical  | 4                   | The status of existing checking account                               |
| duration                             | Numerical    | [4 - 72]            | The duration of the credit (month)                                   |
| credit-history                       | Categorical  | 5                   | The credit history                                                    |
| purpose                              | Categorical  | 10                  | Purpose (car, furniture, education, etc.)                            |
| credit-amount                        | Numerical    | [250 - 18,424]      | Credit amount                                                         |
| savings-account                      | Categorical  | 5                   | Savings account/bonds                                                 |
| employment-since                     | Categorical  | 5                   | Present employment since                                              |
| installment-rate                     | Numerical    | [1 - 4]             | The installment rate in percentage of disposable income               |
| personal-status-and-sex              | Categorical  | 4                   | The personal status and sex                                           |
| other-debtors                        | Categorical  | 3                   | Other debtors/guarantors                                              |
| residence-since                      | Numerical    | [1 - 4]             | Present residence since                                               |
| property                             | Categorical  | 4                   | Property                                                              |
| age                                  | Numerical    | [19 - 75]           | The age of the individual                                             |
| other-installment                    | Categorical  | 3                   | Other installment plans                                               |
| housing                              | Categorical  | 3                   | Housing (rent, own, for free)                                         |
| existing-credits                     | Numerical    | [1 - 4]             | Number of existing credits at this bank                               |
| job                                  | Categorical  | 4                   | Job (unemployed, (un)skilled, management)                             |
| number-people-provide-maintenance-for| Numerical    | [1 - 2]             | Number of people being liable to provide maintenance for              |
| telephone                            | Binary       | Yes, None         | Telephone number                                                      |
| foreign-worker                       | Binary       | Yes, No           | Is the individual a foreign worker?                                   |
| Risk (target)                        | Binary       | Good, Bad         | Class                                                                 |

5. **Simplified version:** It may be difficult for someone to understand all these features. There is a [simplified version](https://www.kaggle.com/datasets/uciml/german-credit/data) uploaded in the kaggle and it's a readable CSV file.

### Dataset2: Adult
1. **Description:** Prediction task is to determine whether a person's income is over $50,000 a year based on census data. Also known as "Census Income" dataset. It has 48842 instances and 14 features.
2. **URL:** https://archive.ics.uci.edu/dataset/2/adult
3. **Sensitive features:** Age, Sex, Race
4. **Features:** see more details after entering the url.

### Dataset3: KDD Census-Income
1. **Description:** Prediction task is to determine whether a person's income is over $50,000 a year based on census data. This data set contains weighted census data extracted from the 1994 and 1995 Current Population Surveys conducted by the U.S. Census Bureau.It is **an extended version of the Adult Dataset with a larger scale**, used to study classification model performance and feature engineering methods. It has 299285 instances and 41 features.
2. **URL:** https://archive.ics.uci.edu/dataset/117/census+income+kdd
3. **Sensitive features:** Age, Sex, Race
4. **Features:** see more details after entering the url.
    
### Dataset4: Bank Marketing
1. **Description:** The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. It has 45211 instances and 16 features.
2. **URL:** https://archive.ics.uci.edu/dataset/222/bank+marketing
3. **Sensitive features:** Age, (marital)
4. **Features:** see more details after entering the url.

### Dataset5: Default of Credit Card Clients
1. **Description:** This research aimed at the case of customers' default payments in Taiwan and compares the predictive accuracy of probability of default among six data mining methods. It has 30000 instances and 23 features.
2. **URL:** https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients
3. **Sensitive features:** Age, Sex, (Marital, Education)
4. **Features:** see more details after entering the url.

### Dataset6: COMPAS 
1. **Description:** COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) is a popular commercial algorithm used by judges and parole officers for scoring criminal defendant’s likelihood of reoffending (recidivism). It has been shown that the algorithm is biased in favor of white defendants, and against black inmates, based on a 2 year follow up study (i.e who actually committed crimes or violent crimes after 2 years).
2. **URL:** https://github.com/propublica/compas-analysis/
3. **Sensitive features:** Age, Sex, **Race (many researches here)**
4. **Features:** see more details after entering the url.
5. **Simplified Versions:** 
    - [compas-scores-two-years.csv](https://github.com/propublica/compas-analysis/blob/master/compas-scores-two-years.csv) (common version, 7215 instances, subset of compas-scores.csv),
    - [compas-scores-two-years-violent.csv](https://github.com/propublica/compas-analysis/blob/master/compas-scores-two-years-violent.csv) (4743 instances, subset of compas-scores.csv), 
    - [compas-scores-raw.csv](https://github.com/propublica/compas-analysis/blob/master/compas-scores-raw.csv) (it needs more preprocessing), 
    - [compas-scores.csv](https://github.com/propublica/compas-analysis/blob/master/compas-scores.csv) (11757 instances)

### Dataset7: Diabetes 130-US Hospitals
1. **Description:** The dataset represents ten years (1999-2008) of clinical care at 130 US hospitals and integrated delivery networks. Each row concerns hospital records of patients diagnosed with diabetes, who underwent laboratory, medications, and stayed up to 14 days. The goal is to determine the early readmission of the patient within 30 days of discharge.
2. **URL:** https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008
3. **Sensitive features:** Age, Sex, Gender
4. **Features:** see more details after entering the url.
5. **Comment from website:** Not a bad dataset, but definitely not for beginners or intermediates. This is a very imbalanced dataset, and even if you manage to soften this issue with under/oversampling techniques, the chance of distinguishing between the majority and minority class is very small. Confusion matrices look like a mess, don't count on the usual accuracy metric. Even feature engineering, or even PCA techniques, can't find any reliable new source of info, not enough to have enough true positives without making too many false positive at the same time. But this is just part of the nature of the problem we are trying to solve itself. 

### Reference:
1. [Le Quy, Tai, et al. "A survey on datasets for fairness‐aware machine learning." Wiley Interdisciplinary Reviews: Data Mining and Knowledge Discovery 12.3 (2022): e1452](https://wires.onlinelibrary.wiley.com/doi/full/10.1002/widm.1452).
2. [Markelle Kelly, Rachel Longjohn, Kolby Nottingham,
The UCI Machine Learning Repository](https://archive.ics.uci.edu).