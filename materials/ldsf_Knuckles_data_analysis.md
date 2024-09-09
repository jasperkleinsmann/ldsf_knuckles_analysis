![](figs/CIFOR-ICRAF_logo.png)

# LDSF Data Analysis in the Knuckles project

## What will you learn in the workshop?

We will cover a number of topics, including:

- Introduction to the **LDSF** and its applications
- Introduction to R and Quarto

                - Quarto notebooks
                - Loading LDSF data into R
                - Data exploration and visualization
                - Summary statistics
                - Data visualization using ggplot2
                - Mapping data using leaflet
                - Statistical analysis using mixed-effects models

All of the above exercises will be hands-on working with LDSF data from the Knuckles project. We will work in Quarto, which is a great tool for reproducible research. Quarto can be used for [report writing](https://rstudio-conf-2022.github.io/get-started-quarto/materials/04-static-documents.html#/static-quarto-documents), data analysis, and to create [presentations](https://rstudio-conf-2022.github.io/get-started-quarto/materials/05-presentations.html#/presentations), among other things.

See also some slides about the LDSF [here](https://tvagen.github.io/LDSF-presentations/LDSF_advances_LH_assessments.html#/title-slide) and the [LDSF website](https://ldsf.thegrit.earth) for more information.


## Before we get started...

We will be working in _R Statistics_ for the analysis of LDSF data. The R programming language is a dynamic language built for statistical computing and graphics. R is often used in statistical analysis, scientific computing, machine learning, and data visualization. For a comprehensive introduction to R for data science, [this book is highly recommended](https://r4ds.hadley.nz/). It takes you through the basics of R programming as well as more advanced topics for those already familiar with R. We will not be following the book in the workshop, but it is a great resource for learning R.

## Software needed for this workshop
#### Please install the following software ahead of the workshop:
1. **R Statistics**: You will need to install it on your computer. Navigate to the [R Project website](https://cloud.r-project.org/) and download the latest version of R for your operating system. Follow the installation instructions for your operating system.
2. **VS Code**: This is a versatile code editor that can be used for any programming language. It is lightweight and has a lot of features that make it a great choice for coding. You can download it from the [VS Code website](https://code.visualstudio.com/).
3. Install **Quarto** from the [Quarto website](https://quarto.org/). Quarto is a document processing tool that allows you to write documents in markdown and R code. We will be using Quarto withon VS Code to write our reports and analyses.

#### Once R, VS Code and Quarto are installed, please install the following extensions in VS Code:

a) Open VS Code and navigate to the _Extensions_ tab on the left sidebar.

![The VS Code Extensions tab](figs/vs_code_extensions.jpg)

- Search for and install the [R extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r).
- Search for and install the [Quarto extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=quarto-dev.quarto-vscode).

b) Open R in the terminal

![How to start the R console in the terminal within VS Code.](figs/vs_code_terminal_R.jpg)

Once R is started in the terminal, run the following command to install the languageserver package:

```R
install.packages("languageserver")
```

We will work with some additional libraries/packages in the workshop. Please install these beforehand if you can:

```R
install.packages("dplyr") ## For data wrangling
install.packages("ggplot2") ## For plotting
install.packages("leaflet") ## For mapping
install.packages("lme4") ## For statistical modeling
```

_(We will install additional libraries during the workshop as needed.)_
