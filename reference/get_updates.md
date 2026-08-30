# Update the retriever's dataset scripts to the most recent versions.

This function will check if the version of the retriever's scripts in
your local directory `~/.retriever/scripts/` is up-to-date with the most
recent official retriever release. Note it is possible that even more
updated scripts exist at the retriever repository
<https://github.com/weecology/retriever/tree/main/scripts> that have not
yet been incorperated into an official release, and you should consider
checking that page if you have any concerns.

## Usage

``` r
get_updates()
```

## Value

No return value, updatea the retriever's dataset scripts to the most
recent versions

## Examples

``` r
if (FALSE) { # \dontrun{
rdataretriever::get_updates()
} # }
```
