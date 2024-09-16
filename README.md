# Acute Myeloid Leukemia Heatmap Analysis

## Project Overview

This project performs a heatmap analysis on acute myeloid leukemia (AML) RNA-sequencing data. The analysis is adapted from a refine.bio-examples notebook and uses a dataset from Shih et al., 2017, pre-processed by refinebio.

### Goals

1. Process and analyze RNA-sequencing data from 19 AML model mice.
2. Create a clustered heatmap to visualize gene expression patterns.
3. Annotate the heatmap with mutation and treatment information.

## Last Updated

October 2021

## Software Requirements

- R (version used in the project should be specified)
- R packages:
  - pheatmap
  - magrittr
  - readr
  - tibble
  - dplyr
  - sessioninfo

## File Structure

```
├── data/
│   └── SRP070849/
│       ├── SRP070849.tsv
│       └── metadata_SRP070849.tsv
├── plots/
│   └── aml_heatmap.png
├── results/
│   └── top_90_var_genes.tsv
└── 01-heatmap.Rmd
```

## Running the Analysis

1. Ensure all required R packages are installed.
2. Download the dataset from refine.bio: [SRP070849](https://www.refine.bio/experiments/SRP070849)
3. Place the downloaded data in the `data/SRP070849/` directory.
4. Run the R Markdown file `01-heatmap.Rmd`.

## Output

- A heatmap visualization saved as `plots/aml_heatmap.png`
- A TSV file with the top variable genes: `results/top_90_var_genes.tsv`

## Potential Optimizations

1. Use parallel processing for variance calculations on large datasets.
2. Implement data.table or dplyr for faster data manipulation.
3. Consider using a more efficient heatmap package like ComplexHeatmap for larger datasets.
4. Optimize gene selection criteria based on specific research questions.
5. Implement caching of intermediate results to speed up re-runs.

## Contributing

[Add information about how to contribute to the project, if applicable]

## License

[Specify the license under which this project is released]

## Contact

[Provide contact information for the project maintainer]