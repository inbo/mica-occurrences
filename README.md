# landsnails-occurrences
Research Project Landsnails

# Landsnails in Spain & Gran Canaria


## Rationale


This repository contains the functionality to standardize the data of the Landsnails of Spain dataset to a [Darwin Core Occurrence](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org).

## Workflow

<!-- This section describes how we go from raw data to standardized Darwin Core data -->

[source data](data/raw) <!-- Additionally, you can write here where that raw data came from, e.g. "(downloaded as [Supplementary Material 1](http://neobiota.pensoft.net//lib/ajax_srv/article_elements_srv.php?action=download_suppl_file&instance_id=31&article_id=4007))" --> → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Published dataset


* [Dataset on the IPT](<!-- Add the URL of the dataset on the IPT here -->)
* [Dataset on GBIF](<!-- Add the DOI of the dataset on GBIF here -->)

## Repo structure

<!-- This section helps users (and probably you!) to find their way around this repository. You can leave it as is, unless you're starting to adapt the structure a lot. -->

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── checklist-recipe.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── data
│   ├── raw                : Source data, input for mapping script
│   └── processed          : Darwin Core output of mapping script GENERATED
│
├── docs                   : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd    : Darwin Core mapping script, core functionality of this repository
    ├── _site.yml          : Settings to build website in docs/
    └── index.Rmd          : Template for website homepage
```

## Installation

<!-- This section is for users who want to download/adapt your checklist repository. You can leave it as is. -->

1. Click on `Use this template` to create a new repository on your account
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `docs/` (advanced)

## Contributors

Ward Langeraert
Dimitri Brosens

[List of contributors](https://github.com/BelgianBiodiversityPlatform/landsnails-occurrences/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
