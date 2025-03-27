# 432 Class 20: 2025-03-27

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
20 | 2025-03-27 | **[Slides 20](https://thomaselove.github.io/432-slides-2025/slides20.html)** | **[Word 20](https://thomaselove.github.io/432-slides-2025/slides20w.docx)** | **[Code 20](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides20.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. Lab 6 submissions and status [are available here](https://github.com/THOMASELOVE/432-classes-2025/tree/main/lab6). Those not yet complete have until 2025-04-15 to get this done (with a late penalty.) Your fellow students should be able to help you via Campuswire.
2. Project A grades will not be available today or tomorrow. I hope you'll have them before Tuesday.
3. The [Project B Proposal Form](https://bit.ly/432-2025-projB-proposal) is due at noon on Wednesday 2025-04-02. Please read the instructions at <https://thomaselove.github.io/432-2025/projB.html> thoroughly before completing the form.
    - We want you to have your data successfully ingested in R before you fill out the form, too. This doesn't mean you've cleaned the data yet, especially, but it does mean that you have the data in R and can summarize the number of complete cases for each of your variables.
    - If you are working with a partner, exactly **one** of you should complete the form. The non-submitting partner should send an **email** to Dr. Love by the deadline with the subject line **432 Project B Partnership** confirming that you are working in a partnership and telling me the name of your partner.

## Today's Agenda

- A new example of regression on an ordered multi-categorical outcome
- Fitting Proportional Odds Logistic Regression Models with `MASS::polr()` and with `rms::lrm()`
- Assessing the Proportional Odds Assumption with a multinomial logistic regression fit
- Fitting Ordinal Logistic Regression Models with `rms::orm()` when we want to penalize incorrect classifications differently depending on "how wrong" we are


