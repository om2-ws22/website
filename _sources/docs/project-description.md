# Project description

## Timeline


| Topic                 | Deadline      | GitHub folder & hints |
| ---                   | ---           |  ---                  |
|[](topic-ideas)        | Fri, Oct 4    | references/           |
|[](project-proposal)   | Fri, Nov 25   | references/           |
|[](draft-analysis)     | Fri, Dec 9    | notebooks/            |
|[](peer-review-draft)  | Fri, Dec 16   | use [](issue-template)|
|[](report)             | Fr, Feb 3     | reports/              |
|[](slides-video)       | Fri, Feb 10   | reports/              |
|[](github-repo)        | Fri, Feb 10   | "Repo in final state" |
|[](comments)           | We, Feb 15    | "Comment in Moodle"   |
|[](team-eval)          | Fri,Feb 17    | "Fill out survey"     |


## Introduction

**TL;DR**: *Pick a data set and use the concepts and methods covered in our course. That is your final project.*

The goal of the final project is for you to use analytical methods to analyze a data set of your own choosing.
The data set may already exist or you may collect your own data by scraping the web.

Choose the data based on your group's interests or work you all have done in other courses or research projects.
The goal of this project is for you to demonstrate proficiency in the techniques we have covered in this class (and beyond, if you like) and apply them to a data set to analyze it in a meaningful way.

All analyses must be done in Python, and all components of the project **must be reproducible** (with the exception of the final presentation) placed inside the provided GitHub repo.

### Logistics

You will work on the project with your team. Use the provided Github-repo and template files for your project. 

The primary deliverables for the final project are

-   A draft analysis ("draft-analysis.ipynb")
-   A written, reproducible report detailing your analysis ("report.ipynb")
-   A GitHub repository corresponding to your report
-   Slides + a video presentation
-   Formal peer review on another team's project


(topic-ideas)=
## Topic ideas 

Identify 2 data sets you're interested in potentially using for the final project.
If you're unsure where to find data, you can use the list of potential data sources in the [Tips + Resources](project-tips-resources.md) section as a starting point.
It may also help to think of topics you're interested in investigating and find data sets on those topics.

The purpose of submitting project ideas is to give you time to find data for the project and to make sure you have a data set that can help you be successful in the project.
**Therefore, you must use one of the data sets submitted as a topic idea, unless otherwise notified.**

The data sets should meet the following criteria:

-   At least 500 observations

-   At least 10 columns

-   At least 6 of the columns must be useful and unique predictor variables.

    -   Identifier variables such as "name", "social security number", etc. are not useful predictor variables.
    -   If you have multiple columns with the same information (e.g. "state abbreviation" and "state name"), then they are not unique predictors.

-   At least one variable that can be identified as a reasonable response variable.

    -   The response variable can be quantitative or categorical.

-   A mix of quantitative and categorical variables that can be used as predictors.

-   Observations should reasonably meet the independence condition.
    Therefore, avoid data with repeated measures, data collected over time, etc.

-   You may not use data that has previously been used in any course materials, or any derivation of data that has been used in course materials.

**Please ask me if you're unsure whether your data set meets the criteria.**

For each data set, include the following:

#### Introduction and data

-   State the source of the data set.
-   Describe when and how it was originally collected (by the original data curator, not necessarily how you found the data)
-   Describe the observations and the general characteristics being measured in the data

#### Research question

-   Describe a research question you're interested in answering using this data.

#### Overview of data

-   Use the Pandas functions to provide an overview of each data set

Submit the HTML or PDF of the topic ideas to Moodle.


(project-proposal)=
## Project proposal

The purpose of the project proposal is to help you think about your analysis strategy early.

Include the following in the proposal:

### Introduction

The introduction section includes

-   an introduction to the subject matter you're investigating
-   the motivation for your research question (citing any relevant literature)
-   the general research question you wish to explore
-   your hypotheses regarding the research question of interest.

### Data description

In this section, you will describe the data set you wish to explore.
This includes

-   description of the observations in the data set,
-   description of how the data was originally collected (not how you found the data but how the original curator of the data collected it).

### Analysis approach

In this section, you will provide a brief overview of your analysis approach.
This includes:

-   Description of the response variable.
-   Visualization and summary statistics for the response variable.
-   List of variables that will be considered as predictors
-   Your model type (what kind of model(s) will you use ... e.g. linear regression)

### Data dictionary

Create a data dictionary for all the variables in your data set. Include the following information for every variable: Name, description, role, type and format.

- `Role`: response, predictor, ID (ID columns are not used in a model but can help to better understand the data)
- `Type`: nominal, ordinal or numeric
- `Format`: int, float, string, category, date or object

### Submission

