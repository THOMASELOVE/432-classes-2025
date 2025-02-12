# Project A Plan Comments from Dr. Love

## Project Plans for which I need to see a full revision by Monday 2025-02-17 at 9 AM

Your Next Step: Read the rest of this page, review my comments on our Shared Drive in the Project A Plan Feedback document, then build and submit a fully revised Project A Plan to Canvas (the Project A Plan REVISION assignment) no later than **Monday 2025-02-17 at 9 AM**.

- Grade on Project A Plan: To be determined after the revision is reviewed by Dr. Love

Group | Investigators | Reason
:---: | :----------------------: | :---------------
11 | Gina Lin | New pull of data, to focus on 2017 only.
20 | Arya Patel | New sample and new linear model.
21 | Tom Kupferer | New data set required.
23 | Reilly Burhanna and Jose Diz Ferre | New sample and new linear model.
28 | Leia George | New sample and new linear and logistic models.
29 | Kelao Neumbo | New sample and new linear and logistic models.
38 | Anika Krishna | New logistic model needed that uses original data, or new data.
39 | Morgan McLoughlin | New linear and logistic models.
40 | Manu Bulusu | New linear model.

## Project Plans where a new model (linear or logistic or both) is required, but where Dr. Love doesn't need a revision.

Your Next Step: Read the rest of this page, review my comments on our Shared Drive in the Project A Plan Feedback document, then make my suggested and any other changes while building your Project A Portfolio, and develop the new model or new sample (which might require a new outcome or new predictors or both - see my comments) as listed below. Regardless, read and heed my comments, but your plan is accepted.

- Grade on Project A Plan: 26 out of 30.

Group | Investigators | Reason
:---: | :----------------------: | :---------------
1 | Jeff Lambe and Tatchaporn Ongphichetmetha | New linear model needed
5 | Dana Jian | New linear model needed
6 | Nihit Mehta | New linear model needed
12 | Graham Stockdale | New linear model needed
14 | Zuhair Khan | Larger sample of counties needed
16 | Mahsa Sheikh and Tatiana Dombrovski | New linear model needed
22 | Toni Shoyinka | Larger sample of institutions needed
25 | Nick Nazak and Rebecca Stinson | New sample if possible, new linear model
26 | Weiyun Liang | New linear model needed
30 | Shraddha Dumawat | New linear model needed
31 | Ajay Mahenthiran | New linear model needed
32 | Veda Machiraju | New sample if possible, new linear model

## Project A Plans where Dr. Love doesn't need to see a revision, and where the plans for the models seem OK at present.

Your Next Step: Read the rest of this page, review my comments on our Shared Drive in the Project A Plan Feedback document, then make my suggested changes as part of your Project A Portfolio. This may include developing a new linear or logistic outcome, or predictor set, but you'll have to look at my comments. Your Project A plan is accepted.

- Grade on Project A Plan: 27 out of 30 if accomplished in first version, 25 out of 30 if one revision was required.

Group | Investigator(s) | Group | Investigator(s) | Group | Investigator(s)
:---: | :----------------------: | :---: | :----------------------: | :---: | :----------------------:
2 | Spancer Zhou | 3 | JiaWei Yu | 4 | Olivia Lindberg
7 | Medhat Farwati and Mohammad Nasirpour | 8 | Lingzhu Shen | 9 | Saar Anis 
10 | Katherine Papahadjopoulos | 13 | Haley Altadonna | 15 | Harshita Kumar and Kartik Lakhotiiya 
17 | Dalí Nemecio | 18 | Monique Katsuki and Trisha Lal | 19 | Kelly Bowen 
24 | Debbie Seifert | 27 | Alayna Rowell and Feriel Presswalla | 33 | Megan Zelinsky 
34 | Carly DaCosta and Gabrielle Davis | 35 | Ben Hauk | 36 | Adam Salem 
37 | Brooke Bhattacharya

## New Requirements for the Portfolio that apply to everyone

As of 2025-02-11 at Noon, the posted version of:

