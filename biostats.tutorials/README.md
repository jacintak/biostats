# Introduction

Welcome! We need to set up our computer to start using tutorials in R.  

Follow this checklist in order to make sure you are set up:

1. Have you installed R version 4.0 or above? - if not, install R
    * You can check your R package version using `R.version()$version.string`
2. Have you installed RStudio version 1.0.136? - if not installing RStudio
    * You can check your RStudio version using `RStudio.Version()$version`
3. Have you installed the following packages? - if not use `install.packages()` to do so
    * `Tidyverse`
    * `learnr`
    * `devtools`

If everything works then you should see a Tutorials tab in one of your RStudio windows (perhaps next to Environment and History) 

***

# Installing the tutorials

Now we need to install the tutorial. The tutorials are stored in a Package. Use the following code:

```
devtools::install_github("jacintak/biostats", subdir = "biostats.tutorials", dependencies = TRUE)
```
Hopefully the package loaded properly. If not, make sure you have the above packages installed.  
You will only have to do this once at the beginning.

***

# Running a tutorial

You should be able to run a tutorial from the Tutorial tab when you open RStudio without needing to do anything.  
Make sure it's a tutorial from the biostats.tutorials package.  

If you click run tutorial, the tutorial will show up in the tab. You can click the "Show in new window" icon to open it in another window. Press the "Home" icon to return to the Tutorials tab.  

Otherwise use this code and the tutorial will open in another window:

```
learnr::run_tutorial("Introduction", package = "biostats.tutorials")
```
