# 432 Class 21: 2025-04-01

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
21 | 2025-04-01 | **[Slides 21](https://thomaselove.github.io/432-slides-2025/slides21.html)** | **[Word 21](https://thomaselove.github.io/432-slides-2025/slides21w.docx)** | **[Code 21](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides21.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Project A Feedback

Project A feedback, including all grades and comments, is now in your CWRU email (sent last night.)

- The PDF is several pages long, and includes information on more than 100 different issues.
- The highest project A grade was 96. Grades of 90-96 are A, grades of 86-89 are A-, and grades of 70-85 are various types of B.
- There was no important difference between the distributions of grades for single investigators and pairs of two.
- The TAs reviewed Section 10 (Discussion), while I did the rest.
- There were 40 projects, including more than 49,000 lines of Quarto code, and data on 47,027 subjects with an average of just over 8 non-subject variables per project.
- Seven projects were done with R version 4.4.3, one with 4.4.1 (need to upgrade), and the rest with version 4.4.2
- Three projects used Windows 10, 14 used Windows 11, while 23 used various MacOS setups, including 2 with Big Sur (macOS 11), 3 with Monterey (macOS 12), 1 with Ventura (macOS 13), 3 with Sonoma (macOS 14), and 14 using various versions of Sequoia (macOS 15). If you're below Sonoma, I would upgrade, if possible.
- Data Sources for the 40 projects:
    - 5 with Behavioral Risk Factor Surveillance System (BRFSS)
    - 4 with Cleveland Community Cat Project Outcomes dataset collected from 2023-2024
    - 4 with Racial and Ethnic Representativeness of US Postsecondary Education Institutions project provided by the Urban Institute Data Catalog
    - 3 with CDC PLACES / 500 Cities
    - 3 with National Survey on Drug Use and Health (NSDUH)
    - 2 with the Asthma Call-Back Survey from the Behavioral Risk Factor Surveillance System (BRFSS)
    - 2 with Coffee Ratings from TidyTuesday 2020-07-07
    - 2 with General Social Survey (GSS) Data
    - 2 with Health and Retirement Study
    - 2 with National Survey of Family Growth (NSFG)
    - 1 with CDC WONDER Multiple Causes of Death data merged with County Health Rankings
    - 1 with Homeowner Assistance Fund County-Level Targeting Data from the Urban Data Catalog along with County Health Rankings
    - 1 with Household Conditions by Geographic School District data from the Urban Institute
    - 1 with NIH RePORTER and ClinicalTrials.gov
    - 1 with Project FeederWatch via Tidy Tuesday 2023-01-10
    - 1 with State of Connecticut Accidental Drug Related Deaths (2012-2023)
    - 1 with The National Survey of Children’s Health (NSCH), from the year 2023
    - 1 with TidyTuesday 2020-03-10 Tuition Tracker and Pay Scale information
    - 1 with TidyTuesday 2024-03-05 Trash Wheel Collection data as part of the Baltimore Healthy Harbor Initiative
    - 1 with Winter Olympics Data from Tidy Tuesday Archive from 2021-07-27
    - 1 with Youth Development Study, a longitudinal study housed at the University of Minnesota
- I made all of the final decisions about grading. If you have a concern, contact me via email before 2025-04-15, after which I will consider this project closed.

## Announcements

1. The [Project B Proposal Form](https://bit.ly/432-2025-projB-proposal) is due at noon tomorrow (2025-04-02) - please read the instructions at <https://thomaselove.github.io/432-2025/projB.html> thoroughly before completing the form. **Please** make the deadline.
    - If you are working with a partner, exactly **one** of you should complete the form. The non-submitting partner should send an **email** to Dr. Love by the deadline with the subject line **432 Project B Partnership** confirming that you are working in a partnership and telling me the name of your partner.
    - Thanks to an alert student, we've fixed a typo in the Project B Plan Description (The main reason why we *don't* approve projects... instead of *doesn't*).
    - A list of Project B projects I have received some information about [is here](https://github.com/THOMASELOVE/432-classes-2025/tree/main/projectB).
2. [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) grades are now posted to the Shared Google Drive's Course Grading Roster. I've included a reminder of what you need to do if you haven't yet completed the assignment. The final deadline is 2025-04-15.
3. [Lab 7](https://thomaselove.github.io/432-2025/lab7.html) is the final lab this term, and is due at noon on 2025-04-09.
    - There are four questions. You should be able to do all of questions 1-3 as well as part (a) of question 4 after today's class. You'll be able to do part (b) of question 4 after Thursday's Class 22.
    - Remember that Lab 7, like Lab 6, is not "skippable".
    - For Lab 7, we will charge a 5 point penalty for a lab that is 1-24 hours late.
    - The answer sketch will be posted online 24 hours after the lab is due. As a result, we will charge a 15 point penalty for a response that is more than 24 hours but less than 48 hours late, and, as always, we won't grade anything received more than 48 hours late.
4. **On Assuming MCAR** Little's `mcar_test()` can be used to help build up some understanding as to whether we'll see a meaningful difference if we assume MCAR (and use complete cases) vs. MAR (with imputation.) If the test shows a low *p* value, this is a firm indication that the MCAR assumption isn't reasonable. On the other hand, if the `mcar_test()` result shows a large *p* value, that doesn't mean the data are MAR, specifically. They still could certainly be missing not at random (MNAR).
5. I'm not suggesting this would work as a data set for Project B, but the [Cleveland Health Survey](https://prchn.org/clehealthsurvey/) for 2025 has released some of its early reports, and it's a very important project.

## Agenda for Today's Slides

Multinomial Logistic Regression, including two examples about alligators that I described in Class 20.

## Sources

- [Chapter 28](https://thomaselove.github.io/432-notes/multinomial.html) of our [Course Notes](https://thomaselove.github.io/432-2025/notes.html)
- A good source of information on fitting these models is [this link](https://stats.idre.ucla.edu/r/dae/multinomial-logistic-regression/) from UCLA.
- Using the tidymodels structure to fit these models is another good idea. Julia Silge has a [very nice example here](https://juliasilge.com/blog/multinomial-volcano-eruptions/)
- More mathematically oriented sources include the following texts:
  - Hosmer DW Lemeshow S Sturdivant RX (2013) Applied Logistic Regression, 3rd Edition, Wiley
  - Agresti A (2007) An Introduction to Categorical Data Analysis, 2nd Edition, Wiley.

## Methods for Regression on Nominal Multi-Categorical Outcomes

These recent examples from the open-access literature come from [this link](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md).

- Bendera A et al. (2022) [Factors Associated with Low Uptake of Medical Male Circumcision Among Adolescent Boys in Tanzania: A Multinomial Logistic Regression Modeling](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9785118/) HIV AIDS (Auckl). 2022; 14: 565–575. [DOI](https://doi.org/10.2147%2FHIV.S387380)
- Verhoeven J et al. (2022) [Patient characteristics and dispatch responses of urinary tract infections in a prehospital setting in Copenhagen, Denmark: a retrospective cohort study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9736713/) BMC Prim Care. 2022; 23: 319. [DOI](https://doi.org/10.1186%2Fs12875-022-01915-4)
- Sakala N and Kaombe TM (2022) [Analysing outlier communities to child birth weight outcomes in Malawi: application of multinomial logistic regression model diagnostics](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9701370/) BMC Pediatr. 2022; 22: 682. [DOI](https://doi.org/10.1186%2Fs12887-022-03742-z)
- Klu D et al. (2022) [Determinants of communication on sexual issues between adolescents and their parents in the Adaklu district of the Volta region, Ghana: a multinomial logistic regression analysis](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9044737/) Reprod Health. 2022; 19: 101. [DOI](https://doi.org/10.1186%2Fs12978-022-01402-0)
- Yokoi Y et al. (2022) [How Sleep Quality Relates to Bodily and Oral Symptoms: An Analysis from Japanese National Statistics](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9690173/) Healthcare (Basel). 2022 Nov; 10(11): 2298. [DOI](https://doi.org/10.3390%2Fhealthcare10112298)

