# R_project_template
Template repo for R-based analysis projects

Use this repository as a template to set up a new repo for R-based analysis projects.

The R markdown template file `Project_Template.Rmd` is designed to be used with [RStudio (Posit)](https://posit.co/downloads/) to write and execute R code blocks, and with [knitR](https://yihui.org/knitr/) to execute the full code and generate HTML or PDF reports of the results for easy sharing.

The purpose is to allow easy sharing of project data AND code, so that others in the project team can easily view and edit the data, code and/or outputs; and post/propose modifications. It can also be used to share data and code for publication, to ensure reproducibility of analyses in a paper. In either case, the goal is that others should be able to clone the repo and execute it without needing to download other code (except perhaps installing R packages).

Key principles to keep things simple:
* the Rmd file sets the R working directory to the location of the script, i.e. the project repo itself, via `knitr::opts_knit$set(root.dir = getwd())`
* input data should be stored within the same repository (ideally in a `/data` dir) so it can be easily shared and loaded; OR stored elsewhere online and loaded via URL
* output files should be stored within the repository in suitably labelled directories, e.g. `/figs` and `/tables`, to keep things organised
