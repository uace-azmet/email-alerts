## AZMet email alerts

This repository houses code to check for missing data on the AZMet API for daily frequency and send email alerts.

`check_reporting.Rmd` is published on Posit Connect [here](https://viz.datascience.arizona.edu/connect/#/apps/01512403-b992-4ab5-baa8-746761ba76a6/access/48) where it is run as a scheduled report.
When the validation conditions in that document aren't met, Posit Connect will send an email generated by `report_email.Rmd` to administrators (currently Eric and Jeremy).

### Contributing

#### `renv`

This project uses [`renv`](https://rstudio.github.io/renv/articles/renv.html) for package management.
When opening this repo as an RStudio Project for the first time, `renv` should automatically install itself and prompt you to run `renv::restore()` to install all package dependencies.

### Deployment

There is no automatic deployment currently set up.
If you make changes to either of the .Rmd documents, you'll need to re-publish `check_reporting.Rmd` to Posit Connect.
