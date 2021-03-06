# Introduction

Welcome! We need to set up our computer to start using tutorials in R.  

Follow this checklist in order to make sure you are set up:

1. Have you installed R version 4.0 or above? - if not, install/update R
    * You can check your R package version using `R.version()$version.string`
2. Have you installed RStudio version 1.0.136 or above? - if not install/update RStudio
    * You can check your RStudio version using `RStudio.Version()$version`
3. Have you installed the following packages? - if not use `install.packages()` to do so
    * `learnr` - needed to run the tutorials
    * `remotes` (or `devtools`) - needed to install the tutorials
    * `knitr` - for displaying content

If everything works then you should see a Tutorials tab in one of your RStudio windows (perhaps next to Environment and History) 

***

# Installing the tutorials

Now we need to install the tutorial. The tutorials are stored in a Package available on GitHub. You will only have to install the package once at the beginning.   
Use the following code:

```
remotes::install_github("jacintak/biostats", dependencies = TRUE)
```

If you are asked to install any other packages, choose yes but don't do any compiling (press no if asked).  
If the package installed properly, you should automatically see the tutorials in the Tutorial tab.

***

# Running a tutorial

You should be able to run a tutorial from the Tutorial tab when you open RStudio without needing to do anything.  
Make sure it's a tutorial from the `biostats.tutorials` package.  

If you click run tutorial, the tutorial will show up in the tab. You can click the "Show in new window" icon to open it in another window. Press the "Home" icon to return to the Tutorials tab.  

If that doesn't work use this code and the tutorial will open in another window:

```
learnr::run_tutorial("<insert name of the tutorial to run>", package = "biostats.tutorials")
```

If neither works, check that the `biostats.tutorials` package installed properly.  

Quit a tutorial by pressing the "Stop" icon.