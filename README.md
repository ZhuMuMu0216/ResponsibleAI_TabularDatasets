# ResponsibleAI_TabularDatasets
This is a collection of Tabular Dataset used in ResponsibleAI (eXplainable AI, fairness domain).

Because I am currently doing research in the field of fairness, and I am very anxious with the stage of finding suitable datasets for experiments, so I open this repository to record the current mainstream datasets and their download URLs. For a better visual experience, you can enter https://zhumumu0216.github.io/ResponsibleAI_TabularDatasets/.

### Dataset1: German Credit

1. **Description:** The dataset contains 1000 instances without any missing values and 20 features.
2. **URL:** https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data
3. **Sensitive features:** Age, Sex
4. **Features:**

| Attributes                           | Type         | Values              | # Missing values | Description                                                           |
|--------------------------------------|--------------|---------------------|-------------------|-----------------------------------------------------------------------|
| checking-account                     | Categorical  | 4                   | 0                 | The status of existing checking account                               |
| duration                             | Numerical    | [4 - 72]            | 0                 | The duration of the credit (month)                                   |
| credit-history                       | Categorical  | 5                   | 0                 | The credit history                                                    |
| purpose                              | Categorical  | 10                  | 0                 | Purpose (car, furniture, education, etc.)                            |
| credit-amount                        | Numerical    | [250 - 18,424]      | 0                 | Credit amount                                                         |
| savings-account                      | Categorical  | 5                   | 0                 | Savings account/bonds                                                 |
| employment-since                     | Categorical  | 5                   | 0                 | Present employment since                                              |
| installment-rate                     | Numerical    | [1 - 4]             | 0                 | The installment rate in percentage of disposable income               |
| personal-status-and-sex              | Categorical  | 4                   | 0                 | The personal status and sex                                           |
| other-debtors                        | Categorical  | 3                   | 0                 | Other debtors/guarantors                                              |
| residence-since                      | Numerical    | [1 - 4]             | 0                 | Present residence since                                               |
| property                             | Categorical  | 4                   | 0                 | Property                                                              |
| age                                  | Numerical    | [19 - 75]           | 0                 | The age of the individual                                             |
| other-installment                    | Categorical  | 3                   | 0                 | Other installment plans                                               |
| housing                              | Categorical  | 3                   | 0                 | Housing (rent, own, for free)                                         |
| existing-credits                     | Numerical    | [1 - 4]             | 0                 | Number of existing credits at this bank                               |
| job                                  | Categorical  | 4                   | 0                 | Job (unemployed, (un)skilled, management)                             |
| number-people-provide-maintenance-for| Numerical    | [1 - 2]             | 0                 | Number of people being liable to provide maintenance for              |
| telephone                            | Binary       | Yes, None         | 0                 | Telephone number                                                      |
| foreign-worker                       | Binary       | Yes, No           | 0                 | Is the individual a foreign worker?                                   |
| Risk (target)                         | Binary       |  Good, Bad       | 0                 | Class                                                                 |
5. **Simplified version:** It may be difficult for someone to understand all these features. There is a [simplified version](https://www.kaggle.com/datasets/uciml/german-credit/data) uploaded in the kaggle and it's a readable CSV file.

| Attributes                           | Type         | Values              | # Missing values | Description                                                           |
|--------------------------------------|--------------|---------------------|-------------------|-----------------------------------------------------------------------|
| checking-account                     | Categorical  | 4                   | 0                 | The status of existing checking account                               |
| duration                             | Numerical    | [4 - 72]            | 0                 | The duration of the credit (month)                                   |
| purpose                              | Categorical  | 10                  | 0                 | Purpose (car, furniture, education, etc.)                            |
| credit-amount                        | Numerical    | [250 - 18,424]      | 0                 | Credit amount                                                         |
| savings-account                      | Categorical  | 5                   | 0                 | Savings account/bonds                                                 |
| Sex              | Categorical  | 4                   | 0                 | The personal status and sex                                           |
| age                                  | Numerical    | [19 - 75]           | 0                 | The age of the individual                                             |
| housing                              | Categorical  | 3                   | 0                 | Housing (rent, own, for free)                                         |
| job                                  | Categorical  | 4                   | 0                 | Job (unemployed, (un)skilled, management)                             |
| Risk (target)                         | Binary       |  Good, Bad       | 0                 | Class                                                                 |

### Dataset2: Adult
1. **Description:** Prediction task is to determine whether a person's income is over $50,000 a year based on census data. Also known as "Census Income" dataset. It has 48842 instances and 14 features.
2. **URL:** https://archive.ics.uci.edu/dataset/2/adult
3. **Sensitive features:** Age, Sex, Race
4. **Features:**
    
| **Attributes**      | **Type**       | **Demographic** | **Description**                                                                                                                | **Missing Values** |
|----------------------|----------------|------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------|
| age                 | Integer        | Age              | N/A                                                                                                                           | no                  |
| workclass           | Categorical    | Income           | Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.                        | yes                 |
| fnlwgt              | Integer        |                  | N/A                                                                                                                           | no                  |
| education           | Categorical    | Education Level  | Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool. | no                  |
| education-num       | Integer        | Education Level  | N/A                                                                                                                           | no                  |
| marital-status      | Categorical    | Other            | Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.                    | no                  |
| occupation          | Categorical    | Other            | Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces. | yes                 |
| relationship        | Categorical    | Other            | Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.                                                           | no                  |
| race                | Categorical    | Race             | White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.                                                                  | no                  |
| sex                 | Binary         | Sex              | Female, Male.                                                                                                                 | no                  |
| capital-gain        | Integer        |                  | N/A                                                                                                                           | no                  |
| capital-loss        | Integer        |                  | N/A                                                                                                                           | no                  |
| hours-per-week      | Integer        |                  | N/A                                                                                                                           | no                  |
| native-country      | Categorical    | Other            | United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands. | yes                 |
| income (target)     | Binary         | Income           | >50K, <=50K.                                                                                                                  | no                  |

### Dataset3: KDD Census-Income
1. **Description:** Prediction task is to determine whether a person's income is over $50,000 a year based on census data. This data set contains weighted census data extracted from the 1994 and 1995 Current Population Surveys conducted by the U.S. Census Bureau.It is **an extended version of the Adult Dataset with a larger scale**, used to study classification model performance and feature engineering methods. It has 299285 instances and 41 features.
2. **URL:** https://archive.ics.uci.edu/dataset/117/census+income+kdd
3. **Sensitive features:** Age, Sex, Race
4. **Features:** see more details after entering the url.
    
### Dataset4: Bank Marketing
1. **Description:** The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. It has 45211 instances and 16 features.
2. **URL:** https://archive.ics.uci.edu/dataset/222/bank+marketing
3. **Sensitive features:** Age, (marital)
4. **Features:**
    
| Attributes     | Type         | Demographic       | Description                                                                                                                                                                           | Missing Values |
|-----------------|--------------|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
| age            | Integer      | Age               | Age                                                                                                                                                                                   | no             |
| job            | Categorical  | Occupation        | Type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')            | no             |
| marital        | Categorical  | Marital Status    | Marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)                                                                     | no             |
| education      | Categorical  | Education Level   | (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')                                                        | no             |
| default        | Binary       |                   | Has credit in default?                                                                                                                                                               | no             |
| balance        | Integer      |                   | Average yearly balance                                                                                                                                                               | no             |
| housing        | Binary       |                   | Has housing loan?                                                                                                                                                                    | no             |
| loan           | Binary       |                   | Has personal loan?                                                                                                                                                                   | no             |
| contact        | Categorical  |                   | Contact communication type (categorical: 'cellular','telephone')                                                                                                                     | yes            |
| day_of_week    | Date         |                   | Last contact day of the week                                                                                                                                                         | no             |
| month          | Date         |                   | Last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')                                                                                                     | no             |
| duration       | Integer      |                   | Last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before | no             |
| campaign       | Integer      |                   | Number of contacts performed during this campaign and for this client (numeric, includes last contact)                                                                               | no             |
| pdays          | Integer      |                   | Number of days that passed by after the client was last contacted from a previous campaign (numeric; -1 means client was not previously contacted)                                   | yes            |
| previous       | Integer      |                   | Number of contacts performed before this campaign and for this client                                                                                                                | no             |
| poutcome       | Categorical  |                   | Outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')                                                                                          | yes            |
| y (target)     | Binary       |                   | Has the client subscribed a term deposit?                                                                                                                                            |                |
### Dataset5: Default of Credit Card Clients
1. **Description:** This research aimed at the case of customers' default payments in Taiwan and compares the predictive accuracy of probability of default among six data mining methods. It has 30000 instances and 23 features.
2. **URL:** https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients
3. **Sensitive features:** Age, Sex, (Marital, Education)
4. **Features:**

| **Attributes** | **Type**  | **Demographic**      | **Description**                | **Missing Values** |
|--------------------|-----------|----------------------|--------------------------------|---------------------|
| ID                | Integer   |                      |                                | no                  |
| X1                | Integer   | LIMIT_BAL            |Amount of given credit in NT dollars (includes individual and family/supplementary credit                                | no                  |
| X2                | Binary   | Sex                  | Gender (1=male, 2=female)                               | no                  |
| X3                | Categorical   | Education Level      | (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)                     | no                  |
| X4                | Categorical   | Marital Status       | Marital status (1=married, 2=single, 3=others)                       | no                  |
| X5                | Integer   | Age                  | AGE                            | no                  |
| X6                | Categorical   |                      |Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)                         | no                  |
| X7                | Categorical   |                      |Repayment status in August, 2005 (scale same as above)                         | no                  |
| X8                | Categorical   |                      |Repayment status in July, 2005 (scale same as above)                         | no                  |
| X9                | Categorical   |                      |Repayment status in June, 2005 (scale same as above)                  | no                  |
| X10               | Categorical   |                      |Repayment status in May, 2005 (scale same as above)    | no                  |
| X11               | Categorical   |                      |Repayment status in April, 2005 (scale same as above)                         | no                  |
| X12               | Integer   |                      |Amount of bill statement in September, 2005 (NT dollar)                      | no                  |
| X13               | Integer   |                      |Amount of bill statement in August, 2005 (NT dollar)                    | no                  |
| X14               | Integer   |                      |Amount of bill statement in July, 2005 (NT dollar)                  | no                  |
| X15               | Integer   |                      |Amount of bill statement in June, 2005 (NT dollar)                      | no                  |
| X16               | Integer   |                      |Amount of bill statement in May, 2005 (NT dollar)                     | no                  |
| X17               | Integer   |                      |Amount of bill statement in April, 2005 (NT dollar)                      | no                  |
| X18               | Integer   |                      |Amount of previous payment in September, 2005 (NT dollar)                       | no                  |
| X19               | Integer   |                      |Amount of previous payment in August, 2005 (NT dollar)                       | no                  |
| X20               | Integer   |                      |Amount of previous payment in July, 2005 (NT dollar)                       | no                  |
| X21               | Integer   |                      |Amount of previous payment in June, 2005 (NT dollar)                      | no                  |
| X22               | Integer   |                      |Amount of previous payment in May, 2005 (NT dollar)                     | no                  |
| X23               | Integer   |                      |Amount of previous payment in April, 2005 (NT dollar)                     | no                  |
| Y (target)        | Binary    |                      | default payment next month (1=yes, 0=no)    | no                  |


### Reference:
1. [Le Quy, Tai, et al. "A survey on datasets for fairness‐aware machine learning." Wiley Interdisciplinary Reviews: Data Mining and Knowledge Discovery 12.3 (2022): e1452](https://wires.onlinelibrary.wiley.com/doi/full/10.1002/widm.1452).
2. [Markelle Kelly, Rachel Longjohn, Kolby Nottingham,
The UCI Machine Learning Repository](https://archive.ics.uci.edu).