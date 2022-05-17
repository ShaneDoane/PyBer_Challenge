# Ridesharing analysis

## Overview
The purpose of this analysis is to examine differences in fares for Uber rides between different market types: Rural, Suburban, and Urban. This started with two datasets: ride-level data by date_time with fares and city-level data with market type and driver count. The two datasets were merged on the city variable for the following analysis. The time frames were Jan to April 2019.

## Results

Here is a summary table of rides after consolidating into a summary dataframe

<img width="612" alt="image" src="https://user-images.githubusercontent.com/93338132/151098502-b6c8bee4-62d9-4f1a-a293-aae9c9990ef0.png">

Of note: 
* As market density increases, so does total ride count and driver count. This makes sense given the larger populations
* Inverse to this, avg fare per ride and per driver decreases with market density. This could be explained by urban trips being shorter in both milage and duration.

Here is a chart with total fare by market type

<img width="988" alt="image" src="https://user-images.githubusercontent.com/93338132/151098605-3507dbb6-080f-486b-b5b7-6fb6767c730a.png">

The chart helps illustrate two things: 1) as market density increases, so does total fares and 2) there is not any obvious seasonility to total ride fares. (potentially an uptick in warmer months, but would like to see the total year before making that claim)

## Summary and Recommendations

Overall, urban markets have more density in both riders and drivers, providing affordability to riders, but potentially lower earnings for drivers.

I would recommend: 
1) Reduce total number of drivers in urban markets. There are currently more drivers than total rides, evidencing potential 'wasted drivers'
2) Begin tracking fare by time. It's important to know when demand is happening. i.e. are urban rides mostly at night? With this information, we can inform decisions on if these excess urban drivers are necessary. As an example, if there are on average 100 trips between 8 pm and 10 pm, and a driver can make 2 trips per hour, we would need 50 drivers. If demand (riders) begins outstripping supply (drivers), fares would need to shift accordingly.
3) There may be potential to increase driver supply in rural and suburban markets to lower fare prices to induce demand in those markets.
