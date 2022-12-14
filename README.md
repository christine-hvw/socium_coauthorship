# The Formation of Co-authorship Networks - A Case Study of the SOCIUM Research Institute - *Working paper*

## Summary

This study aims at counteracting the neglect of social science co-authorship practices in the literature by accessing the complete scientific publication data of a well-established research center at the University of Bremen. The dataset encompasses a network of 240 authors over the course of ten years (2010-2019). Alongside the bibliographic entries, several other features to investigate the generative process behind this case of co-authorship were encoded during the data collection process. To account for the interdependent as well as temporal nature of the data, I employ the temporal version of an exponential random graph model (TERGM) to explain the emergence of co-authorship, i.e., the formation of ties in this network.

![grafik](https://github.com/christine-hvw/socium_coauthorship/blob/main/figures/plot_nw-1.png?raw=true)

## Repository structure and instructions

|                    |Description         |
|--------------------|--------------------|
|socium-coauthorship/|                    |  
|  ├── data/| raw data used in analyses |
|  ├── figures/| figures included in report | 
|  ├── intermediate/| intermediate objects |
|  ├── renv/| files to restore package versions  |
|  ├── ...  | |
|  ├── renv.lock | package versions |
|  ├── report.pdf|  compiled report  |
|  ├── report.Rmd|  **code and text used to compile report** |  
|  └── ...  | |

To reproduce the analyses, download this repository and run `report.Rmd`. Also, delete the objects in `intermediate/` if you want to re-compute them. They were saved to reduce compilation time of the report.

More information on how to use the `{renv}` package can be found [here](https://rstudio.github.io/renv/articles/renv.html). In short, the function `renv::restore()` will load package versions as specified in `renv.lock` into your R session.

For any further help or questions please contact c.hedde-vonwesternhagen@students.uu.nl.
