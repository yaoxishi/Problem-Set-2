# Problem Set 2

_Remember to submit a single rendered PDF or HTML file (either from .Rmd or a Jupyter Notebook) via GitHub by **Saturday at 12 noon.**_


### Computation

You fielded a survey and collected some wildly descriptive feature vectors. Use the following vectors to address questions 1-3:

```
p{1, 2}
q{3, 4}
```

1. Calculate Manahattan, Canberra, and Euclidean distances "by hand" (i.e., create the data, program each line, and make the calculations). What are the values for each measure?

2. Use the `dist()` function in R to check your work. Were you right or wrong? (be honest in your reporting). If wrong, after debugging, where and why did you go wrong?

3. What are the key differences between these measures, and why does it matter? How might you see these differences "in action" with these fictitious data?


**Download the [old faithful data set](https://stat.ethz.ch/R-manual/R-patched/library/datasets/html/faithful.html) and use to address questions 4-6:**

4. Use some basic EDA techniques to present and discuss the data (e.g., visualize, describe in multiple ways, etc.)

5. Calculate a dissimilarity matrix of these data.

6. Generate an ODI for the Old Faithful data. What do you see?


**Download the Iris data set we used in class (e.g., `data(iris)` in R), and use to address questions 7-10:**

7. Using any munging tools you’d like (e.g., dplyr from the Tidyverse), create a subset of the data excluding the species feature, scaling the features, and calculating a dissimilarity matrix (think `%>%` for stacking functions to do this quickly, e.g.).

8. Fit an agglomerative hierarchical clustering algorithm using complete linkage on your subset data and render the dendrogram of clustering results. What do you see?

9. Try cutting the tree at 2 and 3 branches and show these trees side-by-side. How do they differ?

10. Now fit the algorithm using single and complete linkage and present each dendrogram side-by-side. Discuss the differences. What effects can we see in the clustering patterns when using different linkage methods? 


### Critical Thinking

1. You just assessed the clusterability of some feature space, `R^n`. Address the following questions:

  * How would you go about determining whether clustering made sense to consider or not? 

  * What are techniques you would use, and what might you be looking for from each? 

  * How might these techniques work together to motivate clustering or not? 

  * And ultimately, can/should you proceed if you find little to no support for clusterability? Why or why not?

2. Locate (and read) a paper that applies the hierarchical agglomerative clustering technique. Address the following questions:

  * Describe the author(s) process. 

  * Do they go through similar steps as we covered this week both in setting the stage for clustering (e.g., assessing clusterability, calculating distance, etc.), as well as in fitting the algorithm? If not, what did they omit and does this omission impact their findings in your opinion?

  * Describe at least one possible extension from the study that could emerge based on their findings.

