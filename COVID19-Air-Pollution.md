---
title: 'Causes of reduction in airborne NO<sub>2</sub> and CO emissions in Europe during COVID-19 crisis'
date: 2020-12-01
toc: true
toc_sticky: true
toc_label: "Causes of reduction in airborne NO<sub>2</sub> and CO emissions in Europe during COVID-19 crisis"
header:
overlay_image: https://raw.githubusercontent.com/Bashinim/COVID19-EU/main/Cropped%20Images/Background.jpg
  overlay_filter: 0.3 
  caption: "Causes of reduction in airborne NO<sub>2</sub> and CO emissions in Europe during COVID-19 crisis"
read_time: false

## Causes of reduction in airborne NO<sub>2</sub> and CO emissions in Europe during COVID-19 crisis

Most presumed causes of reduction in observed reduction in air pollution are reduction in surface traffic and people staying at home due to the travel bans imposed. In this analysis changes of NO<sub>2</sub> and CO emissions are compared against the three variables:

- Average population in Europe
- Road density in Europe
- Vessel routes density in the Mediterranean Sea and the black sea

### Processing candidate variables

<center>
<figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/1.annex.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/1.annex.jpg?raw=true"></a>
    <figcaption>Estimated average number of persons for square kilometer in 2020 in Europe [<a href = "https://developers.google.com/earth-engine/datasets/catalog/CIESIN_GPWv411_GPW_Basic_Demographic_Characteristics">NASA SEDAC at the Center for International Earth Science Information Network</a>].  </figcaption>
    </figure> </center>

<center>
<figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.3.1.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.3.1.jpg?raw=true"></a>
    <figcaption>Road network of Europe extracted from OSM data; the highways tagged as motorway, trunk, primary,
secondary, tertiary, unclassified, and residential in OSM [<a href = "https://zenodo.org/record/4284076#.X8VIHbMo_IW">Processed dataset</a>].  </figcaption>
    </figure> </center>

<center>
<figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.2.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.2.jpg?raw=true"></a>
    <figcaption>Road density of Europe; number of roads within 7 km radius from each considered geolocation point. Each
distinctive road is identified by a unique ‘Osm id’. </figcaption>
    </figure> </center>

<center>

<figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.1.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.1.jpg?raw=true"></a>
    <figcaption>Vessel routes density in the Mediterranean Sea and the Black Sea; number of vessel routes within 7 km radius from each
considered geolocation point. Each distinctive route is identified by a unique ‘Osm id’.   </figcaption>
    </figure> </center>


### Processing air pollution variables

In this analysis the time between 1<sup>st</sup> of March 2020 to 31<sup>st</sup> of April 2020 is considered as the time where strict
confinement policies were applied across Europe, thus as the <b>‘lock-down period’</b>.

Following three variables are used to indicate the changes in  NO<sub>2</sub> and CO emissions. Data was preprocessed in Google Earth Engine (GEE) Code editor and further analysis was done with python.

- Average NO<sub>2</sub> and CO emissions during Covid-19 in Europe
- Slope of the time series change of NO<sub>2</sub> and CO emissions during lock-down period
- Percentage change of NO<sub>2</sub> and CO emissions during lock-down period compared to the average values of previous year in the same period.

Two videos below show the weekly average NO<sub>2</sub> and CO emissions from 1<sup>st</sup> of January to 31<sup>st</sup> of July 2020.Areas with no data values are displayed in black colour. Codes used to create the videos can be found in here [<a href="https://code.earthengine.google.com/a968bd2c8a502ccba6a6af3dfc4f0eb6?noload=true"> NO<sub>2</sub></a> , <a href="https://code.earthengine.google.com/c3e02c47cf15255a0f61baa9744fbe94?noload=true"> CO</a>].

<center>
<figure>
    <a href="https://drive.google.com/file/d/1Lp6GMMKtILuKKBBwf0gmqFnctCxwIJ39/view?usp=sharing"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/NO2_weekly_average.gif?raw=true"></a>
    <figcaption>Weekly average NO<sub>2</sub> emissions of Europe from 1<sup>st</sup> of January to 31<sup>st</sup> of July 2020, measured in mol/m<sup>2</sup>.  </figcaption>
    </figure> </center>

