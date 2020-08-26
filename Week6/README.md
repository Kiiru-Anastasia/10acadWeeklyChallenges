# Bank Institution Term Deposit Predictive Model

**Client : Bank of Portugal**

### Business Need
The investment and portfolio department for Bank of Portugal wants to be able to identify the customers who potentially would subscribe to term deposits. There has been heightened interest of marketing managers to carefully tune their directed campaigns to the rigorous selection of contacts, therefore, the goal of the employer (Bank of Portugal) is to find an effective model that can predict which future clients would subscribe to their term deposits.

**Why do we need an effective predictive model?**

An effective predictive model can help increase the campaign efficiency as they would be able to identify customers who would subscribe to their term deposit, therby direct their marketing efforts to them. Additionally the model will help them better manage their resources (human effort, phone calls, time, etc.)

The Bank of Portugal, therefore, collected a huge amount of data that includes customer profiles of those who have subscribed to term deposits and the ones who did not subscribe to a term deposit to be used as basis for analysis.

To come up with an effective predictive model, this project will cover:
1. [Data Exploration]()
2. [Data Cleaning]()
3. [Feature Extraction]() and
4. [Development of Robust Machine Learning Algorithms]()

First, we access and understand the features of our data.

### Data and Features
The data for this project is a 20 features and one target variable dataset found [here](http://archive.ics.uci.edu/ml/datasets/Bank+Marketing). The data source has multiple datasets but we will be using the bank-additional-full.csv dataset found [here](http://archive.ics.uci.edu/ml/machine-learning-databases/00222/bank-additional.zip). The same dataset can be found in the data folder in the repository.

The 20 features in our dataset are equally distributed into categorical and numerical features, i.e. 10 categorical features and 10 numerical features.

**Categorical Features:**

1. *job* - type of job of customer ('admin', 'blue-collar', 'entrepreneur', 'housemaid', 'management', 'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown')
2. *marital* - marital status of a customer ('divorced', 'married', 'single', 'unknown')
3. *education* - education level of the customer ('basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')
4. *default* - whether the customer has credit in default ('no', 'yes', 'unknown')
5. *housing* - whether customer has housing loan ('no', 'yes', 'unknown')
6. *loan* - whether customer has personal loan ('no', 'yes', 'unknown')
7. *contact* - contact communication type ('cellular', 'telephone')
8. *month* - last contact month of year
9. *day_of_week* - last contact day of the week ('mon',...,'fri')
10. *poutcome* - outcome of the previous marketing campaign ('failure', 'nonexistent', 'success')

**Numerical Features:**

1. *age* - age of customer
2. *duration* - last contact duration, in seconds. It is also, important to note that this feature has been stated to highly affect the output target directly. We will therefore, just include it for benchmark purpose but discard it to have a realistic predictive model.
3. *campaign* - number of contacts performed during this campaign and for a specific customer.
4. *pdays* - number of days that passed by after the client was last contacted from a previous campaign. (999 means a customer wan not previously contacted)
5. *previous* - number of contacts performed before this campaign and for this customer.
6. *emp.var.rate* - employment variation rate (quarterly indicator)
7. *cons.price.idx* - consumer price index (monthly indicator)
8. *cons.conf.idx* - consumer confidence index (monthly indicator)
9. *euribor3m* - euribor 3 month rate (daily indicator)
10. *nr.employed* - number of employees (quarterly indicator)

**Target Variable**
* *y* - if the client has subscribed for a term deposit ('yes', 'no')