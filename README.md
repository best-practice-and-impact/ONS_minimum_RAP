# Minimum reproducible analytical pipelines (RAP) guidance for the Office for National Statistics (ONS)

This repository contains draft minimum RAP standards for the ONS. This is not currently finalised, nor is this guidance official ONS policy at this time. The contents of this repository should only be used for feedback purposes.

## Building the site

Make sure you have quarto installed and working. With the R project open in RStudio, run the following command: 

`
quarto::quarto_render("site")
`

Alternatively, if you do not have the repository location as your working directory, run the following command:

`
quarto::quarto_render("path_to_repository/site")
`

## Editing the site

All site contents can be found in the `site/` folder. When adding or removing pages, or changing filenames, remember to edit the `_quarto.yml` file under the website settings, e.g.:

`
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
`
