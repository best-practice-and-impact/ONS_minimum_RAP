# Minimum Reproducible Analytical Pipelines (RAP) standards for the Office for National Statistics (ONS)

## Building the site

Make sure you have [quarto](https://quarto.org/) installed and working before you start. 

We have used [RStudio](https://posit.co/products/open-source/rstudio/) and [R](https://www.r-project.org/) to build the site. To follow the same approach, make sure you have R and RStudio installed. Install the [quarto](https://cloud.r-project.org/web/packages/quarto/index.html) package and associated dependencies for R. 

Open the R project ONS_minimum_RAP.Rproj in RStudio.

Run the following command: 

```
quarto::quarto_render("site")
```    

Alternatively, if you do not have the repository location as your working directory, run the following command:

```
quarto::quarto_render("path_to_repository/site")
```

## Editing the site

All site contents can be found in the `site/` folder. When adding or removing pages, or changing filenames, remember to edit the `_quarto.yml` file under the website settings, e.g.:

```
website:
  title: ONS minimum RAP standards
  navbar:
    left:
      - href: index.qmd
        text: Home
      - href: page_1.qmd
        text: Page 1
      - href: page_2.qmd
        text: Page 2
```
