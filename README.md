# R tutorial – Research Methods, Year 1
 
Step-by-step R tutorials (Quarto `.qmd`, html + pdf) for first-year students with no programming experience. Each week explains an idea and lets students try it in **Your turn** tasks. Students work in one folder, `research_methods`, and build on the class survey data (`class_survey.csv`).
 
## Weeks
 
| Week | File | Topic | Main R |
|---|---|---|---|
| 1 | `r_tutorial_week_01.qmd` | Folders, RStudio, scripts, objects, vectors, indexing, functions, packages | `<-`, `c()`, `[ ]`, `mean()`, `library()` |
| 2 | `r_tutorial_week_02.qmd` | Load, inspect, clean and describe the class data | `read.csv()`, `$`, `summary()`, `ifelse()`, `table()`, `hist()`, `boxplot()`, `write.csv()` |
| 3 | `r_tutorial_week_03.qmd` | Sample vs population, sampling distribution, standard error, 95% CI by hand | `sample()`, `set.seed()`, `rnorm()`, `replicate()` |
| 4 | `r_tutorial_week_04.qmd` | Hypothesis testing: one- and two-sample t-test, effect size, power | `t.test()`, `pt()`, `psych::cohen.d()` |
| 5 | `r_tutorial_week_05.qmd` | Simple regression: dummy vs t-test, correlation, slope test, R², assumptions, influential cases | `lm()`, `summary()`, `confint()`, `cor.test()`, `plot(model)`, `cooks.distance()` |
| 6 | `r_tutorial_week_06.qmd` | Threats to validity: comparable groups, confounding, subgroups, dropout, external validity | `tapply()`, `prop.table()`, `is.na()`, `na.rm = TRUE` |
 
## Design conventions
 
### Panels
 
| Element | Markdown | Look (flatly) | Used for | Title |
|---|---|---|---|---|
| Your turn | `::: your-turn` + `### Your turn {.unnumbered}` | Teal bg `#eaf4f1`, border `#18bc9c` (custom CSS) | The task to do now; after (almost) every explanation | "Your turn" |
| Note | `::: {.callout-note}` | Blue | Examples, analogies, concepts, checklists | "Example: …" or short concept |
| Tip | `::: {.callout-tip}` | Green | Shortcuts, links between ideas | Short descriptive |
| Optional | `::: {.callout-tip collapse="true"}` | Green, folded | Extra material | "Going further (optional): …" |
| Warning | `::: {.callout-warning}` | Orange | Common mistakes, error messages | "Watch out" / "Watch out: …" |
| Important | `::: {.callout-important}` | Red | Must not miss, serious research errors | Short direct |
| Blockquote | `>` | Grey | Once only (week 1, console output) | – |
 
### Inline formatting
 
| What | Format | Example |
|---|---|---|
| Code, functions, objects, files | `` `...` `` | `mean()`, `survey`, `week5.R` |
| Key terms (first use) | `**...**` | **working directory** |
| UI, menus, keys | `*...*` | *Session* > *Set Working Directory*, *Ctrl* + *Enter* |
| Maths | `$...$`, `$$...$$` | $H_0: \beta = 0$ |
| Numbers from data in text | `` `r ...` `` | slope, CI, p in example conclusions |
 
### Plot colours
 
| Colour | Meaning |
|---|---|
| `steelblue` | Data (bars, dots, curves); first group |
| `darkorange` | Second group (week 6) |
| red | Cut-offs, CI edges (dashed); regression line (solid) |
| black | True / population value |
| grey | Background (CI hits, H0 curve, residual lines) |
 