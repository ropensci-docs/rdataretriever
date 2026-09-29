# Install datasets via the Data Retriever.

Data is stored in CSV files

## Usage

``` r
install_csv(
  dataset,
  table_name = "{db}_{table}.csv",
  data_dir = getwd(),
  debug = FALSE,
  use_cache = TRUE,
  force = FALSE,
  hash_value = NULL
)
```

## Arguments

- dataset:

  the name of the dataset that you wish to install or path to a
  committed dataset zip file

- table_name:

  the name of the database file to store data

- data_dir:

  the dir path to store data, defaults to working dir

- debug:

  setting TRUE helps in debugging in case of errors

- use_cache:

  Setting FALSE reinstalls scripts even if they are already installed

- force:

  setting TRUE doesn't prompt for confirmation while installing
  committed datasets when changes are discovered in environment

- hash_value:

  the hash value of committed dataset when installing from provenance
  directory

## Value

No return value, installs datasets into CSV

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install_csv("iris")
} # }
```
