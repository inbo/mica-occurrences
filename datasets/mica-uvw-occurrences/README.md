# muskrat-uvw-occurrences
 rato data publication muskrat

# Mica - Muskrat Occurrences collected by UVW in The Netherlands

## Rationale

This repository contains the functionality to standardize the data of _Mica - Muskrat Occurrences collected by UVW in The Netherlands to a [Darwin Core Occurrence](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org).

## Workflow

[source data](data/raw) → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Published dataset

* [Dataset on the IPT](http://NLBIFIPT/resource?r=mica-rato-occurrences)
* [Dataset on GBIF](<!-- Add the DOI of the dataset on GBIF here -->)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── muskrat-occurrences.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── data
│   ├── raw                : Source data, input for mapping script
│   └── processed          : Darwin Core output of mapping script GENERATED
│
└── src
    └── dwc_mapping.Rmd    : Darwin Core mapping script, core functionality of this repository
```

## Installation

1. Click on `Use this template` to create a new repository on your account
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data

## Contributors

[List of contributors](https://github.com/inbo/muskrat-occurrences/graphs/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.

