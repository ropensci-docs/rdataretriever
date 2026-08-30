# Install datasets via the Data Retriever (deprecated).

Data is stored in either CSV files or one of the following database
management systems: MySQL, PostgreSQL, SQLite, or Microsoft Access.

## Usage

``` r
install(
  dataset,
  connection,
  db_file = NULL,
  conn_file = NULL,
  data_dir = ".",
  log_dir = NULL
)
```

## Arguments

- dataset:

  the name of the dataset that you wish to download

- connection:

  what type of database connection should be used. The options include:
  mysql, postgres, sqlite, msaccess, or csv'

- db_file:

  the name of the datbase file the dataset should be loaded into

- conn_file:

  the path to the .conn file that contains the connection configuration
  options for mysql and postgres databases. This defaults to mysql.conn
  or postgres.conn respectively. The connection file is a file that is
  formated in the following way:

  |          |                       |
  |----------|-----------------------|
  | host     | my_server@my_host.com |
  | port     | my_port_number        |
  | user     | my_user_name          |
  | password | my_password           |

- data_dir:

  the location where the dataset should be installed. Only relevant for
  csv connection types. Defaults to current working directory

- log_dir:

  the location where the retriever log should be stored if the progress
  is not printed to the console

## Value

No return value, main install function

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::install("iris", "csv")
} # }
```
