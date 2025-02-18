# 432 Class 11: 2025-02-18

[Main Website](https://thomaselove.github.io/432-2025/) | [Calendar](https://thomaselove.github.io/432-2025/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2025/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2025/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2024/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | HTML | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
11 | 2025-02-18 | **[Slides 11](https://thomaselove.github.io/432-slides-2025/slides11.html)** | [Code 11](https://github.com/THOMASELOVE/432-slides-2025/blob/main/slides11.qmd) | **Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

- In today's class, we'll return to the [Slides from Class 10](https://thomaselove.github.io/432-slides-2025/slides10.html). We'll start today's class by returning to **Slide 57** then moving forward from there. 

---

## Announcements

1. On 2025-02-17, I revised the [Slides from Class 10](https://thomaselove.github.io/432-slides-2025/slides10.html) to resolve an issue I'd created by changing the random seeds between creating the slides and publishing them. Most of the slides with text explaining the models have revised coefficients as a result.
    - Don't forget about [the outline](https://github.com/THOMASELOVE/432-classes-2025/blob/main/class10/outline.md) for the slides from Class 10.
    - The only material change from the initially published version is to the `fit3` model (where I switched a variable in, and left one out.)
    - However, many of the text explanations referred to my original results (before I switched random seeds) so I had to correct all of those explanations. This issue (plus a couple of typos I caught) required me to make changes to the text in the following slides: 33, 34, 39-40, 42, 46-48, 55-59, 84-85, 90, 94, 98, 102, 107, 192-193, 199, 218, 220 and 246-250, so you definitely want [the latest version](https://thomaselove.github.io/432-slides-2025/slides10.html).
    - In slide 59 of the **correct** version, you will see a graph where the x axis runs from 8-11 and the red and blue lines cross between values of x at 10 and 11.
2. I have completed a review of revised Project A Plans. You'll find your grade and some comments from me on Canvas, with the other comments on the Google Doc of Project A Plan Feedback on our Shared Drive.
    - If you have questions about my feedback, ask me through email or on Campuswire.
    - If you have questions inspired by my feedback, I won't review your Plan again, but I am happy to try to clarify whether any new ideas on your part seem to resolve my concern if that's helpful, again either through email or Campuswire.
    - Everyone who has a grade on Canvas for the Project A Plan should now switch to working on the Project A Portfolio. I remind you to get Sections 1-7 right (following the [updated Project A instructions provided on 2025-02-11](https://thomaselove.github.io/432-2025/projA.html)) before you launch too far into the new sections for the Portfolio, and I encourage you to make good use of [the Project A Portfolio Template](https://raw.githubusercontent.com/THOMASELOVE/432-data/refs/heads/master/data/432_projectA_portfolio_template.qmd).
3. Grades and feedback for Lab 3 will be posted to our Shared Drive in the Course Grading Roster as soon as possible. The answer sketch and grading rubric for Lab 3 is already available in the Labs and Answer Sketches folder on the Shared Drive.
4. A student asked "When do I need to include `outcome == "Yes"` rather than just `outcome` when fitting a logistic model?
    - The best answer: Always, *unless* you create the outcome to have the two codes 0 and 1 (where 1 means that the outcome occurs.)
    - It is way too easy, otherwise, for the model to fit the log odds of the outcome being No instead of Yes without you realizing it.
5. I'll skip thoughts today on *How to be a Modern Scientist* in the interest of time. More to come in our next few READMEs.

## Reminders

1. [Lab 4](https://thomaselove.github.io/432-2025/lab4.html) is due to Canvas tomorrow (2024-02-19) at Noon.
2. [Lab 5](https://thomaselove.github.io/432-2025/lab5.html) is due to Canvas on 2024-02-26 at Noon, but will be **much, much** easier to do after this Thursday's Class 12.
3. [Quiz 1](https://thomaselove.github.io/432-2025/quiz1.html) will be available to you at noon on Friday 2024-02-28. All I can tell you now is that I intend for it to include 25 questions, each worth 4 points, it covers materials from How to be a Modern Scientist and classes 1-14, and that I don't expect it to be longer or shorter than the 431 Quizzes. Quiz 1 is due on Wednesday 2025-03-05 at Noon.
4. Spring Break means no 432 classes or office hours from 2025-03-08 through 2025-03-14. Dr. Love will also be unavailable on those days.
5. The [Project A portfolio](https://thomaselove.github.io/432-2025/projA.html) is due to Canvas at noon on 2025-03-19.
6. You can work on [Lab 6](https://thomaselove.github.io/432-2025/lab6.html) at any time including now, but it is due to Campuswire on 2025-03-26 at noon. 
7. We will return to in-person classes on Tuesday 2025-03-18. Classes on and after that date will be held in Room E321-323 of the Robbins building at the School of Medicine at CWRU. If you are unsure as to how to get to the room, please email Dr. Love. If you took 431 in 2022, 2023 or 2024 with Dr. Love, it's the same room.
    - I will continue to **try** to record the classes for those who cannot attend due to illness or being out of town, but we do expect you to attend whenever possible and safe. 

## Cat Update

That's [Josephine](https://en.wikipedia.org/wiki/H.M.S._Pinafore) on the left (who's been with us since August) and [Rose Maybud](https://en.wikipedia.org/wiki/Ruddigore) on the right (who we rescued earlier this month.) They are healthy and fairly friendly with each other and us.

![Josephine (left) and Rose Maybud (right) 2025-02-17.](https://github.com/THOMASELOVE/432-classes-2025/blob/main/class11/josephine_rose_maybud_2025-02-17.png)
