# 432 Class 09: 2025-02-11

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
09 | 2025-02-11 | **[Slides 09](https://thomaselove.github.io/432-slides-2025/slides09.html)** | [Code 09](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides09.qmd) | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

- In today's class, we'll return to the [Slides from Class 08](https://thomaselove.github.io/432-slides-2025/slides08.html). Specifically, we will start with **slide 35**.

---

## Announcements

1. There was a typo - fixed after class 2025-02-06 in slides 54, 96, 131, 166, and 203 of the [Slides from Class 08](https://thomaselove.github.io/432-slides-2025/slides08.html), where the C = 0.5 + Dxy/2 equation was missing the /2 part.
2. Frank Harrell's [Regression Modeling Strategies](https://hbiostat.org/rmsc/) and [Biostatistics for Biomedical Research](https://hbiostat.org/bbr/) books are incredibly useful resources for more on the `rms` and `Hmisc` packages.

## Some General Thoughts on the Project A Plans

1. In your portfolio, I'm adding the following requirements and I will change the template accordingly:
    - In section 6.2, I want to see the following three things for your linear outcome, in each case, restricting the data to the observations with complete data on that outcome.
        1. plots - at least a histogram and Normal Q-Q plot of the linear outcome, built using `ggplot2` and `patchwork`.
        2. numerical summaries - the results of both `Hmisc::describe()` and `mosaic::favstats()` for the linear outcome.
        3. a `tabyl()` (from the **janitor** package) of the most common values of your outcome, along with the fraction of all cases with complete data on that outcome that have that particular value, so that you can verify that no value occurs in more than 10% of your complete observations.
    - In a new section 6.3, I want to see a missingness summary including `n_miss`, `miss_var_summary()` and `miss_case_table()` across all variables in the codebook **after** filtering to the cases with complete data on your linear outcome.
    - In section 7.2, I want to see a a `tabyl()` (again from the **janitor** package) of the values of your outcome.
    - In a new section 7.3, I want to see a missingness summary including `n_miss`, `miss_var_summary()` and `miss_case_table()` across all variables in the codebook **after** filtering to the cases with complete data on your binary outcome.
2. I want to discourage you from using data set names, variable names and especially category level names that are long (more than perhaps 10 characters) if you can avoid it. You want to be clear, certainly, but long names are (a) harder to type and (b) harder to see in plots and tables.
3. I'm also not a fan of labels in R data sets for variables, as they make the results of many plots, tables and things like data_codebook() much harder to read.

## Today in "How To Be A Modern Scientist"

- Jeff Leek on "[How to share data with a statistician](https://github.com/jtleek/datasharing)"
- Shannon Ellis and Jeff Leek's publication (2018) [How to share data for collaboration](https://pmc.ncbi.nlm.nih.gov/articles/PMC7518408/). *The American Statistician*.

### On Data Sharing...

1. It is really hard to create a serious, research quality data set in almost any scientific discipline.
2. Data should be made available when papers are published. The question with reproducibility isn't "if" anymore, it is "how".
3. The transition toward reproducibility is likely to be rough.
4. Data sharing isn't easy and it isn't cheap.
5. Not knowing how to share data isn't an excuse - to be a modern scientist, this is one of the skills you have to have.
6. The culture of credit hasn't caught up with the culture of science.


