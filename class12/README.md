# 432 Class 12: 2025-02-20

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
12 | 2025-02-20 | **[Slides 12](https://thomaselove.github.io/432-slides-2025/slides12.html)** | **[Word 12](https://thomaselove.github.io/432-slides-2025/slides12w.docx)** | **[Code 12](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides12.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. Some of you may be struggling with estimating and interpreting effect sizes in linear and logistic regression models. [Chapter 22 of the Course Notes](https://thomaselove.github.io/432-notes/effectsize.html) walks through this for fits built with `lm()`, `glm()`, `ols()` and `lrm()`, including what to do if we include a spline or interaction term, and making predictions and building prediction intervals for linear fits, among other things. [It might be the most useful chapter in the Notes](https://thomaselove.github.io/432-notes/effectsize.html).
2. Note that I don't have any use for the notion of statistical significance. Estimating P values or confidence intervals are completely fine, but then binarizing something meaningful like that into "the p value is less than 0.05, so my result is meaningful" is something I encourage you never to do again, in any situation, and definitely not in this class. My only regret in Chapter 22 of the Notes is that in one spot I describe something as having detectably lower odds, which is just a synonym for the odds being lower and also being associated with a small p value. For more on this, read [the first two articles on our Sources page](https://github.com/THOMASELOVE/432-sources?tab=readme-ov-file#key-articles).

## Links about Today's New Packages

1. Links related to the **here** package: <https://here.r-lib.org/>
    - Jenny Bryan [I love the here package. Here's why.](https://github.com/jennybc/here_here)
    - R for Data Science (2nd ed.) [chapter on Workflow: Scripts and Projects](https://r4ds.hadley.nz/workflow-scripts)
2. Link related to the **conflicted** package: <https://conflicted.r-lib.org/>
3. Link related to the **tableone** package: <https://github.com/kaz-yos/tableone> which lists many complimentary packages for doing similar things
    - Introductory vignette is <https://cran.r-project.org/web/packages/tableone/vignettes/introduction.html>.
4. Some data we'll discuss today comes from [NHANES](https://www.cdc.gov/nchs/nhanes/index.html).
    - It seems that [the nhanesA package](https://cran.r-project.org/web/packages/nhanesA/index.html) is working again, which should be a relief to those of you considering NHANES as a source of data for Project B later this semester.
    - The `nh1314.Rds` and `nhanes_class12_data2.Rds` files are available on [our 432 data page](https://github.com/THOMASELOVE/432-data), and also [here](data).

## Materials for the `bradley` example we'll discuss today

- The original source is Steven M. Bradley, Joleen A. Borgerding, G. Blake Wood, et al. [Incidence, Risk Factors, and Outcomes Associated With In-Hospital Acute Myocardial Infarction](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2720923) *JAMA Netw Open* 2019; 2(1): e187348. doi:10.1001/jamanetworkopen.2018.7348.
- [JAMA Table Creation Instructions](https://jama.jamanetwork.com/data/ifora-forms/jama/tablecreationinst.pdf) (pdf)
- The bradley_sim file: [.qmd code](bradley/bradley_sim.qmd), [.html result at RPubs](https://rpubs.com/TELOVE/bradley-simulate-432)
- The bradley_table1 file: [.qmd code](bradley/bradley_table1.qmd), [.html result at RPubs](https://rpubs.com/TELOVE/bradley-table1-432)
- The [bradley.csv](data/bradley.csv) data file
- The [bradley_table1_result.csv](data/bradley_table1_result.csv) file

[Chapter 18 in the Course Notes](https://thomaselove.github.io/432-notes/) covers the topic of building a Table 1 far more extensively, with two detailed examples.

-----

## Today in "How To Be A Modern Scientist"

### On Peer Review

What should I do and why?

- Review papers quickly or not at all
- (Try to) get credit for your reviews.
- Reviewing templates and how to build comments to the authors (summary, major issues, minor issues, typos)
- Who are the key players?

Reviewing: What is the job?

- Evaluating quality and accuracy of methods, data and results.
- Determining whether the methods, data and results justify the claims.
- Determining how important the claims are and whether they belong in the journal the paper was submitted to.
- Submitting a recommendation (and not being a jerk)

### On "Credit"

- Don't forget that the primary thing you will be judged on is publications.
- Quantify everything.
- Include metrics on your CV.
- Discuss your approach with a senior colleague.
