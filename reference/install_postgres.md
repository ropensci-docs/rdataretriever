# Install datasets via the Data Retriever.

Data is stored in PostgreSQL database

## Usage

``` r
install_postgres(
  dataset,
  user = "postgres",
  password = "",
  host = "localhost",
  port = 5432,
  database = "postgres",
  database_name = "{db}",
  table_name = "{db}.{table}",
  bbox = list(),
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

- database:

  the database name default is postres

- database_name:

  database schema name in which dataset will be installed

- table_name:

  table name specified especially for datasets containing one file

- bbox:

  optional extent values used to fetch data from the spatial dataset

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

No return value, installs datasets into PostgreSQL database

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install_postgres(dataset = "portal", user = "postgres", password = "abcdef")
} # }
```
