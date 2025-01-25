# How Will We Assess the Project A Plans?

Step 1 for me once I see your files appear on Canvas will be to ensure that your planned linear and logistic regression outcomes, as outlined in Sections 6 and 7 of the Plan document, are appropriate for what you're going to be doing in the rest of the Project. If that's not true, I won't look at anything else, because that has to be right before we move on. Instructions on [Choosing Your Data are found here](https://thomaselove.github.io/432-2025/projA.html#choosing-your-data).

Step 2 for me is to ensure that you have a reasonable set of predictors (matching what is required in the instructions) and a reasonable sample size (also matching what is required in the instructions) for both your linear regression model and your logistic regression model. Again, if that's not true, I won't look at anything else, because that has to be right before we move on.

**If you don't get through Steps 1 and 2 here, I'll make you resubmit the work, at a penalty.**

Once I think your choice of data and other issues related to Steps 1 and 2 above, then my last step is to look the Plan over much more carefully. In doing this, I have 20 things in mind, some more complex than others, and some more important than others. I may assess all of them, perhaps with the help of the TAs, or just some. We'll see what happens, but all of these issues are also important in the final Project A, not just in the plan.

I thought sharing my list might help before you start polishing up your Project A Plan submission. Instructions for [the Plan are found here](https://thomaselove.github.io/432-2025/projA.html#the-project-a-plan).

1. Does your **on-time** Canvas submission include your HTML file, your Quarto file, and your .Rds cleaned data set?
2. Are you working alone or with a partner?
    - If you are working with a partner, did your partner also submit a one-page note on Canvas, as requested?
    - If you are working with a partner, are both your names in the "author" section of the YAML?
3. Does your title avoid including the terms "432", "Project", "Proposal" and "Plan", as requested?
4. Does your title exceed 80 characters in length?
5. Is your title meaningful, in that it describes your actual data and plan to some degree?
    - Note that when we refer to the "title" here, we do not include the subtitle for either parts 3, 4 or 5. Although we encourage you to use a subtitle to amplify your ideas, we won't share your subtitle with your fellow students - so the "main title" needs to stand on its own.
6. Does your HTML file display a working Table of Contents with one unnumbered and 10 numbered sections using the section titles Dr. Love placed in the instructions?
7. Does the Table of Contents work, in the sense that clicking on a link within the Table takes the reader to that section?
8. Does the Code tool work, in the sense that there is an item marked `</> Code` next to your title which when opened allows the user to show all code, hide all code and download the Quarto code?
9. Is there an unnumbered section called "R Packages and Setup" which contains `library()` statements for all packages used in the work?
    - I prefer you to load `janitor` and `naniar` first, but that's not critical.
    - Be sure to load `easystats`, rather than loading its individual components, and do so next to last.
    - Be sure to load `tidyverse`, rather than loading its individual components, and do so last.
    - I expect that in the final project, you will also need to load (at least) `broom`, `gt`, `patchwork` and `rms`. There is no need to load `Hmisc` if you're already loading `rms`. You may or may not need these packages (and others) in developing your Plan.
    - You are welcome to load all of these packages (`janitor`, `naniar`, `broom`, `gt`, `patchwork`, `rms`, `easystats` and `tidyverse`) I listed above, even if you don't use them in developing your Plan, but don't load any other packages or functions unless you actually use them in the Plan.
    - The code chunk in this unnumbered section specifically can use `#| message: false` but do not use `#| warning: false` here or do not use either item (`message: false` or `warning: false`) anywhere within the numbered sections of your project Plan without providing a careful explanation.
    - Be sure your code chunk for this section includes `knitr::opts_chunk$set(comment = NA)` and a `theme_set()` function used to pick your ggplot style. I recommend `theme_bw()` or `theme_lucid()`, personally.
10. Is the section numbered 1 in the Table of Contents called Data Source?
    - Does it contain complete information on the source of the data, as described in the instructions?
    - Does it include a clear link (with all necessary details) to the URL which we can use to obtain the raw data freely?
11. Is the section numbered 2 in the Table of Contents called The Subjects?
    - Does it contain a description of the subjects and how they were sampled, as described in the instructions?
12. Is the section numbered 3 in the Table of Contents called Loading and Tidying the Data?
    - Do you do the things specified in the instructions, for example...
    - Do you, within that section, create appropriate subsections for Loading the Raw Data, and for Cleaning the Data, and perhaps several subsubsections within Cleaning the Data?
    - Did you use `janitor::clean_names()` to help change the variable names to more useful ones?
    - Did you sample the data if necessary to meet the data specifications?
    - Did you create appropriate factors for all categorical predictors?
    - Did you build a row (subject) identifier that is unique for each row?
    - Did you remember NOT to print out the tibble in this section?
    - Did you remember NOT to remove or impute any missing values here?
13. Is the section numbered 4 in the Table of Contents called The Tidy Tibble?
    - Do you meet the requirements of the instructions for this section?
    - Do we have a clean listing of the tibble in section 4.1?
    - Do we have appropriate statements about Size and Identifiers in section 4.2?
    - Is the tidied tibble saved properly as an .Rds file in section 4.3, and is that the same tibble we obtain when we ingest the .Rds file you sent via Canvas, including the same name?
14. Is the section numbered 5 in the Table of Contents called The Code Book?
    - Is section 5.1 called Defining the Variables, and does it contain what the instructions call for?
        - In particular, be sure to clearly indicate both the quantitative outcome (for your linear model) and the binary outcome (for your logistic model). The binary outcome would ideally be a factor coded either 0 and 1, or No and Yes at this stage.
    - Is section 5.2 called Numerical Description, and does it contain the `data_codebook()` results? Note that you can choose to include or exclude the subject ID information here. Do the `data_codebook()` results match up with the names and order of variables shown in section 5.1?
15. Is the section numbered 6 in the Table of Contents called Linear Regression Plans?
    - Is section 6.1 called My First Research Question and does it contain what the instructions call for?
    - Is section 6.2 called My Quantitative Outcome and does it contain what the instructions call for?
    - Is section 6.3 called My Planned Predictors (Linear Model) and does it contain what the instructions call for?
        - In particular, does the end of section 6.3 contain brief specifications of your guesses as to the expected direction of relationships between your (quantitative) outcome and each of your planned predictors, along with some brief motivation for those guesses from your understanding of the problem of interest (rather than a data display?)
    - **Important**: Sections 6 and 7 are places where students often try to use the term "statistical significance" or any synonym for it. **Don't do this**. Set up your research questions so they define things (quantities, like percentages or mean differences or slopes in a model) that can be estimated.
16. Is the section numbered 7 in the Table of Contents called Logistic Regression Plans?
    - Is section 7.1 called My Second Research Question and does it contain what the instructions call for?
    - Is section 7.2 called My Binary Outcome and does it contain what the instructions call for?
    - Is section 7.3 called My Planned Predictors (Linear Model) and does it contain what the instructions call for?
        - In particular, does the end of section 7.3 contain brief specifications of your guesses as to the expected direction of relationships between your (binary) outcome and each of your planned predictors, along with some brief motivation for those guesses from your understanding of the problem of interest (rather than a data display?)
17. Are the sections numbered 8-10 in the Table of Contents appropriately labeled "Affirmation", "References" and "Session Information", respectively, and does each of those sections contain what is required in them, according to the instructions?
18. Is your R version 4.4.2 or later, according to your session information?
19. How many spelling errors did we find by running F7 on your Quarto file? How many more did we find in the HTML document itself?
    - Did you use the term "statistical significance" or any synonym for this anywhere in the document? If so, we'll be unhappy. **Don't do this.**
20. Is your HTML file reasonably attractive?
    - Do you exclusively use complete English sentences in each section of the document, outside of code chunks?
    - Have you remembered to leave a **blank line** in your Quarto file...
        - before and after **every code chunk**, **every heading for every section, subsection or subsubsection**, and **every paragraph of text**.
        - Otherwise, you will bring up meaningful irritations for your reader in terms of white space.
    - Have you avoided printing long sections of useless output? This includes printing tibbles anywhere other than section 4.3?
    - Have you avoided incorrect numbering of sections? We need to see that you never have (for instance) something like 7 followed by 7.0.1 instead of 7.1?
    - Have you avoided subsubsubsections? While you're welcome to have 7, 7.1 and even 7.1.1, we'd like you to avoid further splitting into 7.1.1.1., for example.
