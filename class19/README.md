# 432 Class 19: 2025-03-25

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
19 | 2025-03-25 | **[Slides 19](https://thomaselove.github.io/432-slides-2025/slides19.html)** | **[Word 19](https://thomaselove.github.io/432-slides-2025/slides19w.docx)** | **[Code 19](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides19.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. If you learn nothing else from this course in general and this project in particular, please learn that statistical significance is not in any way a useful concept, and you shouldn't be using it for any purpose.
2. [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) is due tomorrow. Submissions I have so far received [are listed here](https://github.com/THOMASELOVE/432-classes-2025/tree/main/lab6), as well as on Campuswire.
3. The [Project B Proposal Form](https://bit.ly/432-2025-projB-proposal) is due at noon on Wednesday 2025-04-02. Please read the instructions at <https://thomaselove.github.io/432-2025/projB.html> thoroughly before completing the form.
    - We want you to have your data successfully ingested in R before you fill out the form, too. This doesn't mean you've cleaned the data yet, especially, but it does mean that you have the data in R and can summarize the number of complete cases for each of your variables.
    - If you are working with a partner, exactly **one** of you should complete the form. The non-submitting partner should send an **email** to Dr. Love by the deadline with the subject line **432 Project B Partnership** confirming that you are working in a partnership and telling me the name of your partner.
4. The 2025 A-mu-sing competition is on again at [Cause Web](https://www.causeweb.org/cause/a-mu-sing/2025/rules).
    - The Fun Collection is available [here](https://www.causeweb.org/cause/resources/fun/).

## Sources from Today's Slides

- [UCLA site on Ordinal Logistic Regression](http://stats.idre.ucla.edu/r/dae/ordinal-logistic-regression/)
    - [How do I interpret the coefficients in an ordinal logistic regression in R?](https://stats.oarc.ucla.edu/r/faq/ologit-coefficients/)
- [UCLA site on Multinomial Logistic Regression](https://stats.oarc.ucla.edu/r/dae/multinomial-logistic-regression/)
- [MASS reference manual (pdf)](https://cran.r-project.org/web/packages/MASS/MASS.pdf)
- Frank Harrell on [Model Uncertainty, Penalization, and Parsimony (pdf)](http://hbiostat.org/talks/iscb98.pdf)
- Frank E. Harrell [Regression Modeling Strategies](https://github.com/THOMASELOVE/432-sources/blob/main/pdf/Harrell_Regression_Modeling_Strategies_2015_2e_protected.pdf), 2nd Edition, 2015. (password-protected PDF)

## Recent Examples: Regression on Ordinal Outcomes ([Notes, Chapter 27](https://thomaselove.github.io/432-notes/ordinaloutcome.html))

These recent examples from the open-access literature come from [this link](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md).

- Bhattacharyay S et al. (2022) [The leap to ordinal: Detailed functional prognosis after traumatic brain injury with a flexible modelling approach](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9255749/) PLoS One. 2022; 17(7): e0270973. [DOI](https://doi.org/10.1371%2Fjournal.pone.0270973)
- Nawi MAA et al. (2022) [The patterns of facial fractures in traumatic brain injury (TBI) patients using ordinal regression: a retrospective study of five years](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9581734/) AIMS Neurosci. 2022; 9(3): 345–357. [DOI](https://doi.org/10.3934%2FNeuroscience.2022019)
- Glasgow TW et al. (2022) [Eat, sleep, play: health behaviors and their association with psychological health among cancer survivors in a nationally representative sample](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9190125/) BMC Cancer. 2022; 22: 648. [DOI](https://doi.org/10.1186%2Fs12885-022-09718-7)
- Akinosoglou K et al. (2023) [Efficacy and safety of early soluble urokinase plasminogen receptor plasma-guided anakinra treatment of COVID-19 pneumonia: A subgroup analysis of the SAVE-MORE randomised trial](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9791950/) eClinicalMedicine. 2023 Feb; 56: 101785. [DOI](https://doi.org/10.1016%2Fj.eclinm.2022.101785)
- Bersch I et al. (2022) [A Prediction Model for Various Treatment Pathways of Upper Extremity in Tetraplegia](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9397669/) Front Rehabil Sci. 2022; 3: 889577. [DOI](https://doi.org/10.3389%2Ffresc.2022.889577)

