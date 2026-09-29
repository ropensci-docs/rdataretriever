# Download datasets via the Data Retriever.

Directly downloads data files with no processing, allowing downloading
of non-tabular data.

## Usage

``` r
download(
  dataset,
  path = "./",
  quiet = FALSE,
  sub_dir = "",
  debug = FALSE,
  use_cache = TRUE
)
```

## Arguments

- dataset:

  the name of the dataset that you wish to download

- path:

  the path where the data should be downloaded to

- quiet:

  logical, if true retriever runs in quiet mode

- sub_dir:

  downloaded dataset is stored into a custom subdirectory.

- debug:

  setting TRUE helps in debugging in case of errors

- use_cache:

  Setting FALSE reinstalls scripts even if they are already installed

## Value

No return value, downloads the raw dataset

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::download("plant-comp-ok")
# downloaded files will be copied to your working directory
# when no path is specified
dir()
} # }
```
