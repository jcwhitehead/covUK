# covUK

Public Health England (PHE) is currently publishing daily updates of confirmed Covid-19 case numbers in English local authorities.

This repository tracks the evolution of the regional case counts over time.  It digests the PHE data to produce some graphs, chiefly for my personal use, summarising the progression of the epidemic.

It should update automatically each day, shortly after the day's results have been published.

## Case density

(colour map: black ~ 8 cases per 1000)
![chloropleth map of England](UK_regional/map_density_LTLA.png)

## New case density (~last week)
(colour map: black ~ 2 new cases per 1000)
![chloropleth map of England](UK_regional/map_density_LTLA_lw.png)

## R(t) snapshot

(colour map: green R < 1; white R ~ 1; red R > 1)
![chloropleth map of England](UK_regional/map_reff.png)

## Estimate of R(t), over time

Methodology based on RKI's.

![graphs of all UTLAs' estimated effective reproduction index](UK_regional/plots/R.png)

## Regional data over time
### Density of cases

![graphs of all UTLAs' case densities, divided by region](UK_regional/plots/UTLAs_density.png)

### Total number of cases
![graphs of all UTLAs' case counts, divided by region](UK_regional/plots/UTLAs.png)

## Exponential potential

In exponential growth, the rate of increase is proportional to the total at the time.  By plotting these against each other, we can detect the eventual departure from exponential growth when it occurs.  Any variation in the slope of the graph is due to changes in the exponential growth-parameter, representing a deviation from pure exponentiality.  As growth tails off the eventual *x*-intercept represents the final count.

![graphs of (new cases over previous 6 days) vs (total cases) for England, the regions, and UTLAs](UK_regional/plots/UTLAs_exp.png)
