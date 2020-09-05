# Zimnat Insurance Recommendation Challenge - Zindi
**Client: Zimnat Insurance**
Insurance companies pool and spread risk across a broad customer base. This works best where the population to be insured is diverse and large. Understanding the varied insurance needs of a population, and matching them to appropriate products offered by insurance companies, makes insurance more effective and makes insurance companies more successful. At the heart of this, understanding the consumer of insurance products helps insurance companies refine, diversify, and market their product offerigs. Increased data collection and improved data science tools offer the chance to greatly improve this understanding.

Zimnat Insurance wants a ML model to use customer data to predict which kinds of insurance products to recommend to customers. We will therefore, leverage data and ML methods to improve market outcomes for the company by matching consumer needs with product offerings in the Zimbabwean Insurance market.

Our data is of nearly 40,000 customers who have purchased two or more insurance products from Zimnat. The data can be accessed [here](https://zindi.africa/competitions/zimnat-insurance-recommendation-challenge/data). The data is divided into Train and Test sets. For both sets, each row corresponds to a customer, assigned a unique ID('ID'). Each set also has customer related information ('join_data', 'sex','marital_status', 'birth_year', 'occupation_code', 'occupation_category_code'). The branch code of the customer ('branch_code') is also provided. The rest of the data corresponds to the 21 products on offer.

For each product that a customer has, there is 1 in the column and 0 if the customer doesn't have that product. This is true for both train and test set except that for each customer, ONE product has been removed in the test set, i.e. the 1 has been replaced with a 0. The goal is to predict this missing product.

To come up with a ML model we first need to understand the data we are working with. This notebook will go through the exploratory data analysis and data pre-processing to prepare our data for model training.

The data exploration codes are all included in the .ipynb file as a jupyter notebook file.