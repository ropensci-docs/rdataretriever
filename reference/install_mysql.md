# Install datasets via the Data Retriever.

Data is stored in MySQL database

## Usage

``` r
install_mysql(
  dataset,
  user = "root",
  password = "",
  host = "localhost",
  port = 3306,
  database_name = "{db}",
  table_name = "{db}.{table}",
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

- user:

  username for database connection

- password:

  password for database connection

- host:

  hostname for connection

- port:

  port number for connection

- database_name:

  database name in which dataset will be installed

- table_name:

  table name specified especially for datasets containing one file

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

No return value, installs datasets into MySQL database

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install_mysql(dataset = "portal", user = "postgres", password = "abcdef")
} # }
```
