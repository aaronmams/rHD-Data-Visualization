The primary objective of this lesson is to show how to plot/chart data.

In the
[Data-Import-Export](https://github.com/aaronmams/rHD-Data-Import-Export)
and [Data-Wrangling](https://github.com/aaronmams/rHD-Data-Wrangling)
repositories we provided code focused on getting real life data into an
R workspace and making it "useable." This lesson will illustrate some
methods for visualizing your data.

This lesson contains both introductory and non-introductory content.

Contents
--------

### Code

This R code for this lesson is contained in the following files.

#### Skills

1.  `skills/ggplot-examples.Rmd`

`ggplot-examples.Rmd` should be a very approachable lesson appropriate
for basically everybody.

#### Recipes

1.  `recipes/mapping-census-data.Rmd`
2.  `recipes/Covid19-CA-countymap.Rmd`
3.  `R/data-clean.R`

`mapping-census-data.Rmd` has some non-introductory content. There's
nothing terrifying in there but it does deal a little bit with spatial
data types, GIS data, and extracting JSON data from the web so I'd
probably peg it somewhere between novice and intermediate.

`Covid19-CA-countymap.Rmd` is another 'mapping' illustration. It pulls
data on new Covid-19 cases by U.S. county from a GitHub repository and
combines that data with a county-level population file for California,
and a shapefile containing California county boundaries, to make a
'heatmap' of new Covid-19 cases by county for California.

`data-clean.R` is a just a script that:

1.  pulls Covid-19 data from a webhosted .csv file
2.  cleans and prepares that data
3.  joins the Covid-19 data with a county-level population file
4.  joins that data with California county-boundaries

This script does most of the data manipulations necessary to prepare
data for the mapping exercise that is included in
`recipes/Covid-19-countymap.Rmd`. It's really just a script that is
designed to keep the `recipes/Covid-19-countymap.Rmd` file from being
too cluttered with data manipulations.

### Data

There are 4 .csv files and 1 .shp files in the `data` directory that
support the lessons in this repository.

First, there are three separate "toy" data files that support the
examples in `skills/ggplot-examples.Rmd`. They are:

1.  `russian_troll_tweets.csv`
2.  `vms.sample.csv`
3.  `weatherAUS.csv`

These are all comma separated value files.

I got the `weatherAUS.csv` file from the data science platform
[Kaggle](https://www.kaggle.com/).

I got the `russian_troll_tweets.csv` from a GitHub repository maintained
by the data-journalism site
[fivethirtyeight.com](https://fivethirtyeight.com/).

I got the `vms.sample.csv` data from my own work on Vessel Monitoring
System Data. I stipped out all the personally identifiable information
and business identifiable information so that this would be shareable.

Additionally, there is 1 .csv file that supports the
`recipes/Covid-19-countymap.Rmd` example. It is a .csv file with 2019
population estimates for all California counties. It lives here:
`data/CA-county-pop.csv`.

Additionally, there are some GIS files that I have included in this
project. They support the `recipes/mapping-census-data.Rmd` and
`recipes/Covid-19-countymap.Rmd` vignettes. These files are contained in
a directory within this project ("CA\_Counties"), which is itself a
subdirectory within the "data" directory.

Lesson Narrative
----------------

Everybody likes making cool plots, charts, and figures. Sometimes we do
it to help ourselves better understand our data. And sometimes we do it
to tell other people about our data (a picture is worth 1,000 words kind
of thing).

This lesson tries to balance simplicity with coolness. I want the lesson
to be approachable. I also want to demonstrate that, using R, it's
possible to make some pretty interesting visuals with a rather modest
time investment.
