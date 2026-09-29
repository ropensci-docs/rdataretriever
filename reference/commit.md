# Commit a dataset

Commit a dataset

## Usage

``` r
commit(dataset, commit_message = "", path = NULL, quiet = FALSE)
```

## Arguments

- dataset:

  name of the dataset

- commit_message:

  commit message for the commit

- path:

  path to save the committed dataset, if no path given save in
  provenance directory

- quiet:

  logical, if true retriever runs in quiet mode

## Value

No return value, provides confirmation for commit

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::commit("iris")
} # }
```
