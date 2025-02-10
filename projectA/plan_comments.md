# Project A Plan Comments from Dr. Love

**If you come across this, ignore it until Dr. Love has made final plans, which should be Monday 2025-02-10. Thanks.**

## New Requirements for the Portfolio?

1. In your portfolio, I'm adding the following requirements and I will change the template accordingly:
    - Section 6 should begin by filtering the data to the observations with complete data on the quantitative outcome (for the linear model.)
    - In section 6.2, I want to see the following three things for your linear outcome, in each case, restricting the data to the observations with complete data on that outcome.
        1. plots - at least a histogram and Normal Q-Q plot of the linear outcome, built using `ggplot2` and `patchwork`.
        2. numerical summaries - the results of both `Hmisc::describe()` and `mosaic::favstats()` for the linear outcome.
        3. a `tabyl()` (from the **janitor** package) of the most common values of your outcome, along with the fraction of all cases with complete data on that outcome that have that particular value, so that you can verify that no value occurs in more than 10% of your complete observations.
    - In a new section 6.3, I want to see a missingness summary including `n_miss`, `miss_var_summary()` and `miss_case_table()` across all variables in the codebook that play a role in your planned linear regression model **after** filtering to the cases with complete data on your linear outcome.
    - Section 7 should begin by filtering the data to the observations with complete data on the binary outcome (for the logistic model.)
    - In section 7.2, I want to see a a `tabyl()` (again from the **janitor** package) of the values of your binary outcome, after restricting the data to the observations with complete data on your primary outcome.
    - In a new section 7.3, I want to see a missingness summary including `n_miss`, `miss_var_summary()` and `miss_case_table()` across all variables in the codebook that play a role in your planned linear regression model **after** filtering to the cases with complete data on your binary outcome.

## General Comments

1. I want to discourage you from using data set names, variable names and especially category level names that are long (more than 8-10 characters) if you can avoid it. You want to be clear, certainly, but long names are (a) harder to type and (b) harder to see in plots and tables.
    - More than 8 characters in a category level's name will make a lot of plotting very irritating down the line, especially in something like a nomogram or prediction plot.
2. I'm also not a fan of labels in R data sets for variables, as they make the results of many plots, tables and things like `data_codebook()` much harder to read.
3. Use **association** instead of *correlation*, basically always, unless you are referring specifically to a correlation coefficient.
4. If your logistic regression outcome cannot be expressed in the form of a yes/no question, coded as 1 = yes and 0 = no, and if the name of that variable doesn't tell us what 1 means, then adjust your setup accordingly until this is true.
    - For example, don't use "Active / Inactive" for a `status` variable, instead use `active` = 1 or 0 for the same information.
    - This is because if you use a factor in R for your outcome, the logistic regression model will not necessarily choose the result (Yes instead of No, 1 instead of 0) that you're looking for unless you actually use 0 and 1 or No and Yes for the levels, and 0 and 1 have fewer characters.
    - If your outcome was "High / Low" it will choose Low because it is the second one alphabetically!
    - Also, if you use 1 and 0 as your levels, the prediction process I have described in slides 8 and in the support1000 example will work, every time. If you do something else, it might not.
