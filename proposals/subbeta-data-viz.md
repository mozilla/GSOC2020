# GSOC 2020 Proposal Template. Put your proposal name here

**Mentor:** Corey Dow-Hygelund

**Email:** cdowhygelund@mozilla.com

## Project Description

This project will investigate and implement the best methods for visualizing statistical matching model performance, 
and the resultant inferred measurements. The final result of the project is a suite of dashboards for use 
in model development and interpretation.  

## Skills Required

Required experience:

* Git/GitHub
* Data manipulation (e.g., Pandas or R)
* Data visualization

Nice to have experience:
* Javascript
* [d3](https://d3js.org/)

## Project Details

The [subBeta project](https://docs.google.com/document/d/1Ygz6MkudYHZjnDnD9Z97kUyFrvV3KGWsjXyPjddhHq0/edit#heading=h.lvb9l8gw2nee)
attempts to utilize prerelease versions of Firefox to inform Release behavior and characteristics _before_ it has been 
launched to the general public (e.g., forecasting). It circumvents issues regarding differing user populations 
between the channels by novel applications of 
[statistical matching](https://en.wikipedia.org/wiki/Matching_(statistics)) techniques. This project would assist 
in two fronts:
1. Model development and validation by helping to enable rapid analyses. 
2. Interpretation of the model results by employing optimal data visualizations, and ease of segmentation across
various metrics (e.g., User country, User machine characteristics). 

Currently, the subBeta project has investigated forecasting 
[performance metrics](https://docs.google.com/document/d/1W-EREsJLuRvTPvGXaW71FvuAGXkoLNDZmZl-sbaeMZM/edit#). However,
there are parallel efforts to address user engagement metrics. This project would support these and additional use 
cases.

## Additional Information

The ultimate goal that this project will directly address is to build production level dashboards for use by 
Data Science and other stakeholders regarding applications of the techniques employed in the subBeta project. 
