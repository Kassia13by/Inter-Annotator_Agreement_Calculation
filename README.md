# Find_Index

#### This file is for finding the index of the marked words and orgnizing them to a dataframe that can apply inter-annotator agreemnet calculation.

* First, multiple annotators annotate article on the website called "Markus".
* Second, download the marked article from the website in .html form.
* Third, use the file "Find_Index_Clean.ipynb" to find the indices of marked words and create a dataframe.
* Finally, follow the steps of the file "inter-annotator agreement.html" to calculate Cohen's kappa and Fleiss kappa.

#### Character-based calculation

Given the extent to which the uniform of multiple annotators while annotating particular categories, applying Inter Annotator Agreement (IAA) is necessary. In this case, to avoid various problems of word segmentation, the calculation of IAA is character-based. That is, if the words met the requirement of the annotating guideline and were marked, they were assigned to “Y” category, while the unmarked ones fell into “N” category as the table below shows.

| **id** | **text** | **rater\_a** | **rater\_b** |
| ------ | -------- | ------------ | ------------ |
| **1**  | 台        | N            | N            |
| **2**  | 中        | N            | N            |
| **3**  | 5        | N            | N            |
| **4**  | 間        | N            | N            |
| **5**  | 愛        | Y            | Y            |
| **6**  | 店        | N            | N            |
| **7**  | 名        | N            | N            |
| **8**  | 單        | N            | N            |
| **9**  | 分        | Y            | Y            |
| **10** | 享        | Y            | Y            |

#### p.s.
* Cohen’s kappa gives the score of interrater agreement between pair raters on categorical data while Fleiss kappa gives the score of interrater agreement among more than two raters.
* Here, using R rather than Python to calculate kappa value is due to its trait of quick processing dataframe.
