# Overview
This lab focuses on spatial analysis techniques using the Boston dataset. It includes tasks such as ordinary least squares (OLS) regression, diagnostics tests for spatial autocorrelation, spatial lag regression, spatial error regression, and geographically weighted regression (GWR).

### **Getting Started**
To run the code and reproduce the analysis, follow these steps:

1. Make sure you have R and RStudio installed on your computer.
2. Install the required R packages mentioned in the code.
3. Download the necessary shapefile (`boston_tracts.shp`) from the spData package.
4. Open the R Markdown file in RStudio.
5. Run each code chunk sequentially to execute the analysis and generate plots.

## Part One

### **0.1 To Load the library**
```{r,comment="",echo=TRUE,eval=FALSE}
# Load necessary libraries
library(sp)
library(spatstat)
library(sf)
library(spatstat.geom)
library(ctv)
library(terra)
library(spdep)
library(rgdal)
library(RColorBrewer)
library(classInt)
library(epitools)
library(DCluster)
library(lmtest)
library(car)
library(spatialreg)
library(spgwr)
library(ggplot2)
```

...

## Part Two
### **Create a Data Frame**
```{r,comment="",echo=TRUE,eval=FALSE}
# Create a data frame
boston.df <- data.frame(Boston)
names(boston.df) # gives us the column names
colnames(boston.df) # alternative call; same thing
attach(boston.df) # Now you can call the variable name without using “$”
LOGCMEDV <- log(CMEDV)
...
```

### **Spatial Lag Regression**
```{r,comment="",echo=TRUE,eval=FALSE}
# Plot local coefficient (CRIME)
...
```

## Conclusion
In this lab, we explored various spatial analysis techniques using the Boston dataset. We conducted OLS regression, diagnostics tests for spatial autocorrelation, spatial lag regression, spatial error regression, and geographically weighted regression (GWR). The results indicate significant spatial patterns and relationships between variables. These findings could be valuable for policymakers interested in addressing environmental or social issues such as pollution or affordable housing.

