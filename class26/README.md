# 432 Class 26: 2025-04-17

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
26 | 2025-04-17 | **[Slides 26](https://thomaselove.github.io/432-slides-2025/slides26.html)** | **[Word 26](https://thomaselove.github.io/432-slides-2025/slides26w.docx)** | **[Code 26](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides26.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. We corrected a small typo in the [Project B portfolio template](https://github.com/THOMASELOVE/432-data/blob/master/data/432_projectB_portfolio_template.qmd), where section 6.1 is now correctly headed as "Managing Data for Analysis 2" instead of for Analysis 1.
2. Feedback on the Minute Paper after Class 25 is found at <https://bit.ly/432-2025-min25-feedback>. You'll need to log into Google via CWRU to see it.
3. A great reference is [On the 12th Day of Christmas, a Statistician Sent to Me](https://doi.org/10.1136/bmj-2022-072883) from BMJ in 2022. Here is an excerpt from the Abstract...

> To elicit the most common issues encountered during statistical peer review, an internal survey was administered to The BMJ’s statistical editors. Twelve items were identified, and each are described here. There is one item for each of the 12 days of Christmas, the period between 25 December and 5 January when the statisticians conduct their reviews in the mindset of *The Grinch*, but with the kind heart of *Miracle On 34th Street*.

## Two Great Courses

- Frank Harrell's Short Course on Regression Modeling Strategies <https://hbiostat.org/doc/rms/4day.html> and his [book on the subject](https://hbiostat.org/doc/rms/book/)
- Richard McIlreath's Statistical Rethinking course <https://github.com/rmcelreath/stat_rethinking_2024> with lectures on YouTube.

## Our Starting Point for Today's Class

- [An Introduction to Hierarchical Modeling (Visual Explanation)](http://mfviz.com/hierarchical-models/) by [Michael Freeman](http://mfviz.com/)

## Other Resources for Hierarchical Data Mentioned in the Class 26 Slides

- [Generalized Linear Mixed Models FAQ](https://bbolker.github.io/mixedmodels-misc/glmmFAQ.html) by Ben Bolker and others. Other work by Ben Bolker includes...
    - [Some notes on (generalized) linear mixed models](https://bbolker.github.io/morelia_2018/notes/glmm.html)
    - [Some worked examples of these models](https://bbolker.github.io/mixedmodels-misc/ecostats_chap.html)
- [The Introduction to Mixed Models from Environmental Computing](http://environmentalcomputing.net/mixed-models/) folks at the University of New South Wales, Australia.
- [Workshop on Linear mixed effects models from the Quebec Centre for Biodiversity Science](https://wiki.qcbs.ca/r_workshop6) developed by Catherine Baltazar, Dalal Hanna and Jacob Ziegler
- [A useful bibliography of mixed effect regression models](https://joelemartinez.com/2015/07/14/mixed-effect-models/) by Joel Eduardo Martinez
- [Using `sjPlot` in R to summarize Mixed Models in HTML tables](https://strengejacke.github.io/sjPlot/articles/tab_mixed.html) and [Using `sjPlot` to Plot Model Estimates](https://strengejacke.github.io/sjPlot/articles/plot_model_estimates.html)
- [UCLA example using mixed effects logistic regression](https://stats.idre.ucla.edu/r/dae/mixed-effects-logistic-regression/)

## Some Machine Learning Sources from Frank Harrell (and friends)

I've been asked to talk a bit about machine learning, so I'll send you to my main sources.

- Frank Harrell's [Road Map for Choosing Between Statistical Modeling and Machine Learning](https://www.fharrell.com/post/stat-ml/)
- Drew Levy on [Navigating Statistical Modeling and Machine Learning](https://www.fharrell.com/post/stat-ml2/) is a great follow-up discussion of Frank's main post.
- Frank also has a video of a talk called [Musings on Statistical Models vs. Machine Learning in Health Research](https://www.fharrell.com/talk/mlhealth/) available.
- Another helpful video on some related issues from Frank is [Controversies in Predictive Modeling, Machine Learning, and Validation](https://www.fharrell.com/talk/stratos19/).