<center> <figure>
    <a href="https://drive.google.com/file/d/1D4hfbxcE7bk2suDp2b_2ocJLfKrU6Xkn/view?usp=sharing"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/CO_weekly_average.gif?raw=true"></a>
    <figcaption>Weekly average CO emissions of Europe from 1<sup>st</sup> of January to 31<sup>st</sup> of July 2020, measured in mol/m<sup>2</sup>.  </figcaption>
    </figure> </center>


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.6.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.6.jpg?raw=true"></a>
    <figcaption>Slope of NO<sub>2</sub> emission data during lock-down period. Negative slopes indicate reductions in NO<sub>2</sub> emission volumes and positive slopes indicate
increase in NO<sub>2</sub> emission volumes. </figcaption>
    </figure> </center>


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.7.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.7.jpg?raw=true"></a>
    <figcaption>Slope of CO emission data during lock-down period. Negative slopes indicate reductions in CO emission volumes and positive slopes indicate increase in CO emission volumes. </figcaption>
    </figure> </center>


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.10.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.10.jpg?raw=true"></a>
    <figcaption>Percentage change of average NO<sub>2</sub> emissions during the lock-down period compared to the previous year. Percentages less than zero indicate reductions in NO<sub>2</sub> emission volumes and percentages greater than zero indicate increase in NO<sub>2</sub> emission volumes compared to
the average values of previous year in the same period.</figcaption>
    </figure> </center>


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.11.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.11.jpg?raw=true"></a>
    <figcaption>Percentage change of average CO emissions during the lock-down period compared to the previous year. Percentages less than zero indicate reductions in CO emission volumes and percentages greater than zero indicate increase in CO emission volumes compared to
the average values of previous year in the same period.</figcaption>
    </figure> </center>
    
<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.13.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.13.jpg?raw=true"></a>
    <figcaption>Mean NO<sub>2</sub> and CO emission volumes over the vessel routes in the Mediterranean Sea and the Black Sea during the lock-down period. </figcaption>
    </figure> </center>
    
<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.12.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.12.jpg?raw=true"></a>
    <figcaption>Slope of NO<sub>2</sub> and CO emissions over the vessel routes in the Mediterranean Sea and the Black Sea during the lock-down period. Negative slopes of NO<sub>2</sub> emission in the
coastal areas in Mediterranean Sea indicate reductions in NO<sub>2</sub> emission in these areas.</figcaption>
    </figure> </center>
    
<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.14.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.14.jpg?raw=true"></a>
    <figcaption>Percentage change average of NO<sub>2</sub> and CO emission volumes over the vessel routes in the Mediterranean Sea and the Black Sea during the lock-down period compared to the previous year same time period.</figcaption>
    </figure> </center>
    
### Assessing the relationships


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/T.4.1.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/T.4.1.jpg?raw=true"></a>
    <figcaption>Correlation statistics between emission variables and road density, vessel routes density and population density. Mean CO and NO<sub>2</sub> are measured
in mol/m<sup>2</sup> and road density and vessel density are measured in number of roads/number of vessel routes within 7 km
radius from each geolocation point. Population density is measured as the number of people living in 7 km radius from
each geolocation point.</figcaption>
    </figure> </center>

### Time series analysis


<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.28.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.28.jpg?raw=true"></a>
    <figcaption>NO2 emission time series change in Lisbon-Portugal, Madrid-Spain and Roam-Italy, and RD of these places. NO2 emissions have dropped significantly during lock-down period in all these places. Volumes start to drop from mid March and start to increase again in late May.</figcaption>
    </figure> </center>

<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.30.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.30.jpg?raw=true"></a>
    <figcaption>NO2 emission time series and the smoothened series change in Barcelona-Spain, Venice-Italy and ˙Istanbul-
Turkey, and VD of these places. NO2 emissions have dropped significantly during lock-down period in all these places. Similar to above figure, this drop has also started in mid March but it continues until the end of July with some irregular spikes in between.</figcaption>
    </figure> </center>
    

<center><figure>
    <a href="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.29.jpg?raw=true"><img src="https://github.com/Bashinim/COVID19-EU/blob/main/Cropped%20Images/F.4.29.jpg?raw=true"></a>
    <figcaption>CO emission time series change and the smoothened series in Ilford-United Kingdom, Barcelona-Spain and Frederiksberg-Denmark, and PD of these places. CO emission has increased during the lock-down period in all these places. The emission volumes have started decreasing again from early May.</figcaption>
    </figure> </center>





















