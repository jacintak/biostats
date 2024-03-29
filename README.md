# Statistical Modelling

These are interactive tutorials created using `learnr`. They are two practicals (3 hours each) about statistical modelling and experimental design. Functional responses are used as the example model.

1. Part 1 - Constructing a statistical model based on functional responses and predator-prey interactions. Design and conduct an experiment (Holling's disc equation experiment)
2. Part 2 - Analyse data collected in Part 1 using multiple linear regression. Visualise the data graphically.

These teaching materials are developed for BYU22S01 Statistics and Computation, Trinity College Dublin, Ireland and provided under a CC0 license. Contact Dr Jacinta Kong for queries: [Email](mailto:kongj@tcd.ie).

The tutorials require R version 4.0 or higher.

To install:

```
remotes::install_github("jacintak/biostats", build_vignettes = TRUE)
```

# Developer notes

2023 version is 3.4
 * Removed troubleshooting tips from start of Part 2. Added reminder about linearised graph.

2022 version is 3.0. Last tag v3.3.3. Built with `learnr` v0.11.2 (CRAN)    
3.0 Updates:

 * Text and question updates
 * Removed simple regression and writing results paragraph
    * Integrated results into 3.0.3
 * Added praise and encouragement (3.0.2)
 * Simplified practical to focus on additive models (3.1.0)
 * Aesthetic updates: HTML boxes, font size, em dash (3.1.1)
 * Text updates and removed multiplicative regression (3.2.0)
 * Removed ANOVA and some quizzes (3.3.0)
 * Built with `learnr` v0.11.2. Vignettes notation updated (3.3.3)
 
2021 version is 2.0. Last tag v2.2.4. Built with `learnr` v0.10.1 (CRAN)

# Known issues

 * Sometimes a trailing garbage issue (see (example)[https://github.com/rstudio/learnr/issues/597]) - reinstall package is easiest solution
 * HTTP error 403. API rate limit exceeded - Seems to be a GitHub access issue. No known workaround.
 * Package not found/write permission denied - Check all packages are up to date and user has administrator rights. Reinstall packages if necessary.
 * Try installing locally if `install_github` does not work
 
# Installing locally
```
remotes::install_local(path = "<path to zip>.zip", build_vignettes = TRUE) # using zip from GitHub
```
