# An Outline of Slides in 432 Class 10

- Don't forget about the similar [outline for the logistic regression slides from Class 8](https://github.com/THOMASELOVE/432-classes-2025/blob/main/class08/outline.md).
- Don't miss the [index of R functions and key statistical ideas](#index-of-r-functions-and-key-statistical-ideas) covered in these slides, too...

## Topics covered in each slide group

Slides | Topic(s)
:------: | :------------------------------------------------------------------------------
1-3 | Title, Agenda, R Setup
4-7 | Introducing the happy data
8-12 | Cleaning the happy data and `data_codebook()` results
13 | Modeling Objective
14-18 | Data checking and outcome summaries
19 | Single imputation via the **mice** package
20-21 | Partitioning into training and test samples
22-27 | Considering transformation of the outcome
28-29 | Fitting `fit4`: 11 main effects
30-35 | Fitting `fit5`: adding non-linear terms to `fit4`
36 | Fitting `fit2`: two predictors + interaction
37-39 | Using "best subsets" to select predictors
40-41 | Fitting `fit1`: three main effects
42-43 | Fitting `fit3`: 5 predictors + non-linearity
44 | Listing our five models (variables, non-linearity, degrees of freedom)
45-76 | Estimation of Coefficients and interpreting effect size
77-82 | Nomograms for our five models
83-105 | ANOVA tables and eta-squared measures
106-113 | Assessing Model Performance in the training sample
114-119 | Comparing Performance and Error Summaries in the training sample
120-160 | Checking Model Assumptions, Calibration
161-167 | Making Predictions
168-171 | Predicting into our Test Sample
172-178 | Bootstrap Validation of R-square and MSE for each model
179-184 | Cross-Validation approaches for summary statistics
185-197 | Multiple imputation with the **mice** package
198-244 | Multiple imputation for an `ols()` fit with `aregImpute()`
245-250 | Comparisons and Conclusions across all 5 models
251 | Other Examples to Consult
252 | Session Information

## Index of R functions and key statistical ideas

Slides | Topic(s)
:--------------: | :------------------------------------------------------------------------------
85-89, 91-93, 95-97, 99-101, 103-105 | ANOVA table and eta-squared and partial eta-squared
166-167 | `augment()` to add fitted values, residuals and other things from a model, from **broom**
22-27 | Box-Cox plot for potential outcome transformation and checking potential impact
127-129, 136, 144, 152, 160, 247 | calibration plots and checks in linear models
4 | cleaning names with `clean_names()` from **janitor**
4 | changing character variables to factors
14 | check variable types with `glimpse()`
121-126, 131-135, 139-143, 147-151, 155-159 | checking assumptions of linear models
9 | collapsing a factor to fewer levels with `fct_lump_n()` from **forcats**
115-118 | plot to compare performance across models in the training sample
16, 20 | counting distinct (unique) values in a variable
10 | creating categories from a quantitative variable with `categorize()`
179-184 | cross-validation of an `lm()` fit with a holdout sample or 5-fold
12 | `data_codebook()`
52-53, 63-64, 67-68, 71-72, 75-76, 204-205, 213-214, 222-223, 231-232, 240-241  | Effect Size plots and tabular summaries after an `ols()` fit
119, 246 | error summaries in the training sample
169-171, 250 | error summaries in a test sample
30, 35-36, 41, 43 | fitting linear models with `lm()`
30, 35-36, 41, 43 | fitting linear models with `ols()`
109-113 | `glance()` to specify summary measures of fit quality from **broom**
18 | identifying the largest and smallest values in a variable by an identifier
35 | including a polynomial term in a linear model
35, 43 | including a restricted cubic spline term in a linear model
35-36, 43 | including an interaction (product) term in a linear model
163-166 | making predictions, with prediction and confidence intervals
15 | missingness summaries from **naniar**
46, 49, 54, 60, 65, 69, 73, 121, 130, 138, 146, 154 | `model_parameters()` to specify linear model coefficients
108, 110-113, 121, 130, 137, 145, 153, 246 | `model_performance()` to summarize quality of fit for a linear model
16 | most common value in a variable
200-203, 209-212, 218-221, 227-230, 236-239  | multiple imputation in an `ols()` fit with `aregImpute()`
186-197 | multiple imputation with **mice**
78-82, 207, 216, 225, 234, 243 | nomogram for a linear model
11, 48, 53, 61 | numerical summaries across levels of a predictor or for multiple variables with `df_stats()`
17 | numerical summaries with `Hmisc::describe()` and `mosaic::favstats()`
37-39, 42 | `ols_step_best_subset()` from **olsrr** to search for best subsets of predictors
21 | partitioning a sample with `data_partition()`
51, 62, 66, 70, 74, 206, 215, 224, 233, 242 | Prediction plots via `ggplot(Predict(...))`
19 | single imputation using **mice**
31-34, 42 | spending degrees of freedom on non-linearity and the Spearman rho-squared plot
50 | `tidy()` to specify coefficients from **broom**
173-177, 208, 217, 226, 235, 244, 249 | validating R-square and MSE with `validate()` for an `ols()` fit
