+++
title = "My economic impact package, iotables, has a much updated released on CRAN"

date = 2019-01-04T19:00:00
lastmod = 2019-01-04T19:00:00
draft = false

authors = ["Daniel Antal"]

tags = ["economic-impact", "R", "multipliers", "open-data"]

summary = "The analytical functions of the package create the usual economic impact analysis, including direct effects, multipliers on gross value added, employment, CO2 or other factors. The package creates a programmatic interface to compare economic impact changes in time, or compare any country with any country in the European Union."

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects = ["R"]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""

  # Show image only in page previews?
  preview_only = false

+++


[![DOI](https://zenodo.org/badge/108267715.svg)](https://zenodo.org/badge/latestdoi/108267715)

This package was related to several of my works for Slovak, Hungarian and Croatian music industry and the Hungarian Film Fund, and my collaboration with Eeconomic impacT s.r.o in the Czech Republic. My R package downloads symmetric input-output and related tax, margins, use tables from the Eurostat bulk data warehouse, and organizes them for macroeconomic analysis.

The analytical functions of the package create the usual economic impact analysis, including direct effects, multipliers on gross value added, employment, CO2 or other factors. The package creates a programmatic interface to compare economic impact changes in time, or compare any country with any country in the European Union.

The package is accompanied by three articles (or ‘vignettes’).  The [Germany 1990](http://iotables.ceemid.eu/articles/germany_1990.html) re-creataes almost all of the practical examples of the [Eurostat Manual of Supply, Use and Input-Output Tables](http://ec.europa.eu/eurostat/documents/3859598/5902113/KS-RA-07-013-EN.PDF/b0b3d71e-3930-4442-94be-70b36cea9b39?version=1.0) by Jörg Beutel.  This may be used as a tutorial to input-ouput analysis or understanding the package interface. Furthermore, it creates as a verification tool in the package testthat infrastructure to make sure that the functions correctly return all published, verified examples by Prof. Beutel.

The [United Kingdom Input-Output Analyitcal Tables](http://iotables.ceemid.eu/articles/united_kingdom_2010.html) article similarly recreates the analytical results, such as GVA and employment cost effects for the [United Kingdom 2010](https://webarchive.nationalarchives.gov.uk/20160114044923tf_/http://www.ons.gov.uk/ons/rel/input-output/input-output-analytical-tables/2010/index.html) table.  While the current UK tables and standard Eurstat tables are somewhat different, this table is accompanied by Richard Wild’s excellent article and published analytical results.

The [Working with Eurostat data article](http://iotables.ceemid.eu/articles/working_with_eurostat.html) shows how to work with real-life, current, SNA2010 compatible data from the Eurostat data warehouse. It contains some comparative results between Czechia and Slovakia.  The package is in itself is extending the functionality of the eurostat package, and it is released with eurostat in the rOpenGov community.