Push all of your final changes to the GitHub repo, and submit the HTML or PDF file of your proposal to Moodle.

### Proposal grading

| Total                | 10 pts |
|----------------------|--------|
| **Introduction**     | 3 pts  |
| **Data description** | 2 pts  |
| **Analysis plan**    | 4 pts  |
| **Data dictionary**  | 1 pts  |

Each component will be graded as follows:

-   **Meets expectations (full credit)**: All required elements are completed and are accurate.
    The narrative is written clearly, all tables and visualizations are nicely formatted, and the work would be presentable in a professional setting.

-   **Close to expectations (half credit)**: There are some elements missing and/or inaccurate.
    There are some issues with formatting.

-   **Does not meet expectations (no credit)**: Major elements missing.
    Work is not neatly formatted and would not be presentable in a professional setting.


(draft-analysis)=
## Draft analysis 

The purpose of the draft analysis is to give you an opportunity to get early feedback on your analysis. Each team should push their final version of the draft analysis to their GitHub repo by the due date.

The structure of the draft analysis is as follows:

```md
- Introduction
- Setup
- Data
    - Import data
    - Data structure
    - Data corrections
    - Variable lists
    - Data splitting
- Analysis
- Model
    - Select model
    - Training and validation
    - Fit model
    - Evaluation on test set
    - Save model
- Conclusion
```

Below is a brief description of the sections to focus on in the draft. 

- *Introduction*: This section includes an introduction to the project motivation, a data dictionary and research question.

- *Setup*: Import all necessary Python libraries.

- *Data*: Includes all data prepartion steps.

- *Analysis*: Focus on the descriptive statistics and EDA for the response variable and a few other interesting variables and relationships. Interpret the results.

- *Model*: Explain the reasoning for the type of model you're fitting and predictor variables considered for the model. Save the model in your models/ folder.

- *Conclusion*: This section includes initial interpretations and conclusions drawn from the model.


(peer-review-draft)=
## Peer review draft analysis

Critically reviewing others' work is a crucial part of the scientific process, and our course is no exception. Each team will be assigned two other teams's projects to review.

During the peer review process, you will be provided read-only access to your partner teams' GitHub repos.

Provide your review in the form of [GitHub issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue) to your partner team's GitHub repo using the issue template provided (see below).

The peer review will be graded on the extent to which it comprehensively and constructively addresses the components of the partner team's report: the research context and motivation, exploratory data analysis, modeling, interpretations, and conclusions.

(issue-template)=
### Issue template

Spend \~30 mins to review each team's project.

1. Find your team to review in Moodle. 
2. Open the repo of the team you're reviewing, read their project draft, and browser around the rest of their repo.
3. Then, go to the `Issues` tab in that repo, click on `New issue` and fill out the issue by answering the following questions (copy the following content and replace it with your feedback):

Issue template:


```md

### Peer review team

- Peer review by: \[NAME OF TEAM DOING THE REVIEW\]
- Names of team members that participated in this review: \[FULL NAMES OF TEAM MEMBERS DOING THE REVIEW\]

### Goal of the project

- Describe the goal of the project.

### Data

- Describe the data used or collected, if any. Is the data adequate for the project?

### Approach, tools and methods

- Describe the approaches, tools, and methods that will be used.

### Lack of clarity

- Is there anything that is unclear from the proposal? 

### Possible improvements

- Provide constructive feedback on how the team might be able to improve their project.Make sure your feedback includes at least one comment on the modeling aspect of the project, but do feel free to comment on aspects beyond the modeling.

### Presentation

- What aspect of this project are you most interested in and would like to see highlighted in the final presentation?

### Organization

- Provide constructive feedback on any issues with file and/or code organization.

### Further comments

- (Optional) Any further comments or feedback?

```

If you are done, click on `Submit new issue`.


(report)=
## Report

Your final report has to be created in the `report.ipynb` file (see folder `reports/`) and must be reproducible. Assume that it will be used to communicate your results to other data analysts who are interested in your findings.

All team members should contribute to the GitHub repository, with regular meaningful commits.

**You also need to submit the HTML of your final report in Moodle** (the HTML you submit must match the files in your GitHub repository *exactly*).

The mandatory components of the report are below. You are free to add additional sections as necessary.
The report, including visualizations, should be **no more than 10 pages long.** There is no minimum page requirement; however, you should comprehensively address all of the analysis and report.

Be selective in what you include in your final write-up.
The goal is to write a cohesive narrative that demonstrates a thorough and comprehensive analysis rather than explain every step of the analysis.

You are welcome to include an appendix with additional work at the end of the written report document; however, grading will largely be based on the content in the main body of the report.
You should assume the reader will not see the material in the appendix unless prompted to view it in the main body of the report.
The appendix should be neatly formatted and easy for the reader to navigate.
It is not included in the 10-page limit.