- the [Project A demo project](https://thomaselove.github.io/432-2025/432_projectA_demo.html) incorporates all of these new requirements for Sections 5-7,
- the [Project A instructions](https://thomaselove.github.io/432-2025/projA.html) incorporate all of these new requirements for Sections 5-7, and all of the general comments listed below, too.
- the [Project A plan template](https://github.com/THOMASELOVE/432-data/blob/master/data/432_projectA_plan_template.qmd) and the [Project A portfolio template](https://github.com/THOMASELOVE/432-data/blob/master/data/432_projectA_portfolio_template.qmd) incorporate these requirements, as well.

1. In **Section 5** of your portfolio (or your revised Plan, if necessary), I am now requiring you to include a table of variables and descriptions, **plus** the `data_codebook()` results. You can add other things, as well, if they are useful to you. Most people already did this, but I want to be sure everyone does.
2. In **Section 6** of your portfolio (or your revised Plan, if necessary), I'm adding the following requirements:
    - Section 6 should begin by filtering the data to the observations with complete data on the quantitative outcome (for the linear model.) This might be necessary if some of the rows in your tibble have complete data on one outcome (binary) but not the other (quantitative). Obviously, if your data are already complete on this outcome, there's no need to re-filter.
    - As part of section 6.2, I want to see the following three things for your linear outcome, in each case, restricting the data to the observations with complete data on that outcome.
        1. plots - at least a histogram and Normal Q-Q plot of the linear outcome, built using `ggplot2` and `patchwork`.
        2. numerical summaries - the results of both `describe()` (from the **Hmisc** package) and `favstats()` (from the **mosaic** package) for the linear outcome.
        3. a `tabyl()` (from the **janitor** package) of the most common values of your outcome, along with the fraction of all cases with complete data on that outcome that have that particular value, so that you can verify that no value occurs in more than 10% of your complete observations.
    - In a new section 6.3.2, I want to see a missingness summary including `miss_var_summary()` and `miss_case_table()` (from the **naniar** package) across all variables in the codebook that play a role in your planned linear regression model **after** filtering to the cases with complete data on your linear outcome. I'm hoping that you'll have complete data for all predictors on more than 60% of your observations, and that you won't be missing more than 20% of any individual predictor.
3. In **Section 7** of your portfolio (or your revised Plan, if necessary), I'm adding the following requirements:
    - Section 7 should begin by filtering the data to the observations with complete data on the binary outcome (for the logistic model.) This might be necessary if some of the rows in your tibble have complete data on one outcome (quantitative) but not the other (binary). Obviously, if your data are already complete on this outcome, there's no need to re-filter.
    - As part of section 7.2, I want to see a `tabyl()` (again from the **janitor** package) of the values of your binary outcome, after restricting the data to the observations with complete data on your primary outcome.
    - In a new section 7.3.2, I want to see a missingness summary including `miss_var_summary()` and `miss_case_table()` (from the **naniar** package) across all variables in the codebook that play a role in your planned logistic regression model **after** filtering to the cases with complete data on your binary outcome. I'm hoping that you'll have complete data for all predictors on more than 60% of your observations, and that you won't be missing more than 20% of any individual predictor.

## General Comments that apply to everyone

1. **Roles of Variables in Section 5** All variables in your tidy data set, and in your codebook in Section 5 should fall into one of four roles. Don't include other things in your tidy data set.
    - **identifiers**: variables that identify the subjects in your data, and these should be labeled as **Identifier** in the variable descriptions part of Section 5.
    - **outcomes** for either of your models, and these should be labeled as **Outcome (linear)** or **Outcome (logistic)** in the variable descriptions part of Section 5.
    - **predictors** for either of your models, and these should be labeled as either **Predictor** or **Input** in the variable descriptions part of Section 5.
    - **other** variables that you needed to use to create something in the previous three groups. These should not be labeled as predictors or outcomes in Section 5.
2. **Labels**: Zap away any variable labels in section 3 using `zap_label()` from the **haven** package or a similar alternative. I'm not a fan of labels in R data sets for variables, as they make the results of many plots, tables and things like `data_codebook()` much harder to read.
3. **Missingness**: If you are considering a predictor for either your linear or logistic regression model which has 20% or more missing values among the observations where you have complete data on the relevant outcome, then either (a) look elsewhere for a more informative predictor, or (b) change your sampling strategy to require complete cases on that variable, as well, if possible.
4. I**Names**: I want to discourage you from using data set names, variable names and especially category level names that are long (more than 8-10 characters) if you can avoid it. You want to be clear, certainly, but long names are (a) harder to type and (b) harder to see in plots and tables.
    - More than 8 characters in a category level's name will make a lot of plotting very irritating down the line, especially in something like a nomogram or prediction plot.
    - Don't use spaces in the names of variables or the names of categories - separate words with underscores.
5. **Labels for a binary variable**: Never use 1 and 2 as the levels of a binary variable, like sex = 1 for M and 2 for F, or anything like that. Always use 1 and 0, or actual names like "M" and "F" as the levels.
6. **Order your multi-category variables**: Be sure that if you have a multi-categorical variable with a natural order of levels (like Low, Medium, High, or Excellent, Very Good, Good, Fair, Poor or Strongly agree, Agree, Neither Agree nor Disagree, Disagree, Strongly Disagree) be sure that the data_codebook() results you show in Section 5 show that order. If you need to fix this, the place to fix it is in Section 3.
7. **Creating categories from numbers**: If you are using a cutpoint to split a quantitative measure into categories, be sure to include in the variable description part of Section 5 exactly what that cutoff (or set of cutoffs') value was (for example, "values above the mean" isn't sufficient, "values above 45.67 (the mean of the data)" is a sufficient response.)
8. **Logistic Regression Outcome**: If your logistic regression outcome cannot be expressed in the form of a yes/no question, coded as 1 = yes and 0 = no, and if the name of that variable doesn't tell us what 1 means, then adjust your setup accordingly until this is true.
    - For example, don't use "Active / Inactive" for a `status` variable, instead use `active` = 1 or 0 for the same information.
    - This is because if you use a factor in R for your outcome, the logistic regression model will not necessarily choose the result (Yes instead of No, 1 instead of 0) that you're looking for unless you actually use 0 and 1 or No and Yes for the levels, and 0 and 1 have fewer characters.
    - If your outcome was "High / Low" it will choose Low because it is the second one alphabetically!
    - Also, if you use 1 and 0 as your levels, the prediction process I have described in slides 8 and in the support1000 example will work, every time. If you do something else, it might not.
9. Use **association** instead of *correlation*, basically always, unless you are referring specifically to a correlation coefficient.
