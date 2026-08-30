# Install datasets via the Data Retriever.

Data is stored in SQLite database

## Usage

``` r
install_sqlite(
  dataset,
  file = "sqlite.db",
  table_name = "{db}_{table}",
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

- file:

  Sqlite database file name or path

- table_name:

  table name for installing of dataset

- data_dir:

  the dir path to store the db, defaults to working dir

- debug:

  setting TRUE helps in debugging in case of errors

- use_cache:

  setting FALSE reinstalls scripts even if they are already installed

- force:

  setting TRUE doesn't prompt for confirmation while installing
  committed datasets when changes are discovered in environment

- hash_value:

  the hash value of committed dataset when installing from provenance
  directory

## Value

No return value, installs datasets into SQLite database

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install_sqlite(dataset = "iris", file = "sqlite.db")
} # }
```
