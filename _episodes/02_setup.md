---
layout: page
title: Tutorial setup
order: 2
session: 1
length: 10
toc: true
---

## Instructions to Launch Tutorial

For this workshop we have developed an interactive tutorial which contains the notes, exercises and some quiz questions for you to complete. This tutorial, along with others in our programme, can be accessed through our bespoke R package hosted on GitHub.  Below we provide complete instructions on how to install the nesesscary packages and open the relevant tutorial. In order to make this more streamline we asked that you install some of these packages in advance.

First we need to (install and) load two packages from CRAN to ensure Rstudio has the required functions. 

```
install.packages("devtools") 
install.packages("learnr") 
library(devtools)
library(learnr)

```

With these successfully installed we can now install the relevant package with the tutorial for this session.

```
devtools::install_github("ejh243/cfrr-r-tutorials")
```

We can now launch the tutorial with this code. Note it need to build the interactive elements so may take a few minutes. The progress of the build can be seen in the **Jobs** tab in the bottom left panel. 

```
learnr::run_tutorial("Regression Analysis with R", "cfrrRTutorials")
```

When ready the tutorial may launch in a new window, or (more likely) there will be some output in red in the **Jobs** console that says something like:  

```
Output created: Regression-Analysis-with-R.html

Listening on http://127.0.0.1:38555

+------------------------------------------------------------------------+
<U+2713> Open the tutorial in your browser: http://127.0.0.1:38555
! Stop or cancel this job to stop running the tutorial
+------------------------------------------------------------------------+
```

To launch the tutorial you shuold need to copy the web address in this case (http://127.0.0.1:38555) into a web browser of your choice, such as chrome. 

We will now continue the workshop in this document. 
