+++
title = "Programatic Approach To Work With European Regional Data Panels"

date = 2020-02-13T12:30:00
lastmod = 2020-02-13T12:30:00
draft = false

authors = ["Daniel Antal, CFA"]

tags = ["market-report", "CEEMID", "rOpenGov"]

summary = "My open source program code was released within the 3.6.1 version of eurostat R package, making the painful boundary alignment with frequent region border changes, and resulting data imputation work automatic and less error-prone. As a result, more and more of my work, and particularly the music indicators of CEEMID are becoming available on provincial/regional level."

projects = ["opendata"]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Center"

  # Show image only in page previews?
  preview_only = false

+++


A very important part of my work is to pre-process data, and integrate various data tables into tidy, comprehensive data tables or databases.  This is particularly difficult but rewarding when I work with statistics on sub-national, regional level.  While country borders are very rarely change in the world, regional boundaries are changing on average every three years withing the European Union. Putting together data with 2010, 2013, 2017 and the forthcoming 2021 regional boundaries is a very difficult task.

![Regional borders are changing very frequently](/img/nuts_history.png)

I released as open source code some of my work withing the [rOpenGov](http://ropengov.github.io/) collaboration in the form of the 3.6.1 version of the R package [eurostat](http://ropengov.github.io/eurostat/), which precisely helps users and researchers with this very painful, error-prone task.  As a result, more and more of my work, and particularly the music indicators of CEEMID, are becoming available not only for the EU member states but for regions, too.  

![More difficult to create than you think](/img/dataanimation/gerd_by_region.gif)

The software code was originally created within a project with IVIR, where we try to understand the drivers of book piracy in Europe.  As 2018 data started pouring into Eurostat’s warehouse, we realized that the NUTS2017 boundary changes made all our reproducible research code fail.   After cleaning, imputing many variables relevant for the internet society, research and book publishing, I created a code that is dealing with all current Eurostat regional products. In the future, I would like to extend this to city/metropolitan area statistical products, too.

If you work with the R language, you can read [my tutorial](http://ropengov.github.io/eurostat/articles/website/regional_data.html) and dwell into regional data right now. If not, you can always ask me to create a tidy, correctly merged and imputed data panel for regional statistics over the last decade in Europe.