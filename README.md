# MICA occurrence datasets

## Rationale

This repository contains the functionality to standardize several datasets of **Muskrat and Coypu occurrences** to [Darwin Core Occurrence](https://www.gbif.org/dataset-classes) datasets that can be harvested by [GBIF](http://www.gbif.org). These datasets are published in the framework of the project [Management of Invasive Coypu and muskrAt in Europe (MICA)](https://lifemica.eu/).

## Datasets

Title (and GitHub directory) | IPT | GBIF
--- | --- | ---
[Muskrat captures in Flanders, Belgium](datasets/mica-legacy-occurrences) | [mica-legacy-occurrences](https://ipt.inbo.be/resource?r=mica-legacy-occurrences) | <https://doi.org/10.15468/pequ4z>
[MICA - Muskrat occurrences collected by RATO in East Flanders, Belgium](datasets/mica-rato-occurrences) | [mica-rato-occurrences](https://ipt.inbo.be/resource?r=mica-rato-occurrences) | <https://doi.org/10.15468/5fps96>
[MICA - Muskrat and coypu occurrences collected by UVW in The Netherlands](datasets/mica-uvw-occurrences) | [mica-uvw-occurrences](http://ipt.nlbif.nl/resource?r=mica-uvw-occurrences) | <https://doi.org/10.15468/qjds4c>
[MICA - Muskrat and coypu camera trap observations in Belgium, the Netherlands and Germany](datasets/mica-agouti-occurrences) | [mica-agouti-occurrences](https://ipt.inbo.be/resource?r=mica-agouti-occurrences) | <https://doi.org/10.15468/5tb6ze>
[MICA - Muskrat occurrences collected by VMM in Flanders, Belgium](datasets/mica-vmm-occurrences) | [mica-vmm-occurrences](https://ipt.inbo.be/resource?r=mica-vmm-occurrences) | <https://doi.org/10.15468/gwzwk4>

## Repo structure

The structure for each dataset in [datasets](datasets) is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── data
│   ├── raw                  : Source data, input for mapping script
│   ├── interim              : Derived data for verification GENERATED
│   └── processed            : Darwin Core output of mapping script GENERATED
│
├── src
│   └── dwc_mapping.Rmd      : Darwin Core mapping script
│
└── specs
    └── dwc_occurrences.yaml : Whip specifications for validation
```

## Contributors

[List of contributors](https://github.com/inbo/mica-occurrences/graphs/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
