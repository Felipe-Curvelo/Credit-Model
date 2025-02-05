## Credit Risk Modeling - Python

This is a credit risk model developed in Python. You can download the datasets used to generate the analysis [here](https://drive.google.com/drive/folders/1IM7wfiwvzlngdyyr-L7Dafdk7oXZZBgN?usp=sharing).

Required Packages
- python 3
- numpy
- scipy
- sklearn
- pandas
- matplotlib
- seaborn
- pickle

## About the model

Credit risk models need to answer the question: How much is my risk appetite? This model is no different.

The calculation consists of the following formula:  
$$\text{EL} = \text{PD} \times \text{LGD} \times \text{EAD}$$  

Where:  
EL ⇒ Expected losses, caused by borrower-specific factors and the economic environment.  
PD ⇒ Probability of default - The borrower’s inability to pay their loan in full or on time.  
LGD ⇒ Loss given default - The proportion of the total exposure that cannot be recovered by the lender once a default has occurred 
EAD ⇒ Exposure at default - The total value that a lender is exposed to when a borrower defaults

This model is based on the Basel II framework. Under its guidelines, it considers EL (Expected Loss), UL (Unexpected Loss), and SL (Specialized Lending). These terms are used in the Internal Ratings-Based (IRB) approach to calculate risk-weighted assets (RWAs) and capital requirements.

![loss distribution](images/P_Loss.png)

## Statistic model used:  
For this model, I chose to use logistic regression, as there is widely available documentation on how to implement it in Python, and it is the most used model in the industry to calculate default.

Under logistic regression, the probability of an event can be represented as the exponential of a linear combination of independent variables and coefficients, divided by 1 plus the same exponential.

The equation looks like this:
![logistic regression](images/logistic.png)

Where:  
𝑃(𝑌=1∣𝑋) is the probability of the event occurring.  
𝛽<sub>0	</sub> is the intercept.  
𝛽<sub>1</sub> ,𝛽<sub>2</sub> ,...𝛽<sub>n</sub> are the coefficients for the independent variables  

In other words, the probability of event occurring divided by the probability of event not occurring is equal to the exponential of odds.

Is this material you will find:
- Data cleansing
- Variables selection
- Chart analysis
- Statistical analysis
- Variable treatment
- Scorecard
- Models calculation