The written report is worth 40 points, broken down as follows

| Total                         | 40 pts |
|-------------------------------|--------|
| **Introduction/data**         | 6 pts  |
| **Methodology**               | 10 pts |
| **Results**                   | 14 pts |
| **Discussion + conclusion**   | 6 pts  |
| **Organization + formatting** | 4 pts  |


[Click here](https://docs.google.com/spreadsheets/d/1gaLs43KiLSguhoHNIQlw5DcWPZfGyrLmjv7HTVQ3_uM/edit?usp=sharing) for an overview of the written report rubric.


### Introduction and data

This section includes an introduction to the project motivation, data, and research question.
Describe the data and definitions of key variables.
It should also include some exploratory data analysis.
All of the EDA won't fit in the paper, so focus on the EDA for the response variable and a few other interesting variables and relationships.

#### Grading criteria

The research question and motivation are clearly stated in the introduction, including citations for the data source and any external research.
The data are clearly described, including a description about how the data were originally collected and a concise definition of the variables relevant to understanding the report.
The data cleaning process is clearly described, including any decisions made in the process (e.g., creating new variables, removing observations, etc.) The explanatory data analysis helps the reader better understand the observations in the data along with interesting and relevant relationships between the variables.
It incorporates appropriate visualizations and summary statistics.

### Methodology

This section includes a brief description of your modeling process.
Explain the reasoning for the type of model you're fitting, predictor variables considered for the model.
Additionally, show how you arrived at the final model by describing the model selection process, variable transformations (if needed), assessment of conditions and diagnostics, and any other relevant considerations that were part of the model fitting process.

#### Grading criteria

The analysis steps are appropriate for the data and research question.
The group used a thorough and careful approach to select the final model; the approach is clearly described in the report.
The model selection process took into account any violations in model conditions.
The model conditions and diagnostics are thoroughly and accurately assessed for their model.
If violations of model conditions are still present, there was a reasonable attempt to address the violations based on the course content.

### Results

This is where you will output the final model with any relevant model fit statistics.

Describe the key results from the model.
The goal is not to interpret every single variable in the model but rather to show that you are proficient in using the model output to address the research questions, using the interpretations to support your conclusions.
Focus on the variables that help you answer the research question and that provide relevant context for the reader.

#### Grading criteria

The model fit is clearly assessed, and interesting findings from the model are clearly described.
Interpretations of model coefficients are used to support the key findings and conclusions, rather than merely listing the interpretation of every model coefficient.
If the primary modeling objective is prediction, the model's predictive power is thoroughly assessed.

### Discussion + Conclusion

In this section you'll include a summary of what you have learned about your research question along with statistical arguments supporting your conclusions.
In addition, discuss the limitations of your analysis and provide suggestions on ways the analysis could be improved.
Any potential issues pertaining to the reliability and validity of your data and appropriateness of the statistical analysis should also be discussed here.
Lastly, this section will include ideas for future work.

#### Grading criteria

Overall conclusions from analysis are clearly described, and the model results are put into the larger context of the subject matter and original research question.
There is thoughtful consideration of potential limitations of the data and/or analysis, and ideas for future work are clearly described.

### Organization + formatting

This is an assessment of the overall presentation and formatting of the written report.

#### Grading criteria

The report neatly written and organized with clear section headers and appropriately sized figures with informative labels.
Numerical results are displayed with a reasonable number of digits, and all visualizations are neatly formatted.
All citations and links are properly formatted.
If there is an appendix, it is reasonably organized and easy for the reader to find relevant information.
All code, warnings, and messages are suppressed.
The main body of the written report (not including the appendix) is no longer than 10 pages.

(slides-video)=
## Slides & video presentation

(slides)=
### Slides

In addition to the report, your team will also create presentation slides (e.g. [Google Slides](https://www.google.com/intl/en_en/slides/about/) with an adequate [template](https://slidesgo.com/themes)). Additionaly, you have to record a video (screencast) that summarize and showcase your project (see [](video)).

Introduce your research question and data set, showcase visualizations, and discuss the primary conclusions.
These slides should serve as a brief visual addition to your report and will be graded for content and quality.

If your presentation slides are online, you can put a link to the slides in a `README.md` file in the `reports/` folder.

**For submission, convert these slides to a .pdf document, and submit the file on Moodle.**

The slide deck should have no more than 6 content slides + 1 title slide.
Here is a *suggested* outline as you think through the slides; you **do not** have to use this exact format for the 6 slides.

-   Title Slide
-   Slide 1: Introduce the topic and motivation
-   Slide 2: Introduce the data
-   Slide 3: Highlights from EDA
-   Slide 4: Final model
-   Slide 5: Interesting findings from the model
-   Slide 6: Conclusions + future work

(video)=
### Video presentation

For the video presentation (i.e., screencast), you can speak over your slide deck.
**The video presentation must be no longer than 8 minutes.** It is fine if the video is shorter than 8 minutes, but it cannot exceed 8 minutes.
You may use any platform that works best for your group to record your presentation.
Below are a few resources on recording videos:

-   [Recording presentations in Zoom](https://kb.siue.edu/61721)
-   [Apple Quicktime for screen recording](https://support.apple.com/en-gb/guide/quicktime-player/qtp97b08e666/mac)
-   [Windows 10 built-in screen recording functionality](https://www.youtube.com/watch?v=OfPbr1mRDuo)
-   [Kap for screen recording](https://getkap.co/)

Once your video is ready, upload the video to Moodle.


(github-repo)=
## GitHub repo

All written work (with exception of presentation slides) should be reproducible, and the GitHub repo should be neatly organized.

:::{Note}
Do not change the content or structure of the repo after the stated deadline. 
:::

You will find an overview of the GitHub structure in the README.md file of the GitHub repo (the project structure is based on DrivenData's [Cookiecutter Data Science-Template](https://drivendata.github.io/cookiecutter-data-science/)).

Points for reproducibility + organization will be based on the reproducibility of the report and the organization of the project GitHub repo. The repo should be neatly organized, there should be no extraneous files, all text in the README should be easily readable.

(comments)=
## Presentation comments 

Each student will be assigned 2 presentations to watch (your viewing assignments will be posted later in the semester)

Watch the group's video, then use the Moodle Forum to post a question for the group.
You may not post a question that's already been asked on the discussion thread.

Additionally, the question should be 

- substantive (i.e. it shouldn't be "Why did you use a bar plot instead of a pie chart"?)
- demonstrate your understanding of the content from the course, and 
- relevant to that group's specific presentation, i.e demonstrating that you've watched the presentation.

*This portion of the project will be assessed individually.*

(team-eval)=
## Teamwork evaluation

You will be asked to fill out a survey where you rate the contribution and teamwork of each team member by assigning a contribution percentage for each team member.

Filling out the survey is a prerequisite for getting credit on the team member evaluation.
If you are suggesting that an individual did less than half the expected contribution given your team size (e.g., for a team of four students, if a student contributed less than 12.5% of the total effort), please provide some explanation.
If any individual gets an average peer score indicating that this was the case, their grade will be assessed accordingly.

If you have concerns with the teamwork and/or contribution from any team members, please email me by the project video deadline.
**You only need to email me if you have concerns**.
Otherwise, I will assume everyone on the team equally contributed and will receive full credit for the teamwork portion of the grade.

(grading)=
## Overall grading

The grade breakdown is as follows:

| Total                              | 100 pts |
|------------------------------------|---------|
| **Topic ideas**                    | 5 pts   |
| **Project proposal**               | 10 pts  |
| **Peer review**                    | 10 pts  |
| **Report**                         | 40 pts  |
| **Slides + video presentation**    | 20 pts  |
| **Reproducibility + orga (GitHub)**| 5 pts   |
| **Video comments**                 | 5 pts   |
| **Peer teamwork evaluation**       | 5 pts   |

*Note: No late project reports or videos are accepted.*

### Grading summary

Grading of the project will take into account the following:

-   Content - What is the quality of the research question and relevancy of data to those questions?
-   Correctness - Are statistical procedures carried out and explained correctly?
-   Writing and Presentation - What is the quality of the statistical presentation, writing, and explanations?
-   Creativity and Critical Thought - Is the project carefully thought out? Are the limitations carefully considered? Does it appear that time and effort went into the planning and implementation of the project?

A general breakdown of scoring is as follows:

-   *90%-100%*: Outstanding effort. Student understands how to apply all statistical concepts, can put the results into a cogent argument, can identify weaknesses in the argument, and can clearly communicate the results to others.
-   *80%-89%*: Good effort. Student understands most of the concepts, puts together an adequate argument, identifies some weaknesses of their argument, and communicates most results clearly to others.
-   *70%-79%*: Passing effort. Student has misunderstanding of concepts in several areas, has some trouble putting results together in a cogent argument, and communication of results is sometimes unclear.
-   *60%-69%*: Struggling effort. Student is making some effort, but has misunderstanding of many concepts and is unable to put together a cogent argument. Communication of results is unclear.
-   *Below 60%*: Student is not making a sufficient effort.

### Late work policy

Projects may be submitted up to 2 days late. There will be a 25% deduction for each 24-hour period the project is late. 

Be sure to turn in your work early to avoid any technological mishaps.
