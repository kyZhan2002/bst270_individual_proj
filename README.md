# BST 270 (Winter 2025): Individual Project by Keyao Zhan

This repository contains my attempt to reproduce tables/figures from FiveThirtyEight's 
[How Americans Like Their Steak](https://fivethirtyeight.com/features/how-americans-like-their-steak/).

## Project Structure

A complete code reproduction attempt is available at `./code/hate_crimes_reproduction.qmd`. This notebook utilize [Quarto](https://quarto.org) and can be compiled via the command line and/or various IDEs/text editors (e.g. RStudio, VSCode, Jupyter, Neovim, Emacs). 
Refer to Quarto's [Get Started](https://quarto.org/docs/get-started/) and [Using R](https://quarto.org/docs/computations/r.html) documentation pages for more information. Quarto documents can also be compiled into multiple different file formats -- the repository also contains HTML, PDF, Tex, and Markdown files.

An image of the original plots is also provided in the `./data` directory.

### Getting Started

1.  Clone the GitHub repository.
2.  Open the `steak_analysis.qmd` file in R Studio (pre-requisite: install `gtsummary` and `ggplot2` R packages).
3.  Click "Preview" or "Run" to execute the notebook.

## Data

The data set used for the reproduction analysis is available at `./data/hate_crimes.csv`. It is available on [GitHub](https://github.com/fivethirtyeight/data/tree/master/hate-crimes).

The following command can also be utilized to obtain the data via command line:

```{bash}
wget -P data https://raw.githubusercontent.com/fivethirtyeight/data/master/hate-crimes/hate_crimes.csv
```

The schema and supporting sources are provided below:

| Header | Definition |
|--------------------------|----------------------------------------------|
| `state` | State name |
| `median_household_income` | Median household income, 2016 |
| `share_unemployed_seasonal` | Share of the population that is unemployed (seasonally adjusted), Sept. 2016 |
| `share_population_in_metro_areas` | Share of the population that lives in metropolitan areas, 2015 |
| `share_population_with_high_school_degree` | Share of adults 25 and older with a high-school degree, 2009 |
| `share_non_citizen` | Share of the population that are not U.S. citizens, 2015 |
| `share_white_poverty` | Share of white residents who are living in poverty, 2015 |
| `gini_index` | Gini Index, 2015 |
| `share_non_white` | Share of the population that is not white, 2015 |
| `share_voters_voted_trump` | Share of 2016 U.S. presidential voters who voted for Donald Trump |
| `hate_crimes_per_100k_splc` | Hate crimes per 100,000 population, Southern Poverty Law Center, Nov. 9-18, 2016 |
| `avg_hatecrimes_per_100k_fbi` | Average annual hate crimes per 100,000 population, FBI, 2010-2015 |

### Original data sources

-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/median-annual-income/?currentTimeframe=0)
-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/unemployment-rate/?currentTimeframe=0)
-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/unemployment-rate/?currentTimeframe=0)
-   [Census Bureau](https://www.census.gov/prod/2012pubs/p20-566.pdf)
-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/distribution-by-citizenship-status/?currentTimeframe=0)
-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/poverty-rate-by-raceethnicity/?currentTimeframe=0)
-   [Census Bureau](https://factfinder.census.gov/faces/tableservices/jsf/pages/productview.xhtml?pid=ACS_10_1YR_B19083&prodType=table)
-   [Kaiser Family Foundation](http://kff.org/other/state-indicator/distribution-by-raceethnicity/?currentTimeframe=0)
-   [United States Elections Project](http://www.electproject.org/2016g)
-   [Southern Poverty Law Center](https://www.splcenter.org/20161129/ten-days-after-harassment-and-intimidation-aftermath-election)
-   [FBI](https://ucr.fbi.gov/hate-crime)
