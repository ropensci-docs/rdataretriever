# Install datasets via the Data Retriever.

Data is stored in MSAccess database

## Usage

``` r
install_msaccess(
  dataset,
  file = "access.mdb",
  table_name = "[{db} {table}]",
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

- file:

  file name for database

- table_name:

  table name for installing of dataset

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

No return value, installs datasets into MSAccess database

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install_msaccess(dataset = "iris", file = "sqlite.db")
} # }
```
