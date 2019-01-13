# White Noise: An analysis of submissions on Auckland Council's Auckland Plan 2050

This is the repo for the data analysis and visualisations included in a story published by RNZ's [In Depth section](https://www.radionz.co.nz/news/in-depth) on January 21, 2019.

It contains the data and code used to analyse ethnic, income and age group disparities between local board areas, among the ~26,000 submissions made on the Auckland Plan 2050, a document setting out Auckland Council's long-term vision for Auckland, New Zealand. It also contains code for the visualisations that accompanied the final story.

- [Data](#data)
- [Analysis](#analysis)
- [Feedback](#feedback)

### Prerequisites

You'll need the latest versions of [R](https://www.r-project.org/) and [R Studio](https://www.rstudio.com/).
This project was created with R version 3.5.1.

## Data

New Zealand's 2018 Census data release has been delayed so this analysis uses 2013 Census data unless otherwise stated, as this contains the most recent local board ethnicity and income data. The proportional analysis for ethnicity is therefore based on 2013 population counts rather than more recent population estimates, to avoid errors/skews in the data. Age group analysis was done for Auckland only (rather than each local board) so here, 2018 estimates have been used.

The output-data folder provides the .csv files necessary to create the visualistions used in the story - it is possible to run akl-submissions-map.Rmd (see [Analysis](#analysis)) without running the initial script importing and tidying the data provided in the raw-data folder.

|Folder|File|Details|
|---|---|---|
|raw-data|2013_mb_dataset_Auckland_Region (folder)|NZ 2013 Census data for Auckland containing ethnicity and income data for local board areas|
|raw-data|age-estimates-2018.csv|Age data for Auckland by five-year age group, extracted from NZ.stat|
|raw-data|auckland_council_submissions.xlsx|Raw data as supplied by Auckland Council, containing individual ethnicity, age, gender and local board data for each submission|
|output-data|ages.csv|Summarised age group data|
|output-data|ethnic-complete-data.csv|Tall data summarising the ethnic breakdown for each local board|
|output-data|local-board-data.csv|Data summarising submissions for each local board by ethnicity, income and as a proportion of all submissions made|

## Analysis

|File|Details|
|---|---|
|akl-submissions.Rmd|R Markdown containing the R code used to import and analyse the council data|
|akl-submissions.html|HTML output of the Rmd file|
|akl-submissions-maps.Rmd|R Markdown containing the R code used to create draft versions of the visualisations published in the final story|
|akl-submissions-map.html|HTML output of the Rmd file|
|viz|Folder containing draft versions of visualisations used in the final story. Titles and labels were added and dimensions were tweaked in Photoshop.|

---

## Feedback

I am a relatively new R user and still learning so would welcome feedback on the code, which contains elements I am sure are inefficient, or any other aspect of this repo.
[I'm a journalist at Radio New Zealand (RNZ)](https://www.radionz.co.nz/authors/kate%20-newton) - you can contact me at kate.newton@rnz.co.nz
