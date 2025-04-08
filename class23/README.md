# 432 Class 23: 2025-04-08

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
23 | 2025-04-08 | **[Slides 23](https://thomaselove.github.io/432-slides-2025/slides23.html)** | **[Word 23](https://thomaselove.github.io/432-slides-2025/slides23w.docx)** | **[Code 23](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides23.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

![](https://imgs.xkcd.com/comics/assigning_numbers.png) [Source: XKCD](https://xkcd.com/2610/)

## Announcements

To come.

## Agenda

- Using `coxph()` and then `cph()` from the **rms** package to estimate and assess Cox propoprtional hazards regression models

## A few thoughts on the adjusted R-square statistic

In linear regression work, the "adjusted R-square" statistic attempts to use the same data to fit the model and evaluate it, through applying a penalty based on the number of coefficient estimates that need to be developed and the sample size. This summary is somewhat interesting, and has some value occasionally. However, I usually avoid placing much weight on the summary statistic "adjusted R-square" to describe the predictive quality of a model, in favor of a validated R-square statistic, which might include:

- the "optimism-corrected" results of a bootstrap validation (as in `validate` for an `ols` fit)
- the r-square value observed when applying a model fit in a training sample to holdout data in a test sample
- some other cross-validated r-square statistic, as can be developed using the `rsample` and `yardstick` packages (see, for example, Chapters 9 and 10 in [Tidy Modeling with R](https://www.tmwr.org/).

So my main point is that I wouldn't use adjusted R-square much (if at all) in linear regression, instead using a better method to assess predictive power in linear regression.


## Sources

- Rossi's recidivism data [are described here](https://rdrr.io/cran/carData/man/Rossi.html), as well as many other places.
- These data are also the main example in John Fox and Sanford Weisberg's [Cox Proportional-Hazards Regression for Survival Data in R](https://www.john-fox.ca/Companion/appendices/Appendix-Cox-Regression.pdf) (pdf) which describes the basis for the Cox model in more detail than I will today, and also explains how to use the **survival** package in R to estimate Cox regressions.
- Frank Harrell's website at <https://hbiostat.org/r/rms/> includes links to [this video](https://www.youtube.com/watch?v=EoIB_Obddrk) demonstrating some interactive survival curves.

