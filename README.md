# bering-sea: Deadliest Catch?
The Bering Sea is an important region in the North Pacific, both oceanographically and economically. It borders the Arctic, allowing for exchange with hydrographically distinct Polar waters. Because of its position on a shallow continental shelf, the sea supports a diverse ecosystem, highlighted by one of the biggest king crab fisheries in the world. As atmospheric CO2 levels rise, the oceans acidity increases, threatening the stability of marine ecosystems. The Bering Sea is particularly vulnerable to acidification because of its already low pH. My study will use shipboard data from 2008-2010, 2012, and 2013 to estimate trends in pH in the eastern Bering Sea and then relate pH and other hydrographic parameters to fluctuations in population across crab species in the Eastern Bering Sea, in an attempt to tease out broader impacts that acidification could have.

## Questions:

 How does acidity vary with time and space in the Eastern Bering Sea?<br>
 Is there a correlation between acidity and population fluctuations in any economically important crab species?<br>

I expect a slight increase in acididty as atmospheric CO2 rises over the 5 year time span, and prior work has shown tanner crabs and blue king crabs as more vulnerable at lower pH, with Snow Crabs showing more resilence. I would expect to see more pronounced decreases in catch in Tanner Crabs and Blue King crabs.

## Data:

### Crab counts
Fisheries population data is recorded in Catch per Unit Effort - not a direct measure of the crab biomass, but a proxy. <br>
[Crab Populations](https://apps-afsc.fisheries.noaa.gov/maps/crabmap/crabmap.html) <br>

### DIC and Total Alkalinity from Cruises
I will use these values to calculate pH with the PyCO2SYS package.

[2008 JUL](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0144981.html) <br>
[2008 APR](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0144549.html) <br>
[2009 APR-MAY](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0189648.html) <br>
[2009 JUN-JUL](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0189660.html) <br>
[2009 SEPT-OCT](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0189662.html) <br>
[2010 MAY-JUN](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0189661.html) <br>
[2012 OCT](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0157265.html) <br>
[2013 OCT](https://www.ncei.noaa.gov/data/oceans/ncei/ocads/metadata/0157335.html) <br>

[PyCO2SYS Documentation](https://pyco2sys.readthedocs.io/en/latest/)

## Analysis
Combining the shipbord data into one dataset will be crucial for a spatiotemporal interpretation, in addition to creating arrays of the resulting pH values. I plan on creating gridded interpolations of the data to show spatial variability, and use timeseries plots for temporal variabilty. If their appears to be seasonality, I will group the data by season, and then plot seasonal anomalies. I will cross plot the crab CPUE data with the pH and other hydrographic parameter sampled by these cruises. <br>

Humphreys, M. P., Schiller, A. J., Sandborn, D. E., Gregor, L., Pierrot, D., van Heuven, S. M. A. C., Lewis, E. R., and Wallace, D. W. R. (2024). PyCO2SYS: marine carbonate system calculations in Python. Zenodo. doi:10.5281/zenodo.3744275.
