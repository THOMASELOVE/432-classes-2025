# An Outline of Slides in 432 Class 08

Slides | Topic(s)
:------: | :------------------------------------------------------------------------------
1-3 | Title, Agenda, R Setup
4-14 | Introducing and Cleaning the mov25 data
15-16 | mov25 Variable Descriptions and `data_codebook()` results
17-18 | Data listing, Discussion of splitting the sample
19 | `love4`: Four More Movies (outside of mov25)
20 | Converting from log odds to odds to probabilities and vice versa
21 | Initial guess as to associations of predictors with outcome
22 | Table One (with `CreateTableOne()` from the `tableone` package)
23 | What Five Models Will We Fit Today?
24-29 | Fitting `fit1` with `glm()` and `lrm()`, plus `model_performance()`, `performance_roc()`, `model_parameters()` and `tidy()`, and the resulting equation
30 | ROC curve analysis with plot for `fit1`
31-34 | Description and values of key pseudo-R-square measures
35-37 | Effect Sizes, tabulated and plotted, as well as Prediction plots
38-41 | Calibration Plot and Hosmer-Lemeshow test
42 | `fit1` Nomogram
43-45 | Predictions for the `love4` movies
46-48 | Building a Confusion Matrix, Picking an "optimal" decision rule, PCP
49-52 | Checking Model Assumptions
53 | Analysis of Deviance results
54 | Bootstrap Validation of key summaries
55 | Cross-Validation of C statistic
56-97 | Model `fit2`, including (starting with slide 78) a more detailed look at checking assumptions in logistic regression models
98-132 | Model `fit3`, including (starting with slide 99) a predictor subset search for models that produce the best AIC 
133-167 | Model `fit4`, including (starting with slide 135) a predictor subset search for models that produce the best BIC
168-204 | Model `fit5`, including (starting with slide 169) a look at including some non-linear terms in the model
205-213 | Comparing our five models in our original sample (`mov25`)
214-222 | Assessing fit in a test sample of 50 more movies
223 | Things that **aren't** in this example
224 | Session Information
