---
layout: post
title: Museum of Trees. An Interactive Visualization of Arnold Arboretum
---

![_config.yml]({{ site.baseurl }}/images/screenshot_arboretum.png)
*Screenshot of a web-based interactive visualization of trees in Harvard Arnold Arboretum.  You can access the interactive visualization at [this link](https://hopehhchen.github.io/arboretum/).*

(The web-based interactive visualization is accessible at [this link](https://hopehhchen.github.io/arboretum/).)

Harvard Arnold Arboretum located to the south of Boston is a live manifestation of the beauty of all four seasons in New England.  Throughout the past century, Arnold Arboretum has collected (and received as gifts) trees from around the world.  The result is a collection of more than a hundred different species of trees, as well as other plants you wouldn't otherwise see in the continental North America.  These plants give different parts of Arnold Arboretum different colors throughout the seasons.

Arnold Arboretum keeps a detailed record of these trees and has made the data public, hidden under a search query page *in a long and messy table!*  This project aims at creating a visualization that links the tree species to their countries of origin and their locations in the arboretum.

I started with scraping and cleaning the data from [Arnold Arboretum Database](https://www.arboretum.harvard.edu/plants/data-resources/).  Since the database appears to be manually logged overtime, the difficulty is to deal with various formatting of the species names as well as historical names for countries of origin.  There is also missing data in the table.  Fortunately, these can be easily solved by first unifying the formats (all lower cases with a uniform spacing) and then using a lookup table to connect different names of a species and of a country.

Running a simple statistic over the cleaned table, I learn that more than 50% of the trees in the arboretum belong to roughly two dozens of species (and their sub-species).  I also find that most of these trees are from five countries, namely the US and its oversea territories, China, Japan, Korea and Canada.  I would love to see how these dominant species cross-correlate with these countries of origin and their locations in the arboretum.

The final web-based interactive visualization is hosted at [this link](https://hopehhchen.github.io/arboretum/).  ***The visualization is designed to show the dominant tree species in the arboretum, their locations and their countries of origin, with the cross-correlation between these properties accessible via a simple over-over interaction.***  The visualization also shows a silhouette of each tree species, so even if you are not familiar with the name, you may still identify it!  I also designed the visualization to be color-blind friendly.  Next time you visit Harvard Arnold Arboretum, check out the visualization first and try to find your favorite trees!
