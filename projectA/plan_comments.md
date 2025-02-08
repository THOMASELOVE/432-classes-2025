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

1. I want to discourage you from using data set names, variable names and especially category level names that are long (more than perhaps 10 characters) if you can avoid it. You want to be clear, certainly, but long names are (a) harder to type and (b) harder to see in plots and tables.
2. I'm also not a fan of labels in R data sets for variables, as they make the results of many plots, tables and things like `data_codebook()` much harder to read.
