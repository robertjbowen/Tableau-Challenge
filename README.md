# Tableau-Challenge

### Link: https://public.tableau.com/views/CitiBike-Challenge_16132624654020/BikeStationUsage?:language=en&:display_count=y&publish=yes&:origin=viz_share_link

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture1.png"/>
    <br>
    <em>CitiBike Tableau Dashboard</em>
</p>

***

The purpose of this challenge is to use Tableau to create visualizations of data from the New York City CitiBike website to discovery and display phenominon related to the CitiBike program. The Data visualizations are then combined to create an interactive dashboard from which stories can be developed to highlight the discovered information. Much of the data set were large with millions of lines of data for each month, representing the individual trip data of actual ridership.

The data is not clean and what has been collected has changed over the years so it was necessary to identify a subset of the data to use for this challenge. I chose to use data from the year 2020 as it posed the added benefit to see how the pandemic might have impacted ridership across NewYork City.

I used Pandas in Jupyter Lab to read, clean, and aggregate the data, and used the Google Places API to gather the zip code data which I appended to the joined data aggregate dataframes. For the map I grouped each monthly data set based on the start location name and then grouped the reduced monthly data sets into an annual dataset effectively reducing over 17 Million lines of code to about 12,000 which was significantly easier for Tableau to manage.

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture7.png"/>
    <br>
    <em>Monthly Grouped Data with zip code and formatted date columns generated with Pandas</em>
</p>

The Map displays each CitiBike Station as a circle, the size of the Circle represents the total number of trip originating from there that month and the color of the circle represents the total combined trip durations for all trips originating from that station. The zip codes are overlayed as a seperate marks layer that can be toggled on and off as required. By stepping through each month a steady increase in new CitiBike Stations can be seen being added to the North throughout the course of the year and popular stations become evedent as the cirles grow and turn green as ridership increases in the summer months and remain steady. A significant dip in ridership in April and May is apparent which coincides with the initial spread of the Pandemic and subsequent lock down of the city.

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture3.png"/>
    <br>
    <em>Northerly growth in CitiBike Stations</em>
</p>

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture5.png"/>
    <br>
    <em>Popular Stations are Near Ports and Parks</em>
</p>

***

Analysis of trip duration, bike id and start and end station data for the month of July revealed individual bikes can have significatantly different use rates and also showed hourly rider trends. It is also possible to spot if a CitiBike might have been stolen.

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture2.png"/>
    <br>
    <em>Bike Usage Dashboard</em>
</p>

<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture4.png"/>
    <br>
    <em>Daily Trip Counts vs. Average Trip Durations</em>
</p>
  
<p>
    <img src="https://github.com/robertjbowen/Tableau-Challenge/blob/main/images/Picture6.png"/>
    <br>
    <em>Individual CitiBike Usage</em>
</p>


***