# 432 Class 22: 2025-04-03

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
22 | 2025-04-03 | **[Slides 22](https://thomaselove.github.io/432-slides-2025/slides22.html)** | **[Word 22](https://thomaselove.github.io/432-slides-2025/slides22w.docx)** | **[Code 22](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides22.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

To come.

## Agenda

Comparing Survival Curves, and an introduction to fitting and interpreting Cox Proportional Hazards Models for Time-to-Event Outcomes.

- Remember that we first talked about time-to-event data back in classes [15](https://github.com/THOMASELOVE/432-classes-2025/blob/main/class15/README.md) and [16](https://github.com/THOMASELOVE/432-classes-2025/blob/main/class16/README.md). 

## Sources

- Our [course notes](https://thomaselove.github.io/432-2025/notes.html) cover time-to-event data and Cox Proportional Hazards Models in [Chapters 29-31](https://thomaselove.github.io/432-notes/survival_data.html).
- Section 8 of the Support 1000 study on our Shared Drive demonstrates Cox regression.
- Today's data on the Stanford Heart Transplant Study are adapted from [this link, which provides more details](https://www.openintro.org/data/index.php?data=heart_transplant).
- More on [the haven package](https://haven.tidyverse.org/) which we use today to bring in an SPSS data set.
    - More on the tidyverse solution to dealing with labels imported from SPSS (or SAS) [here](https://haven.tidyverse.org/articles/semantics.html).
- The OpenIntro resources provide some details on [Survival Analysis in R](https://www.openintro.org/book/surv_in_r/)
- [Survival Analysis](https://epirhandbook.com/en/survival-analysis.html) in [The Epidemiologist R Handbook](https://epirhandbook.com/en/index.html)
- [survminer web site](https://rpkgs.datanovia.com/survminer/index.html)
- [survminer cheat sheet (pdf)](https://rpkgs.datanovia.com/survminer/survminer_cheatsheet.pdf)
- More on log-minus-log plots and related topics in survival analysis at [Survival analysis: part II – applied clinical data analysis](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6781220/) Korean J Anesthesiol. 2019 Oct; 72(5): 441–457.
- Chen and Peace (2011) [Clinical Trial Data Analysis Using R](https://www.taylorfrancis.com/books/mono/10.1201/b10478/clinical-trial-data-analysis-using-ding-geng-din-chen-karl-peace)
- Though we won't do it in 432, one could extend the Cox model to permit covariates to vary over time: see [this PDF](https://cran.r-project.org/web/packages/survival/vignettes/timedep.pdf) for details.

## Recent Open-Source Papers using Methods for Time-to-Event Data 

These recent examples from the open-access literature come from [this link](https://github.com/THOMASELOVE/432-sources/blob/main/recent.md).

- Chen L et al. (2021) [Prognostic Nutritional Index (PNI) in Patients With Breast Cancer Treated With Neoadjuvant Chemotherapy as a Useful Prognostic Indicator](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8042235/) Front Cell Dev Biol. 2021; 9: 656741. [DOI](https://doi.org/10.3389%2Ffcell.2021.656741)
- Onaga C et al. (2022) [High expression of SLC20A1 is less effective for endocrine therapy and predicts late recurrence in ER-positive breast cancer](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9126382/) PLoS One. 2022; 17(5): e0268799. [DOI](https://doi.org/10.1371%2Fjournal.pone.0268799)
- Morris TP et al. (2019) [Proposals on Kaplan–Meier plots in medical research and a survey of stakeholder views: KMunicate](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6773317/) BMJ Open. 2019; 9(9): e030215. [DOI](https://doi.org/10.1136%2Fbmjopen-2019-030215)
- Liang H et al. (2022) [Development and validation of a novel prognosis prediction model for patients with myelodysplastic syndrome](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9597308/) Front Oncol. 2022; 12: 1014504. [DOI](https://doi.org/10.3389%2Ffonc.2022.1014504)
- Dzinza R and Ngwira A (2022) [Comparing parametric and Cox regression models using HIV/AIDS survival data from a retrospective study in Ntcheu district in Malawi](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9523851/) J Public Health Res. 2022 Jul; 11(3): 22799036221125328. [DOI](https://doi.org/10.1177%2F22799036221125328)
- Cirillo C et al. (2022) [Predictors of in-hospital mortality in critically ill patients with COVID-19: a large dual tertiary centre study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9716800/) BMJ Open. 2022; 12(12): e059358. [DOI](https://doi.org/10.1136%2Fbmjopen-2021-059358)
