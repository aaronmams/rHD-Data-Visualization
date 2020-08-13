The primary objective of this lesson is to show how to plot/chart data.

In the
[Data-Import-Export](https://github.com/aaronmams/rHD-Data-Import-Export)
and [Data-Wrangling](https://github.com/aaronmams/rHD-Data-Wrangling)
focused on getting real life data into an R workspace and making it
"useable." This lesson will illustrate some methods for visualizing your
data.

This lesson contains both introductory and non-introductory content.

Contents
--------

### Code

This R code for this lesson is contained in the following files.

#### Skills

1.  `ggplot-examples.Rmd`

`ggplot-examples.Rmd` should be a very approachable lesson appropriate
for basically everybody.

#### Recipes

1.  `mapping-census-data.Rmd`

`mapping-census-data.Rmd` has some non-introductory content. There's
nothing terrifying in there but it does deal a little bit with spatial
data types, GIS data, and extracting JSON data from the web so I'd
probably peg it somewhere between novice and intermediate.

### Data

There are three separate "toy" data files provided for this lesson. They
are:

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

Additionally, there are some GIS files that I have included in this
project. They support the `mapping-census-data.Rmd`. These files are
contained in a directory within this project ("CA\_Counties"), which is
itself a subdirectory within the "data" directory.

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
