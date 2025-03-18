# 432 Class 17: 2025-03-18

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
17 | 2025-03-18 | **[Slides 17](https://thomaselove.github.io/432-slides-2025/slides17.html)** | **[Word 17](https://thomaselove.github.io/432-slides-2025/slides17w.docx)** | **[Code 17](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides17.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. **We have switched to in-person classes.** Class 17, on 2025-03-18, and almost all subsequent classes (see the [Calendar](https://thomaselove.github.io/432-2025/calendar.html) for exceptions) will be held in Room E321-323 of the Robbins Building at CWRU. For directions to the Robbins Building at CWRU, which is located at 2210 Circle Drive Cleveland OH 44106, and information on parking and on accessing the building, [visit this link](https://case.edu/medicine/cbhi/about-us/directions-and-parking/cwru-school-medicine-health-sciences-campus). Again, our classroom is on the third floor of the Robbins building, and is room E321-323.
2. The latest version of RStudio (ver 2024.12.1+563) is [available now](https://posit.co/download/rstudio-desktop/) and should be safe for you to download and use. The latest version of R, version 4.4.3, is [also now available](https://cran.case.edu/). I encouraged you to upgrade to these over Spring Break, but if you haven't done it, please do it now. Either version 4.4.2 or 4.4.3 of R is OK for the rest of this semester.
3. In **Project A**, I think that every student who came to me over the break with a problem fitting a model B or model Z had included multiple non-linear terms. If you note (for instance) that your complicated model isn't fitting properly, fit a simpler one, with fewer non-linear terms.
    - The project instructions encourage you to use about 6 df beyond the main effects model to account for non-linearity and at most 3 non-linear terms. If you are having trouble adding 6 df, then add 3-5 df which is fine and requires no explanation. In some cases, even just adding 1 or 2 df will be the most appropriate choice, and that's also OK, assuming you specify that you tried using more and what the problem was with doing so.
4. The [Biostats4You website](https://biostats4you.umn.edu/) at the University of Minnesota is dedicated to providing carefully selected, freely available biostatistics training materials for medical and public health professionals. The resources range from blog posts to published peer-reviewed articles to videos. The site currently provides 48 vetted resources on 12 topics, ranging from sample-size calculators to non-parametric methods to finding and working with a biostatistician.
    - The three newest resources expand our previously posted topic on the collection of race and ethnicity data to include considerations and best practices for analysis and reporting as well. Check them out [here](https://biostats4you.umn.edu/taxonomy/term/51).
5. [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) is due next Wednesday 2025-03-26 at Noon.
    - Submissions I have received [are posted here](https://github.com/THOMASELOVE/432-classes-2025/tree/main/lab6) as well as [on Campuswire in the Lab 6 folder](https://campuswire.com/).

## Regression on Count Outcomes

This week, we'll be presenting some key ideas on fitting models for count outcomes. Counts are discrete (rather than continuous) and counts are typically integers (0, 1, 2, 3 and so on) and cannot be made more precise. Relevant materials are available in Chapters 24-26 of the [Course Notes](https://thomaselove.github.io/432-notes/). 

Methods we will touch on this week include Poisson regression and negative binomial regression, along with augmentations of these two approaches to inflate the number of zeros predicted, and also "hurdle" versions which specify one process for zero counts and another for positive counts. In Chapters 24-26, we discuss all of these, as well as another approach, called a tobit (or censored) regression model.

![](ghement.png)

Here's [a link to the start of the "tweetorial"](https://twitter.com/IsabellaGhement/status/1363957122787024901) on some key practical aspects of understanding Poisson regression models.

- For more on rootograms, check out Kleiber C Zeileis A [Visualizing Count Data Regressions Using Rootograms](rootograms_2016.pdf) from *The American Statistician* 2016.
- For more on Vuong's test, check out Vuong, QH (1989) Likelihood ratio tests for model selection and non-nested hypotheses. *Econometrica*, 57:307-333.

## From Today's Slides

- [Interpreting Log Transformations](https://library.virginia.edu/data/articles/interpreting-log-transformations-in-a-linear-model).

## Methods for Regression on Count Outcomes (Notes, Chapters 24-26)

These recent examples from the open-access literature come from [this link](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md).

- Green JA (2021) [Too many zeros and/or highly skewed? A tutorial on modelling health behaviour as count data with Poisson and negative binomial regression](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8159206) Health Psychol Behav Med. 2021; 9(1): 436–455. [DOI](https://doi.org/10.1080%2F21642850.2021.1920416)
- Fernandez GA and Vatcheva KP (2022) [A comparison of statistical methods for modeling count data with an application to hospital length of stay](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9351158/) BMC Med Res Methodol. 2022; 22: 211. [DOI](https://doi.org/10.1186%2Fs12874-022-01685-8)
- Schaumberg K et al. (2018) [Improving Prediction of Eating-Related Behavioral Outcomes with Zero-Sensitive Regression Models](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6778476/) Appetite. 2018 Oct 1; 129: 252–261. [DOI](https://doi.org/10.1016%2Fj.appet.2018.06.030)
- Sifakaki M et al. (2023) [Orthorexia Nervosa Practices in Rheumatoid Arthritis: The DORA Study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9919523/) Nutrients. 2023 Jan 31; 15(3):713. [DOI](https://doi.org/10.3390%2Fnu15030713)
- Carcaiso V and Grilli L (2022) [Quantile regression for count data: jittering versus regression coefficients modelling in the analysis of credits earned by university students after remote teaching](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9554398/) Stat Methods Appt. 2022 Oct 12 : 1–22. [DOI](https://doi.org/10.1007%2Fs10260-022-00661-2)

-----

## Why I use `read_csv()` all the time, and never use `read.csv()` anymore

1. `read_csv()` is much faster than `read.csv()`, 
2. `read_csv()` provides a progress meter and a compact method for specifying column types,
3. `read_csv()` will read compressed files automatically,
4. `read_csv()` automatically creates a tibble, and
5. `read_csv()` allows me to speed the process of debugging by providing much more useful error messages about which rows are problematic, especially when the error is non-fatal.

- For more details, see the [Data import section of R for Data Science](https://r4ds.hadley.nz/data-import.html).
- From Josh Gonzales at Medium: [read_csv(): The Best Way to import CSV data into R](https://medium.com/r-tutorials/r-functions-daily-read-csv-3c418c25cba4)
