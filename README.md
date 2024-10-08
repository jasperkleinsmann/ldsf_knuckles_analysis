![](figs/CIFOR-ICRAF_logo.png){width=2in}

# Takehome Assignment - Based on the LDSF Knuckles Data Analysis Workshop

# This assignment:
This document contains a number of quesitons based on the Data Analysis workshop in August 2024 held in Colombo, Sri Lanka. You are encourged to use your own code R produced during the workshop, to consult internet and to work together. 

If you get stuck at a question, move to the next one or ask for help in the WhatsApp group. 

### Get started

- Open VScode
- In VScode, navigate to the folder you used during the workshop (*ldsf_Knuckles_analysis*)
- Open a new Quarto (.qmd) document in this folder 
- Save the document as *takehome_assignment.qmd*


### Load libraries

Load the following R libraries:

- *dplyr*
- *ggplot2*
- *sf*
- *leaflet*


### Import data
Import the "*data/ldsf_knuckles_shrubs.csv*" data set

# Question 1
Explore the data using a combinations of the functions `head()`, `names()`, `dim()`, `summary()` and `str()`


# Question 2
Show the dominant shrub species per site using a bar plot (`geom_col()`) and dissect by site using `facet_wrap()`. To make the plot looks nicer, filter only those species that occur more than 30 times.

Question: What is the dominant shrub species for each site?


# Question 3
Use `geom_boxplot()` to visualise the distribution of shrub height for the different vegetation structures. Use the ggplot functions `labs()`, `theme_bw()` and `theme()` to adjust the x/y labels and the layout of the graph.

Question: Which vegetation structure type has the highest shrub height?


# Question 4
Make the `ldsf_shrubs` dataframe spatial by using `st_as_sf()` function in the *sf* package. 


# Question 5
Using your spatial shrubs dataframe created in Question 4, display the plots with *Coffea arabica* in the *Matale* LDSF site on a leaflet map. Hint: use the function `filter()` before mapping the data with leaflet. 


# Question 6
Render the Quarto .qmd script as an html page. Adjust the page layout to make it look better (for instance, add documentation, headers, etc.)


# Question 7
Render the Quarto .qmd script as a pdf by changing the format in the YAML header to *pdf*. 

*Note: You need to have `tinytex` installed to render a .qmd as a pdf*

To download `tinytex`, go to the terminal (PowerShell) and run `quarto install tinytex`. The instalation may take a few minutes depending on your machine and internet connection.
