---
{"dg-publish":true,"permalink":"/notes/linear-regression/","tags":["probability","statistics"]}
---

# linear regression
> In case of linear [[Notes/regression\|regression]] the relationship between independent and dependent variables can be drawn as a straight line. Linear regression is all about finding the best straight line in the graph plotted between [[Notes/response variable\|dependent variable]] and [[Notes/explanatory variables\|independent variable]].
linear regression is a [[Notes/supervised learning\|supervised learning]] method, meaning it uses [[labeled data\|labeled data]]-- where the input [[Notes/feature\|features]] and corresponding outputs are known for a subset of data--to predict a quantitative response from one or more [[Notes/explanatory variables\|independent variables]]

This model is then applied to make predictions on new, unknown data.

The purpose of linear regression is to measure the [[correlation\|correlation]] between [[Notes/explanatory variables\|independent]] and [[Notes/response variable\|dependent variables]] by finding the line of best fit that models the relationship under the assumption of [[linearity\|linearity]].


##### applications of linear regression model
- marketing organizations predicting sales revenues based on advertising expenditures across multiple channels
- Buyers and lenders predicting future home prices based on size and square footage, number of bedrooms and bathrooms, age and condition of property, architectural design and lot size
- University admissions officers predicting student performance based on high school GPA's and standardized test scores
- Retailers predicting product demand based on historical sales figures

Although more complex methods can transform data to model nonlinear relationships , linear regression is designed to capture relationships that align well with a straight line through the data

##### equation
The equation for a simple linear regression, where the [[Notes/response variable\|dependent variable]] is regressed against just one [[Notes/explanatory variables\|independent variable]], or [[Notes/explanatory variables\|predictor]], is typically represented as follows:
$$
\gamma=\beta_{0} + \beta_{1}x + \epsilon

$$
where:
- $\gamma$ is the observed [[Notes/response variable\|dependent variable]].
- $x$ is the [[Notes/explanatory variables\|independent variable]]
- $\beta_{0}$ is the [[Notes/intercept\|intercept]], or the value of [[Notes/response variable\|response variable]] when $x$ equals $0$.
- $\beta_{1}$ is the [[Notes/slope\|slope]]/[[Notes/regression coefficient\|regression coefficient]] or the change in the [[Notes/response variable\|response variable]] for every one-unit change in $x$.
- $\epsilon$ is the [[Notes/error term\|error term]], capturing the deviation of the observed values from the [[Notes/regression line\|regression line]]


xwhen making prxedictions the model is often expressed in terms of the predicted value, $\hat{\gamma}$ (`gammahat`), omitting the [[Notes/error term\|error term]]:
$$
\hat{\gamma}=\beta_{0} + \beta_{1}x
$$
