# 432 Class 21: 2025-04-01

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
21 | 2025-04-01 | **[Slides 21](https://thomaselove.github.io/432-slides-2025/slides21.html)** | **[Word 21](https://thomaselove.github.io/432-slides-2025/slides21w.docx)** | **[Code 21](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides21.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) grades are now posted to the Shared Google Drive's Course Grading Roster. I've included a reminder of what you need to do if you haven't yet completed the assignment. The final deadline is 2025-04-15.
2. The [Project B Proposal Form](https://bit.ly/432-2025-projB-proposal) is due at noon tomorrow (2025-04-02) - please read the instructions at <https://thomaselove.github.io/432-2025/projB.html> thoroughly before completing the form.
    - We want you to have your data successfully ingested in R before you fill out the form, too. This doesn't mean you've cleaned the data yet, especially, but it does mean that you have the data in R and can summarize the number of complete cases for each of your variables.
    - If you are working with a partner, exactly **one** of you should complete the form. The non-submitting partner should send an **email** to Dr. Love by the deadline with the subject line **432 Project B Partnership** confirming that you are working in a partnership and telling me the name of your partner.
3. [Lab 7](https://thomaselove.github.io/432-2025/lab7.html) is the final lab this term, and is due at noon on 2025-04-09.
    - There are four questions. You should be able to do all of questions 1-3 as well as part (a) of question 4 after today's class. You'll be able to do part (b) of question 4 after Thursday's Class 22.
    - Remember that Lab 7, like Lab 6, is not "skippable".
    - For Lab 7, we will charge a 5 point penalty for a lab that is 1-24 hours late.
    - The answer sketch will be posted online 24 hours after the lab is due. As a result, we will charge a 15 point penalty for a response that is more than 24 hours but less than 48 hours late, and, as always, we won't grade anything received more than 48 hours late.
4. **On Assuming MCAR** Little's `mcar_test()` can be used to help build up some understanding as to whether we'll see a meaningful difference if we assume MCAR (and use complete cases) vs. MAR (with imputation.) If the test shows a low *p* value, this is a firm indication that the MCAR assumption isn't reasonable. On the other hand, if the `mcar_test()` result shows a large *p* value, that doesn't mean the data are MAR, specifically. They still could certainly be missing not at random (MNAR).

## Agenda 

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

