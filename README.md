# Find_Index

#### This file is for finding the index of the marked words and orgnizing them to a dataframe that can apply inter-annotator agreemnet calculation.

* First, multiple annotators annotate article on the website called "Markus".
* Second, download the marked article from the website in .html form.
* Third, use the file "Find_Index_Clean.ipynb" to find the indices of marked words and create a dataframe.
* Finally, follow the steps of the file "inter-annotator agreement.html" to calculate Cohen's kappa and Fleiss kappa.

** p.s.
*** Cohen’s kappa gives the score of interrater agreement between pair raters on categorical data while Fleiss kappa gives the score of interrater agreement among more than two raters.
*** Here, using R rather than Python to calculate kappa value is due to its trait of quick processing dataframe.
