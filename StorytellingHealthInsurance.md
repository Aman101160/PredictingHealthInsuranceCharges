# Health Insurance Cost Prediction System 

![image.png](attachment:image.png)

If there is one thing to know about the United States Health System,it is that is constantly being regulated.It has spilled onto the political arena where one side is arguing for deregulation and the other arguing further regulation.The U.S. Health System is a mix of public and private,for-profit and non-profit insurers and healthcare providers.The United States Federal Government provides funding for programs.There is Medicare which is for adults age 65 and older and some people with disabilities as well as for various programs for veterans and low-income people,including Medicaid and the Children’s Health Insurance Program. In 2018, nearly 92 percent of the population was estimated to have coverage leaving 27.5 million people uninsured. With the dataset provided, I analyze it as well as perform models to compare and contrast the costs among regions as well as see how much the factors impact the costs.   

# 1. Data

For the data, the factors in determining the costs for insurance are age, sex, bmi, children, smoker, and region. 

- https://www.kaggle.com/annetxu/health-insurance-cost-prediction

- https://www.commonwealthfund.org/international-health-policy-center/countries/united-states    

# 2. Method

There are multiple methods involved:

-Linear Regression: As I was conducting Exploratory Data Analysis, Regression had to be utilizing when fitting the column variables. It is also used when building another model that uses both continuous and categorical variables.I also applied the predict to the prediction.
    
-Train_Test_Split: I split the numerical and categorical variables while picking 60% of the data for the training set. Before, I build a random number generator. I separate the variables from the target variable which is charges to determine charges. I create dummy variables so I am able to utilize the categorical varibles turning them into numerical.
    
-Preprocessing.OneHotEncoder: All the variable encoder is doing here is converting our categorical 
variables to binary.We have three categories, which have two, two, and 
four possible entries. The encoder uses one binary for each possible
response in each category; for example, 'sex' has two columns: one that
says yes or no to the individual having 'male' in 'sex', and one that 
says yes or no to the individual having 'female' in 'sex'. This makes 
the third category, where we have four possible categories, directly
comparable to the others. 

# 3. EDA

EDA report: https://github.com/Aman101160/Data-Science-Portfolio/blob/master/Predicting_Health_Insurance_Costs.ipynb

The scatterplot of the age and charges seems to show a positive correlation as the older a person gets, their insurance policy price increases.

![image.png](attachment:image.png)

# 4. PreProcessing and Training Data Development¶

https://github.com/Aman101160/Data-Science-Portfolio/blob/master/InsurCostPredPreProcessing%26TrainingDataDevelopment.ipynb

With the plot, I took the linear regression and subtracted from the traing set for the target variable charges.

![image.png](attachment:image.png)


The scatterplot for the BMI and Age with the hue as the target variable and the data being insurance excluding the charges column variable.

![image.png](attachment:image.png)

The boxplot for the BMI and Age with the data the same as before.

![image.png](attachment:image.png)

# Future Improvements 

- If there were improvements I would make, it should start with the data where we should be collecting more information for more column variables as I feel it was not enough. There still seems to be some vagueness.

- There should be column variables like whether someone has pre-existing conditions or there kids do.

- There should also be a thorough examination of the policy plans especially with regards to the regions.
