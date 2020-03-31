# covUK

Public Health England (PHE) is currently publishing daily updates of the regional breakdown of confirmed Covid-19 cases in English UTLAs.

This repository tracks the evolution of the regional case counts over time.  It should update automatically each day, shortly after the day's results have been published.

## Case distribution

![chloropleth map of England](UK_regional/map.png)

## Case density

![chloropleth map of England](UK_regional/map_density.png)
(colour map: black ~ 3 cases per 1000)

## Regional data over time

![graphs of all UTLAs' case counts, divided by region](UK_regional/plots/UTLAs.png)

## Exponential potential

In exponential growth, the rate of increase is proportional to the total at the time.  By plotting these against each other, we can detect the eventual departure from exponential growth when it occurs.  Any variation in the slope of the graph is due to changes in the exponential growth-parameter, representing a deviation from pure exponentiality.  As growth tails off the eventual *x*-intercept represents the final count.

![graphs of (new cases over previous 6 days) vs (total cases) for England, the regions, and UTLAs](UK_regional/plots/UTLAs_exp.png)
