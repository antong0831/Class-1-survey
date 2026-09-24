# Class 1 survey analysis

This repository contains an R Markdown analysis of the Fall 2026 Advanced Data Analysis class survey. It counts respondents and variables, gives the survey columns shorter names, checks variable types, cleans birth day and month responses, summarizes birth seasons, and answers a question about favorite seasons.

## Files

- `Class_1_survey_analysis.Rmd`: annotated R code and written answers for the seven Class 1 lab tasks.
- `Class 1 Survey Fall 2026.csv`: the unmodified survey dataset supplied in the [course repository](https://github.com/kijohnson/Advanced-Data-Analysis).

The course CSV has 31 responses and 27 columns in the version used for this analysis. The R Markdown file renames columns within the R session; it does not edit the original CSV. The analysis treats `30-Nov` as day 30 and `29-Nov` as day 29, converts written birth months to numbers, and leaves genuinely missing responses as missing. It creates `bseason` using Northern Hemisphere meteorological seasons.

## Run the analysis

1. Put the CSV and R Markdown file in the same folder. Keep the CSV filename exactly as shown above.
2. Install R packages `readr`, `dplyr`, and `rmarkdown` if needed.
3. Open `Class_1_survey_analysis.Rmd` in RStudio and select **Knit**, or run `rmarkdown::render("Class_1_survey_analysis.Rmd")` from this folder.

The code prints the survey dimensions, renamed columns, variable types, tables used for cleaning checks, medians, counts by birth season, and favorite-season frequencies. The written answers reflect the course CSV retrieved September 24, 2026; rerun the file if the source changes.

## Data source

Johnson, K. *Advanced Data Analysis* course repository, `Class 1 Survey Fall 2026.csv`. The course provided the survey for educational analysis. The CSV should be committed as supplied, while all cleaning is performed in code.

## AI assistance

OpenAI. (2026). *ChatGPT (Codex)* [Generative AI tool]. https://chatgpt.com/. ChatGPT assisted with drafting the annotated R Markdown analysis and this README on September 24, 2026. The numerical answers were checked against the course CSV; the student remains responsible for reviewing the final submission.
