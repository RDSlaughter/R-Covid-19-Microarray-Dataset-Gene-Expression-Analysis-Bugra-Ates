# Statistical Analysis on Covid-19 Microarray Dataset with R
## Buğra ATEŞ 17.01.2021

In this R project I applied some statistical methods to analize covid-19 microarray dataset. 
I explained all the steps and code lines in .Rmd file. I made it markdown file , so you can see the each processes.

### Boxplot Visualization Before Normalization
![beforenormalize](https://user-images.githubusercontent.com/49213911/105470905-30092200-5cab-11eb-8d6f-621b01f89618.png)

### Boxplot Visualization After Normalization
![afternormalize](https://user-images.githubusercontent.com/49213911/105470924-38615d00-5cab-11eb-9b8b-ba1c84d03844.png)

### Heatmap Visualization
In each heatmap, the columns represent gene expression profile for the patients while the rows represent the expression profiles for each gene across all patients.

![heatmap](https://user-images.githubusercontent.com/49213911/105470980-4b742d00-5cab-11eb-9cf5-9672d9f75626.png)

### Cluster Dendrogram Visualization
![clustering](https://user-images.githubusercontent.com/49213911/105471044-60e95700-5cab-11eb-8494-2cb7dc32f2cf.png)

## Required R packages: 
### [limma](https://bioconductor.org/packages/release/bioc/html/limma.html)
### [dplyr](https://www.rdocumentation.org/packages/dplyr/versions/0.7.8)
### [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html)
### [RColorBrewer](https://cran.r-project.org/web/packages/RColorBrewer/index.html)

## General Information on the Subject 
### What is Microarray?
Microarray is a high-tech technique used for the detection of inclusions and additions that are too small to be observed with a microscope.
### Why do we use Microarray?
Micorarray studies yield a genomic profile based on thousands of gene expressions for each patient.
![whdoweuse](https://user-images.githubusercontent.com/49213911/105472702-5039e080-5cad-11eb-956d-ef96ff954e32.png)
### What is gene expression profile?
In the field of molecular biology, gene expression profile is the measurement of the activity of thousands of genes at once to create a global picture of cellular function. These profiles can, for example, distinguish between actively dividing cells or show how the cells respond to a particular treatment.

![geneexpression](https://user-images.githubusercontent.com/49213911/105472800-66e03780-5cad-11eb-918e-2afa14a5d610.jpg)

### Why do we use gene expression profile?
A gene expression profile may be used to find and diagnose a disease or condition or to see how well the body responds to treatment.

### What is the aim of doing statistical analysis on Microarray Datasets?
1- Identify the changes in gene sequences that are most often associated with particular diseases

2- Determine how often individuals with a particular mutation actually develop breast cancer.

3- Microarrays can also be used to study the extent to which certain genes are turned on or off in cells and tissues.

### We want to extract what?

Microarray statistical analysis wants to identify genes with significantly changed gene expression.



## Resources
#### https://pubmed.ncbi.nlm.nih.gov/12844246/
#### https://wiki.bits.vib.be/index.php/Analyze_your_own_microarray_data_in_R/Bioconductor#Normalization_of_microarray_data
#### https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2435252/
#### https://genomebiology.biomedcentral.com/articles/10.1186/gb-2003-4-4-210
#### https://pubmed.ncbi.nlm.nih.gov/15849016/
#### https://brb.nci.nih.gov/techreport/CIT_course_McShanePolley_May162011.pdf
#### https://www.rdocumentation.org/packages/
#### http://www.sthda.com/
#### https://www.tutorialspoint.com/
#### https://www.datanovia.com/en/blog/how-to-normalize-and-standardize-data-in-r-for-great-heatmap-visualization/
#### http://www.sthda.com/english/wiki/one-way-anova-test-in-r

##
## Buğra ATEŞ 
## https://github.com/RDSlaughter
## https://www.linkedin.com/in/bugraates/
