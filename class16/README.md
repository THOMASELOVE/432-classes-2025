# 432 Class 16: 2025-03-06

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
16 | 2025-03-06 | **[Slides 16](https://thomaselove.github.io/432-slides-2025/slides16.html)** | **[Word 16](https://thomaselove.github.io/432-slides-2025/slides16w.docx)** | **[Code 16](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides16.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Today's Agenda

1. README announcements and things...
2. Quiz 1 results...
    - The **Quiz 1 answer sketch and grading rubric** is now available (HTML) in the **432 Quiz 1 Materials** folder in our Shared Drive.
        - I'll spend a few moments today on **Questions 2, 5, 9, 12, 21 and 23** in that Sketch.
    - All of you should have received two emails from me (at your CWRU email) this morning,
        - one with the subject line: **432 Quiz 1 results will be coming to you in email soon** and then
        - one with the subject line **432 Quiz 1 Results for {YOUR NAME}** that has your results on the Quiz.
    - Please review my grading, and if you have any questions, email me, and I will respond between March 15 and 17. 
3. More on time-to-event (survival) data (see the slides)
4. **At 2 PM**: Some general suggestions about Project A, followed by "Ask Me Anything" about Project A.

## A few reminders

1. Spring Break is next week, and we will not have class on either 2025-03-09 or 2025-03-11.
2. Dr. Love will be away and unresponsive to emails and Campuswire from 2025-03-07 through 2025-03-14.
3. The TAs will not hold office hours from 2025-03-08 through 2025-03-14.
4. Class 17, on 2025-03-18, and almost all subsequent classes (see the [Calendar](https://thomaselove.github.io/432-2025/calendar.html) for exceptions) will be held in Room E321-323 of the Robbins Building at CWRU. For directions to the Robbins Building at CWRU, which is located at 2210 Circle Drive Cleveland OH 44106, and information on parking and on accessing the building, [visit this link](https://case.edu/medicine/cbhi/about-us/directions-and-parking/cwru-school-medicine-health-sciences-campus). Again, our classroom is on the third floor of the Robbins building, and is room E321-323. I very much look forward to seeing you all in person!

## Announcements

1. The [Project A Portfolio](https://thomaselove.github.io/432-2025/projA.html#the-project-a-portfolio) is due to Canvas at noon on 2025-03-19. Get your questions in before we disappear for Break, if possible.
    - Remember the Portfolio includes a complete Quarto file, complete HTML file, complete tidied R data set file, and (up to 4 minute) video file.
2. Remember that [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) is due on Wednesday 2025-03-26 at Noon. This is a **great** thing to get out of the way during the Break.
3. The latest version of RStudio (ver 2024.12.1+563) is [available now](https://posit.co/download/rstudio-desktop/) and should be safe for you to download and use. The latest version of R, version 4.4.3, is [also now available](https://cran.case.edu/). **I encourage you to upgrade to these over Spring Break.**
4. Those of you who want to get way ahead of things, the [Project B instructions](https://thomaselove.github.io/432-2025/projB.html) are complete, and the [Project B proposal form](https://bit.ly/432-2025-projB-proposal) is open. The form is due Wednesday 2025-04-02 at Noon.
    - On 2025-03-03, I updated the [Project B instructions](https://thomaselove.github.io/432-2025/projB.html), and the [Project B portfolio template](https://github.com/THOMASELOVE/432-data/blob/master/data/432_projectB_portfolio_template.qmd) on our [432 data page](https://github.com/THOMASELOVE/432-data), so make sure you have the new versions.
5. On 2025-03-04, I updated The Support 1000 Study example on our Shared Drive to include new sections 5-8, which cover the main regression modeling approaches we will see after Spring Break.
6. Occasionally, people ask me about whether some of the methods we use appear in the literature frequently. Visit [this link](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md) for examples of, among other things,
    - [Splines to account for Non-Linearity in Linear or Generalized Linear Models](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md#splines-to-account-for-non-linearity-in-linear-or-generalized-linear-models-notes-chapters-13-and-many-others)
    - [Model Validation, the LASSO and ridge regression](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md#model-validation-lasso-ridge-regression)
    - [Single and Multiple Imputation Strategies](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md#single-and-multiple-imputation-strategies-notes-chapters-7-and-17-and-others)
    - [Nomograms](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md#nomograms-notes-chapter-14-and-others)
    - along with topics we'll cover after Spring Break.

---

## Today in "How To Be A Modern Scientist"

### On Social Media

- This is often the section of the book which people view has aged least well
- Use your social media account to promote the work of other people
- Share work you develop
- Include images if you can

### On Teaching

- Put all your teaching materials online
- Put teaching videos online
- Develop a thick skin

----

## Today's Excerpt from "[Moving to a World Beyond 'p < 0.05'](https://github.com/THOMASELOVE/432-sources/blob/main/pdf/ASA_2019_A_World_Beyond.pdf)"

from **Don't say "Statistically Significant"**

To move forward to a world beyond "p < 0.05," we must recognize afresh that statistical inference is not—and never has been—equivalent to scientific inference. However, looking to statistical significance for a marker of scientific observations' credibility has created a guise of equivalency. 

Moving beyond "statistical significance" opens researchers to the real significance of statistics, which is "the science of learning from data, and of measuring, controlling, and communicating uncertainty."

In sum, "statistically significant" -- don't say it and don't use it.

There are many Do's. With the don’ts out of the way, we can finally discuss ideas for specific, positive, constructive actions. 

We have a massive list of them in [the seventh section of this editorial](https://github.com/THOMASELOVE/432-sources/blob/main/pdf/ASA_2019_A_World_Beyond.pdf)! In that section, the authors of all the articles in this special issue each provide their
own short set of do's.

["Not statistically significant" is not the same as zero](https://statmodeling.stat.columbia.edu/2021/09/28/not-statistically-significant-is-not-the-same-as-zero/) from Andy Gelman's blog, 2021-02-28. The money quote for me is this:

> This illustrates one of the challenges of statistical communication: there are so many opportunities to garble the message. And even if you make no mistakes, people can still misinterpret what you’ve written, given the **norm of acting as if every study either makes a discovery or proves that something equals zero**.

- For more on a related example, you might be interested in [RCT on use of cloth vs surgical masks](https://statmodeling.stat.columbia.edu/2020/04/15/rct-on-use-of-cloth-vs-surgical-masks/) from 2020-04-15.

---

## Sources related to Today's Slides

- Laurie et al. (1989) [Surgical adjuvant therapy of large-bowel carcinoma: An evaluation of levamisole and the combination of levamisole and fluorouracil: The North Central Cancer Treatment Group and the Mayo Clinic](https://pubmed.ncbi.nlm.nih.gov/2778478/). *J Clinical Oncology*, 7:1447-1456. DOI: 10.1200/JCO.1989.7.10.1447
- Moertel et al. (1990) [Levamisole and fluorouracil for adjuvant therapy of resected colon carcinoma](https://pubmed.ncbi.nlm.nih.gov/2300087/). *New England J of Medicine*, 332:352-358. DOI: 10.1056/NEJM199002083220602
- The survminer package: <https://rpkgs.datanovia.com/survminer/index.html>
- The survival package: Reference Manual (pdf) is [here](https://cran.r-project.org/web/packages/survival/survival.pdf), while the website is  <https://github.com/therneau/survival>.
- My [course notes chapter on Time-to-Event / Survival Data](https://thomaselove.github.io/432-notes/survival_data.html)

----

# Some Project A Tips

## On Naming Things

Naming things is hard. [Jenny Bryan has you covered](https://speakerdeck.com/jennybc/how-to-name-files). The three principles are:

- machine readable
- human readable
- play well with default ordering

A perfectly lovely **file name** convention for project A would be `2025-03-19_yourname_432projA.xxx`

Naming R data frames (tibbles) can be challenging, as well. I'll add 

- don't name tibbles things that are also data frames or functions or other things in R
- don't name tibbles things that make no sense without a very detailed explanation
- 8 characters is usually a good maximum for a tibble name that you'll use often
- if you insist on separating words in a tibble name, use underscores.

## Some Common Problems You Can Fix in your Project A

1. Sometimes, we see people failing to drop levels of a categorical predictor after combining levels. Use the `droplevels()` command.
2. Sometimes, we see people fitting restricted cubic splines or polynomials either to categorical predictors or to quantitative predictors with just a few observed values.
3. Remember that it's perfectly fine in model B to add fewer than the maximum additional degrees of freedom beyond the main effects model so long as you include at least one non-linear term.
4. Suppose you decide to create a decision rule for a logistic regression model. Feel encouraged to make a rational choice other than 0.5 for the cutoff, probably using `cutpointr()`
5. When you build a plot of the ROC curve for your final model, be sure it provides the same C statistic value as you get from the `lrm` fit to the data, and that you also provide the validation-adjusted C statistic estimate for that model.
6. Something we've seen **a lot** in looking at Quarto files people have sent is the failure to include a blank line **before and after** every **heading and subheading**, and **every code chunk**. This is a problem.
7. Don't name the file `projectAproposal.Rmd` when it's not your proposal. A good generic name would be `2025-03-19_432_projA.Rmd` or `432projectA_2025-03-19.Rmd` assuming it's the version from that date (2025-03-19).
8. Be sure to run the spell-check, and ideally, have someone else read through your work.
9. We hate scrolling windows in HTML output caused by code that runs too long on one line. Use the ENTER key liberally to help avoid this problem, and check your HTML to see if it is happening.
10. Make sure your headings are in an appropriate order, and that you have all of the main sections in your Project A, as laid out in the sample demonstration project A. Check your HTML to make sure the headings make sense, for instance, `10`, then `10.1`, then `10.1.1.` is OK, but `10`, then `10.0.1` isn't OK.
11. If you're loading a package not on our [R packages list](https://thomaselove.github.io/432-2025/software.html#r-packages-to-install), then you should definitely indicate why you're doing this at the top of your work as you load it in a short comment. Also, don't load elements of [the core `tidyverse`](https://www.tidyverse.org/packages/) separately: load them with `tidyverse` only, and don't add packages from [the **easystats** framework](https://easystats.github.io/easystats/) separately: load them with `easystats` only.

## What should I do if I have a problem with Normality in my linear model (Project A)?

1. Not all problems can be fixed with power transformations and non-linear terms.
2. You should describe what the residual plots (from `check_model()`) show, accurately.
3. If there is a problem with the residual plots, use that fact in making a decision about which model to select as your final model. 
4. If you have to select a final model with residual plot problems, describe how those problems might affect your conclusions.

## Exploding Coefficients and Problems in Logistic Regression

Sometimes, we see people fitting models to predict a binary outcome using a predictor which completely determines that outcome (for example, if predictor > 12, then outcome is always no, or if predictor = "Yes" then outcome is always no.)

Take a look at [this toy example with explosive coefficients](https://rpubs.com/TELOVE/explosion_logistic_432) to see one way in which this problem can emerge and what to do about it.

## Project A presentation video advice

The presentation video is literally the first thing Dr. Love will review in your project. As a result, it takes on extra importance.

Make sure that you introduce yourself when you start to speak, over your title slide if you are working alone. We’re happy to see your face during the presentation, but this isn’t mandatory. If you are working with a partner, each of you should introduce yourself at the beginning, and let me know who’s speaking first.

(Essentially) every word and every image/table/chart in your slides can and should come directly from the materials contained in your HTML portfolio.

We suggest you develop about 8 slides. This should include…

- A title slide
- A couple of slides to describe the Subjects, Outcome and Predictors
    - Make sure we understand who the subjects are, how they were selected, what the outcome is and why we should care about it, and what predictors are involved in the model you’ll show.
- Several slides showing meaningful statistical findings (What should we learn from your model?)
    - What does the model (don’t show us details of multiple models in the presentation) say about the relationship between the outcome and the predictors?
    - You’re only showing us one model (of models A, B, Y and Z) in the presentation.
    - How well does this model fit the data you have, and how well might it fit in new data?
- A couple of slides discussing next steps
    - It is unlikely that you’ll have a model that is truly satisfactory all on its own, so what could be done to improve it that you cannot already do with the data you have? What other data could be collected, how could the measures be refined, could you design a study to get to a more convincing answer?
    - Do not exceed the time limit by more than 10 seconds, or we will reduce your grade.
 
