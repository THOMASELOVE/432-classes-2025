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

### Project A: Extra Analytic Sections?

Suppose you've done everything in Sections 8 and 9 of the [Project A Demonstration Project](https://thomaselove.github.io/432-2025/432_projectA_demo.html) to the best of your ability, and you're wondering what else you might consider doing?

I have added two new "Extra" sections to the Project A instructions, which answer this question. They are:

- [EXTRA (potential section 8.9)](https://thomaselove.github.io/432-2025/projA.html#extra-potential-section-8.9), which provides two options for amplifying your linear regression work. You are allowed to select at most one of these two options.
    - Option 1 is appropriate if you have more than 5% of your cases with missing data on predictors in your Model A, and involves doing multiple imputation and some related things.
    - Option 2 involves using best subsets to fit a third model, then completing a series of comparisons across your three models.
- [EXTRA (potential section 9.7)](https://thomaselove.github.io/432-2025/projA.html#extra-potential-section-9.7), which provides two options for amplifying your logistic regression work. You are allowed to select at most one of these two options.
    - Option 1 is appropriate if you have more than 5% of your cases with missing data on predictors in your Model Y, and involves doing multiple imputation and some related things.
    - Option 2 involves using best subsets to fit a third model, then completing a series of comparisons across your three models.

#### Three key points to emphasize (also made in the instructions):

- The required elements of Section 8 (Linear Regression Analysis) should produce sections 8.1 through 8.8, as shown in the [Project A Demonstration Project](https://thomaselove.github.io/432-2025/432_projectA_demo.html). If you have meaningful problems in sections 8.1 - 8.8, I won't even look at your section 8.9. Similarly, the required elements of Section 9 (Logistic Regression Analysis) should produce sections 9.1 - 9.6, as shown in the [Project A Demonstration Project](https://thomaselove.github.io/432-2025/432_projectA_demo.html). If you have meaningful problems in sections 9.1 - 9.6, I won't even look at your section 9.7.
- I provide two alternatives for section 8.9. You may choose **exactly one** of those two alternatives for your portfolio. Similarly, I provide two alternatives for section 9.7. Again, pick at most one of those to present in your portfolio. In each case, do not present both alternatives in your portfolio, or I will ignore both of them. 
- Although completing section 8.9 and/or section 9.7 can only help your grade, this is completely optional, and is not required to get an A grade on the Project. 

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
