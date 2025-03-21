# 432 Class 13: 2025-02-25

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
13 | 2025-02-25 | **[Slides 13](https://thomaselove.github.io/432-slides-2025/slides13.html)** | **[Word 13](https://thomaselove.github.io/432-slides-2025/slides13w.docx)** | **[Code 13](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides13.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## Announcements

1. Lab 4 grades and feedback are posted to our Shared Drive's Course Grading Roster. The updated Lab 4 answer sketch and rubric (edited a few times since our last class) is also posted to our Shared Drive.
    - Note that some Labs generate a lower distribution of grades than others (for example, the medians for the first four labs have been 44, 46, 39, and 42.) In April, I will account for this (and tell you how I do it) so that each of Labs 1-5 have a similar impact on your grade in the course (remember that your lowest grade among labs 1-5 is dropped.)
2. A reminder that [Lab 5](https://thomaselove.github.io/432-2025/lab5.html) is due at noon tomorrow (Wednesday 2025-02-26) to [Canvas](https://canvas.case.edu). If you are skipping this Lab, let us know via a note posted to [Canvas](https://canvas.case.edu) **before** the deadline.
3. A reasonably complete presentation of code for linear regression (Section 3) and logistic regression (Section 4) is found in the **support1000** example which I have posted to our Shared Drive.
    - Other than fixing any typos we catch (and please let me know on Campuswire if you see any problems), I do not anticipate editing Sections 3 and 4 of this example further this semester. 
4. I have added the `miceafter` and the `nhanesA` packages to [our list of R packages to install](https://thomaselove.github.io/432-2025/software.html#r-packages-to-install).
    - Neither of these packages is critical for either Quiz or any of the Labs.
    - Each might be useful in Project B, and I'm including the `miceafter` package so that I can use a couple of functions from it to eventually do one thing (look at a C statistic after a mice-based multiple imputation for a logistic regression model) in the **support1000** example, but it's not there yet, as I decided not to do it at this time.
5. When you run a logistic regression model for Project A, ...
    - Ignore the coefficient and confidence interval for the intercept after exponentiating your coefficients to look at odds ratios.
    - If you see huge coefficients or huge confidence interval values, especially in model Z, try reducing the amount of non-linearity in the model.
    - When you select a model (Y or Z) at the end, don't select one with crazy huge coefficients or confidence interval end points.
    - It's fine to (in Project A) write something like "Although the Spearman rho-squared plot caused me at first to run this set of non-linear terms, as you can see, the coefficients exploded on me, so instead I ran a model with a different set of non-linear terms, where the coefficients are more in control" and then work with that second model.
    - If coefficients explode on you in models you fit before March 6, contact Dr. Love or the TAs in office hours (TAs) or via email (to Dr Love) with your entire Quarto file, your data file (the tidy Rds is OK so long as we can use it to get your results) and a screen shot showing the problem you are having so that we can try to replicate and then diagnose the problem. Otherwise, you'll have to wait until after we return from spring break for our help.
6. **On Statistical Significance and P-values** These are the two main articles on the subject that I ask people to read (or at least skim) in my courses.
    - [Statistical Inference in the 21st Century: A World Beyond *p* < 0.05](https://amstat.tandfonline.com/toc/utas20/73/sup1) from 2019 in *The American Statistician*
    - The American Statistical Association's 2016 [Statement on p-Values](http://amstat.tandfonline.com/doi/full/10.1080/00031305.2016.1154108): Context, Process and Purpose.
7. Next time, we'll be talking about (among other things) Andrew Gelman and John Carlin's paper [Beyond Power Calculations: Assessing Type S (Sign) and Type M (Magnitude) Errors](https://github.com/THOMASELOVE/432-sources/blob/main/pdf/Gelman_Carlin_2014_Beyond_Power_Calculations.pdf)


---

## References from Today's Slides

Today, we're talking about the fundamentals of power and sample size estimation. Here are some relevant references.

- <https://thomaselove.github.io/431-notes/22-samplesize.html> is a chapter from my "old" 431 notes on Power and Sample Size considerations when comparing means.
- <https://thomaselove.github.io/431-notes/27-power_for_rates.html> provides several examples on Power and Sample Size considertions when comparing proportions.
- [This page](https://easystats.github.io/effectsize/articles/statistical_power.html) for interesting initial thoughts on power and sample size from the easystats framework. Unfortunately, the page hasn't been updated in a while.

More extensive discussions available online include:

- [Sample Size calculations with `pwr`](https://bookdown.org/pdr_higgins/rmrwr/sample-size-calculations-with-pwr.html), which is Chapter 20 from [Reproducible Medical Research with R](https://bookdown.org/pdr_higgins/rmrwr/) by Peter D. R. Higgins
- Some notes on [Sample Size Estimation and Power Analysis](https://rpubs.com/mbounthavong/sample_size_power_analysis_R) by Mark Bounthavong
- Some notes on [Power and Sample Size Simulations in R](https://www.ohsu.edu/sites/default/files/2024-11/OCTRI%20PSS%20Simulations%20in%20R%20Seminar_11.21.24.pdf) (pdf) presented by Robin Baudier
- A YouTube video [How to Calculate Sample Size and Power using R](https://www.youtube.com/watch?v=C5L8QSTzvBA)
- [A Practical Guide to Statistical Power and Sample Size Calculations in R](https://cran.r-project.org/web/packages/pwrss/vignettes/examples.html) by Metin Bulus, which describes results using the `pwrss` package in R, which I haven't used but maybe I should.


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

## Quiz 1 coming Friday

I have posted an early draft of the instructions for Quiz 1 (which also lists the R packages used in the Quiz and provides a little information on three of the data sets I'll provide) to [the Quiz 1 Links page](https://thomaselove.github.io/432-2025/quiz1.html) if you are curious.

- By Friday 2025-02-28 at noon, [the Quiz 1 Links page](https://thomaselove.github.io/432-2025/quiz1.html) will provide:
    - A link to a PDF file containing complete instructions and all of the questions,
    - A link to the Google Form Answer Sheet where you will answer the questions, and
    - Links to download the Data Sets I am providing for you
- Quiz 1 is due Wednesday 2025-03-05 at noon.
    - You can obtain help during the Quiz period by (1) emailing Dr. Love or (2) asking him questions during Class 15, on Tuesday 2025-03-04 from 1 to 2:15 PM. We will not answer questions about Quiz 1 posed in any other way, and that includes Campuswire.
    - If we need to make changes or add hints related to Quiz 1 after it is initially made available to you, Dr. Love will email that information to you and it will also be posted to [the Quiz 1 Links page](https://thomaselove.github.io/432-2025/quiz1.html).

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

## Today's Excerpt from "[Moving to a World Beyond 'p < 0.05'](https://github.com/THOMASELOVE/432-sources/blob/main/pdf/ASA_2019_A_World_Beyond.pdf)"

from **Don't is Not Enough**

If you’re just arriving to the debate, here’s a sampling of what not to do:

- Don't base your conclusions solely on whether an association or effect was found to be “statistically significant” (i.e., the *p* value
passed some arbitrary threshold such as *p* < 0.05).
- Don't believe that an association or effect exists just because it was statistically significant.
- Don't believe that an association or effect is absent just because it was not statistically significant.
- Don't believe that your *p* value gives the probability that chance alone produced the observed association or effect or the probability that your test hypothesis is true.
- Don't conclude anything about scientific or practical importance based on statistical significance (or lack thereof).


