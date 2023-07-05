# Marketing-Analysis
Data analysis project about marketing analysis.

# Introduction

We were task to optimize a marketing campaign in order to gain a maximum profit. The company is in need of a new strategy to increase their profit and one of it ways is to launch a new product. Based on the data, we were task to maximize this marketing campaign for a new product to maximize the company profit. 

To tackle this problem we will use $\textit{predictive analysis}$ based on the customer behaviour. We will also try to analyze the customer characteristics to gain insight which customer will accept the product.

# Data Overview
In the dataset that were given, there are a total of 28 columns and 2240 rows.
The columns consist of:
1. Customer Profiles
2. Product preferences
3. Campaign successes/failures
4. Channel performance

The detailed information of the columns are available at 'dictionary.png'. 

# Findings
![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/c13749ae-d967-46f0-ba9d-8be7b8ff9982)
![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/ca579a58-b0ac-4d3e-b08c-a84d46fc7f49)
![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/1db8948b-c146-4fb8-aa1d-7b6bf99eb4d3)
![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/896298ac-f608-4539-a7fa-08eb29d532b5)

Based on the barplot above, there are things that we can take:
1. A person with PhD degree has a higher chance to take the offer, while a person with Basic degree has a lower chance to take the offer.
2. A widow has a higher chance to take the offer.
3. The longer the customer has been a member, the higher the chance they will take the offer.
4. 'AcceptedCmp5','AcceptedCmp3','AcceptedCmp1' has a high positive correlation out of AcceptedCmp 1,2,3,4,5.
5. 'NumCatalogProducts', 'MntMeatProducts', 'MntWines' also have a high positive correlation.
6. 'Recency','Cust_JoinDt', 'Teenhome' has a high negative correlation.

# Model Performance

The model we are using for this problem is RandomForestClassifier. The model managed to get an accuracy of 0.89 with classification report such as:

![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/3311e92a-613e-48e1-8787-8fe33e4812a9)

with the feature that we are using and their importances are:
![image](https://github.com/sftyo/Marketing-Analysis/assets/107123925/a87d994b-4ed0-4722-9f12-217571732ad2)

based on the barplot above, 'Recency' , 'TotalAmntSpnt', 'MntWines' are the three most importance feature for the model to perform.

# Conclusion
Based on the findings and model performance, in order to predict our customer acceptance to our offer, the features that has a high correlation and features that is important for the model need to be dig alot deeper. 
Also, there are some features that have not been touch much, such as 'Country' feature.

That means we still can improve the performance of the model, that is:
1. Dig deeper on the 'Country' feature (Which country that will accept the offer? or to be more general we can make Which region will accept our offer?)
2. Which product is a lot more successful?
3. Best/Worse channels?

# Thank You






