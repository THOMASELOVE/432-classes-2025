# An Outline of Slides in 432 Class 08

Don't miss the [index of R functions and key statistical ideas](#index-of-r-functions-and-key-statistical-ideas) covered in these slides, too...

## Topics covered in each slide group

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

## Index of R functions and key statistical ideas

Slides | Topic(s)
:------: | :------------------------------------------------------------------------------
53, 95, 130, 165, 202 | analysis of deviance
43-45, 72-74, 117-119, 152-154, 189-191, 217-222 | `augment()` from the **broom** package to make predictions into new data and build CIs
38-40, 69, 114, 149, 186, 212 | calibration and the calibration plot
5 | changing all character variables to factors
17 | checking that ID variable values are unique
49-52, 91-94, 126-129, 161-164, 198-201 | checking logistic regression model assumptions with `check_model()` from easystats
80-90, 123-125, 158-160, 195-197 | checking six key assumptions of logistic regression and component + residual plots
206-208 | comparing parameters (coefficients) of various model fits
65, 110, 145, 182, 209 | comparing performance on model indices in the model training sample
47, 76, 121, 156, 193, 211 | confusion matrix - building using the **caret** package, and interpreting
46, 75, 120, 155, 192, 211 | confusion matrix - optimal cutpoint for our decision rule with `cutpointr()`
55, 97, 132, 167, 204, 212 | cross-validation of the C statistic from a `glm()` fit
8 | creating a 1/0 factor from a logical statement
22 | creating a Table 1 with `CreateTableOne` from the **tableone** package
16 | `data_codebook()` to look at ranges, missingness and categorical values
35-36, 66-67. 111-112, 146-147, 183-184 | effect sizes (table and plot) from an `lrm()` fit
10 | `fct_lump()` to collapse a categorical variable
30 | glue together text and R code in a graph label from the **glue** package
41, 70, 115, 150, 187, 212 | Hosmer-Lemeshow test for assessing calibration
26, 58, 102, 137, 175 | `model_parameters()` from easystats
25, 57, 101, 136, 174 | `model_performance()` from easystats
42, 71, 116, 151, 188 | Nomogram after `lrm()` fit
18 | observations needed to fit a logistic regression model well
48, 77, 122, 157, 194, 212 | percentage of correct predictions (PCP) using the Herron method
25, 57, 101, 136, 173, 210 | `performance_roc()` from easystats
30, 62-63, 106-107, 141-142, 178-179 | Plot ROC curve
37, 68, 113, 148, 185 | Prediction Plots from `ggplot(Predict(lrmmodel))`
99-100, 134-135 | Predictor Subset Searching (Best Subsets) with the **bestglm** package
31-34, 64, 108-109, 143-144, 180-181, 210 | Pseudo-$R^2$ measures and interpretations (Nagelkerke, Tjur, McFadden)
2 | R packages used in the **mov25** example
5 | reading in data from an Excel sheet
20 | relation of logit (log odds) to odds to probability
169-172 | Spearman rho-squared plot to identify potential candidates for non-linear terms
99 | splitting a factor into indicator variables using the **cobalt** package
210-212 | summary statistics worthy of comparison after all five models are fit
26 | `tidy()` from **broom**
54, 96, 131, 166, 203, 210, 212 | `validate()` key summaries (C, Nagelkerke R-square, and Brier score) after `lrm()`
217-222 | test sample summaries
