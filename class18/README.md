# 432 Class 18: 2025-03-20

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
18 | 2025-03-20 | **[Slides 18](https://thomaselove.github.io/432-slides-2025/slides18.html)** | **[Word 18](https://thomaselove.github.io/432-slides-2025/slides18w.docx)** | **[Code 18](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides18.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) is due at noon next Wednesday 2025-03-26. Current submissions are posted [here](https://github.com/THOMASELOVE/432-classes-2025/tree/main/lab6) as well as on Campuswire.
2. The [Project B Proposal Form](https://bit.ly/432-2025-projB-proposal) is due at noon on Wednesday 2025-04-02. Please read the instructions at <https://thomaselove.github.io/432-2025/projB.html> thoroughly before completing the form.
    - We want you to have your data successfully ingested in R before you fill out the form, too. This doesn't mean you've cleaned the data yet, especially, but it does mean that you have the data in R and can summarize the number of complete cases for each of your variables.
    - If you are working with a partner, exactly **one** of you should complete the form. The non-submitting partner should send an **email** to Dr. Love by the deadline with the subject line **432 Project B Partnership** confirming that you are working in a partnership and telling me the name of your partner.
3. The TAs and I remain on target for returning grades and feedback on 432 Project A to you by class time on Thursday 2025-03-27.
4. You might be interested in the [Data Rescue Project](https://www.datarescueproject.org/).
    - "Our goal is to serve as a clearinghouse for data rescue-related efforts and data access points for public US governmental data that are currently at risk. We want to know what is happening in the community so that we can coordinate focus. Efforts include: data gathering, data curation and cleaning, data cataloging, and providing sustained access and distribution of data assets."

## Today's Topics

1. What happens if we fit a linear model to a count outcome? (This and items 2-3 also build on the `medicare` data from Tuesday's Class 17.)
2. How do I think about selecting non-linear terms in light of Spearman $\rho^2$? 
3. How do we fit a Poisson regression with the `rms` package, and do we then get everything we get with `ols()` and `lrm()`?

