## Test environments

* ubuntu 18.04, R 4.0.3

## R CMD check results

R CMD check done via `devtools::check()`, resulting in 0 errors, 0 warnings, and 1 note. That note complains that the package is greater than 5 MB in size and that the data directory itself is over 5 MB in size. I wish I knew how to fix this, other than to note the following to CRAN. First, the directory *was* over 5 MB in size. However, I re-saved all the contents of the data directory by way of `tools::resaveRdaFiles("data")` for optimal file compression. The ensuing size of the data directory was cut roughly in half. The source package I submit to CRAN should be around 2.5 MB in size as well. I do not know why `devtools::check()` does not reflect this change.

`devtools::spell_check()` suggests several spelling errors. However, what I submit to CRAN includes only the false positives. Almost all of these false positives occur in the R Documentation file for when I source or add references about the data. I'll note, humbly, that `devtools::spell_check()` did catch more than a few spelling errors in those R Documentation files that were not appropriate for CRAN. I went through and corrected all of them. What remains are just false positives that come from the peculiarities of writing exhaustive R Documentation files for an R package that is primarily about data to be shared with the community of R users.

## Downstream dependencies

This is a new package with no downstream dependencies to note.