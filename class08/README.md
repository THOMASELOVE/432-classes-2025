# 432 Class 08: 2025-02-06

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Word | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
08 | 2025-02-06 | **[Slides 08](https://thomaselove.github.io/432-slides-2025/slides08.html)** | **[Word 08](https://thomaselove.github.io/432-slides-2025/slides08w.docx)** | **[Code 08](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides08.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

---

## Announcements

1. Feedback and grades on [Lab 2](https://thomaselove.github.io/432-2025/lab2.html) are available on the Course Grading Roster on our Shared Drive.
2. I am actively reviewing the [Project A Plans](https://github.com/THOMASELOVE/432-classes-2025/blob/main/projectA/plans.md).
    - The list of plans (and the order in which I am reviewing them) is [available here](https://github.com/THOMASELOVE/432-classes-2025/blob/main/projectA/plans.md).
    - I will get back to all 40 project groups to let them know whether they need to substantially revise their linear or logistic regression plans first (I hope today.)
    - Then, after some meaningful additional review time, I will be in touch again with everyone to provide more detailed feedback (as soon as I can.).
    - The two students who have yet to submit their plans need to **stay on the line after class** to speak with me.
3. The slides posted for Class 8 are enormous (224 slides), and will be discussed (at least) in classes 8 and 9. My effort there is to try to provide a logistic regression example which "covers" material from many different aspects of regression modeling.
    - Here is [an outline](outline.md) of the material discussed in these slides, which also includes [an index of key statistical topics discussed](outline.md#index-of-r-functions-and-key-statistical-ideas).
    - The **support1000 example**, on our Shared Drive already includes many things from these slides, plus some other material. That example will be finished in time for Class 12.
    - In Classes 10 and 11, we will be working through a similarly detailed example, involving linear regression.
4. Today's data comes from the [favorite movies data gathered in 431 this past Fall and in prior years](https://github.com/THOMASELOVE/431-classes-2024/tree/main/movies). The version on our 432-data page is an Excel file, [downloadable here](https://github.com/THOMASELOVE/432-data/raw/refs/heads/master/data/movies_2025-01-28.xlsx).
5. We won't get to it until Class 9, but there is an extra file of 50 more movies, as a .csv, also on our 432-data page, [downloadable here](https://github.com/THOMASELOVE/432-data/blob/master/data/movies_extra.csv).
6. Frank Harrell's [Regression Modeling Strategies](https://hbiostat.org/rmsc/) and [Biostatistics for Biomedical Research](https://hbiostat.org/bbr/) books are incredibly useful resources for more on the `rms` and `Hmisc` packages.
7. Sorry, but I clicked away from the screen I intended to share with the results of the in-class survey. You can see them in the Zoom recording if they're useful to you.
8. There was a typo - fixed after class 2025-02-06 in slides 54, 96, 131, 166, and 203 of the [Slides from Class 08](https://thomaselove.github.io/432-slides-2025/slides08.html), where the C = 0.5 + Dxy/2 equation was missing the /2 part.

---

## Today in "How To Be A Modern Scientist"

### On Publishing...

Here are some (I hope useful but perhaps controversial) quotes:

1. There is now very little reason to wait (a long time) for your paper to appear in print.
2. Preprints allow you to collect feedback on your work and improve it quickly.
3. Preprints give junior scientists and other researchers gratification that helps them handle the stress and pressure of their first publications.
4. Share your work on social media.
5. In terms of career advancement, preprints are almost entirely valueless until they are formally accepted for publication.
6. The most successful scientists continue to stay on top of requests and respond to critiques long after their papers are published.

### A few semi-related thoughts...

- I thought this was a compelling summary: [Open Access vs. Traditional Academic Journals Pros and Cons](https://eikipub.com/index.php/learning-resources/open-access-vs-traditional-academic-journals-pros-and-cons)
- I have never been able to convince my fellow authors to submit a preprint, so much so that I've stopped trying to do so.
- One of my most important research collaborations began as a result of some Powerpoint slides I built for myself to keep some ideas straight that I put online with no expectation that anyone else would use them.
- In graduate school, I thought reading papers was one of the main components of my planned career, but that hasn't been the case for many years, despite my regularly serving as an editor for journals and my own moderately substantial publication record.
- Helping people to turn ideas into papers and grants is a major part of my job, though.
- As an associate editor for a journal, it is far more difficult in 2025 to find people willing to review articles than it was in 2005.
