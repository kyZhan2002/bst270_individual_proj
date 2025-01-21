# BST 270 (Winter 2025): Individual Project

This repository contains my attempt to reproduce tables/figures from FiveThirtyEight's 
[How Americans Like Their Steak](https://fivethirtyeight.com/features/how-americans-like-their-steak/).

## Project Structure

A complete code reproduction attempt is available at `./code/steak_analysis.qmd`. This notebook utilize [Quarto](https://quarto.org) and can be compiled via the command line and/or various IDEs/text editors (e.g. RStudio, VSCode, Jupyter, Neovim, Emacs). 
Refer to Quarto's [Get Started](https://quarto.org/docs/get-started/) and [Using R](https://quarto.org/docs/computations/r.html) documentation pages for more information. Quarto documents can also be compiled into multiple different file formats -- the repository also contains HTML, PDF, Tex, and Markdown files.

Images of the original plot and table that are going to be reproduced are also provided in the `./data` directory. The reproduced figure is provided in the `./fig` directory.

### Getting Started

1.  Clone the GitHub repository.
2.  Open the `steak_analysis.qmd` file in R Studio (pre-requisite: install `knitr`, `dplyr` and `ggplot2` R packages).
3.  Click "Run" to execute the notebook; click "Render" to see the final output html file.

## Data

The data set used for the reproduction analysis is available at `./data/steak-risk-survey.csv`. It is available on [GitHub](https://github.com/fivethirtyeight/data/tree/master/steak-survey). The variables in the dataset are clearly explained by their names.
