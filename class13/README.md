# 432 Class 13: 2025-02-25

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
13 | 2025-02-25 | **[Slides 13](https://thomaselove.github.io/432-slides-2025/slides13.html)** | **[Word 13](https://thomaselove.github.io/432-slides-2025/slides13w.docx)** | **[Code 13](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides13.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. When you run a model for Project A, especially a logistic regression model ...
    - If you see huge coefficients or huge confidence interval values, try reducing the amount of non-linearity in the model.
    - When you select a model at the end, don't select one with crazy huge coefficients or confidence interval end points.
    - It's fine to (in Project A) write something like "Although the Spearman rho-squared plot caused me at first to run this set of non-linear terms, as you can see, the coefficients exploded on me, so instead I ran a model with a different set of non-linear terms, where the coefficients are more in control" and then work with that second model.
    - If coefficients explode on you in models you fit before March 6, contact Dr. Love or the TAs in office hours (TAs) or via email (to Dr Love) with your entire Quarto file, your data file (the tidy Rds is OK so long as we can use it to get your results) and a screen shot showing the problem you are having so that we can try to replicate and then diagnose the problem. Otherwise, you'll have to wait until after we return from spring break.
  
--- 

**Project A**: Suppose you've done everything in Sections 8 and 9 of the [Project A Demo](https://thomaselove.github.io/432-2025/432_projectA_demo.html) to the best of your ability, and you're wondering what else you might consider doing?

- Doing everything correctly in Sections 8 and 9 is great, and a good step towards an excellent grade.
- For linear regression, you are welcome to include **either** choice 1 or choice 2 below. Don't do both.
- For logistic regression, you are welcome to include **either** choice 3 or choice 4 below. Don't do both.

1. **If** in your linear regression you have **more than 5% of cases** with missing data in your predictors, create a new section 8.9 called "Comparing Imputation Strategies", where you show the simple imputation model, and then either:
    - fit an appropriate model using multiple imputation (with an appropriate number of imputations) and the **mice** package, then compare the coefficients and R-square values between the single imputation fit and the multiple imputation fit, **or**
    - use the `aregImpute()` function to fit an appropriate multiply imputed set of results, then compare the coefficients and R-square values between the single imputation fit and the multiple imputation fit.
2. After your linear regression modeling, create a new section 8.9 called "A New Model C" where you do the following:
    - use the best subsets approach to identify another possible model (besides Model A and Model B) using a subset of your predictors, which you'll call Model C, then
    - show a plot of the posterior predictive check for your new model C, and compare it to your previous models A and B, then
    - compare all three of those models using a plot which compares performance on common metrics (root mean squared error, AIC, BIC, multiple R-square and adjusted R-square) across your sample, and interpret the results, then finally
    - perform 5-fold cross-validation for each of your models to compare R-square and the square root of the mean squared error, and interpret those results.
3. **If** in your logistic regression you have **more than 5% of cases** with missing data in your predictors, create a new section 9.9 called "Comparing Imputation Strategies", where you show the simple imputation model, and then either:
    - fit an appropriate model using multiple imputation (with an appropriate number of imputations) and the **mice** package, and compare the coefficients (expressed as odds ratios) and the C statistic values between the single imputation fit and the multiple imputation fit, **or**
    - use the `aregImpute()` function to fit an appropriate multiply imputed set of results, then compare the coefficients and C statistic values between the single imputation fit and the multiple imputation fit.
4. After your logistic regression modeling, create a new section 9.9 called "A New Model X" where you do the following:
    - use the best subsets approach to identify another possible model (besides Model Y and Model Z) using a subset of your predictors, which you'll call Model X, then
    - show a plot of the posterior predictive check for your new model X, and compare it to your previous models Y and Z, then
    - compare all three of those models using a plot which compares performance on common metrics (root mean squared error, AIC, BIC and Tjur's R-squared) across your sample, and interpret the result, then finally
    - perform 5-fold cross-validation for each of your models to compare C statistics, and interpret the results.

---

## Today in "How To Be A Modern Scientist"

### On Scientific Code

- Organize and document your code and the importance of literate programming
- Include links to your code in your publications
- Post your code to a public repository

### On Your Online Identity

- Have a standard handle so it's easier for people to find you
- Use commercial platforms
- Don't be a jerk
