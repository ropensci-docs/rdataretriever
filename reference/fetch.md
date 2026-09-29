# Fetch a dataset via the Data Retriever

Each datafile in a given dataset is downloaded to a temporary directory
and then imported as a data.frame as a member of a named list.

## Usage

``` r
fetch(dataset, quiet = TRUE, data_names = NULL)
```

## Arguments

- dataset:

  the names of the dataset that you wish to download

- quiet:

  logical, if true retriever runs in quiet mode

- data_names:

  the names you wish to assign to cells of the list which stores the
  fetched dataframes. This is only relevant if you are downloading more
  than one dataset.

## Value

Returns a dataframe of `dataset`

## Examples

``` r
if (FALSE) { # \dontrun{
## fetch the portal Database
portal <- rdataretriever::fetch("portal")
class(portal)
names(portal)
## preview the data in the portal species datafile
head(portal$species)
vegdata <- rdataretriever::fetch(c("plant-comp-ok", "plant-occur-oosting"))
names(vegdata)
names(vegdata$plant_comp_ok)
} # }
```
