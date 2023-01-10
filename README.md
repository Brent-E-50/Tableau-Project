# Tableau-Project

# bikesharing
### Overview 
The purpose of this analysis was to visualize data regarding a bike sharing company and to convice investors that opening another location would be a wise decison. In order to do that
I needed to display how frequent people utilize the current bike sharing services. With the Visualizations created I can effectively show investors what they need to know in order to decide whether or not they want to invest into the company. The visualizations that I created show when people are most active and how long their trips are. The visualizatios also show the differences in activiy between genders. This gives the investors as well as the business great insight so they can plan and act accordingly. Potentially this could mean knowing when to deploy maintainence operations or knowing what audiences they need to market their services to more. The information I can extract from the visualizations is beneficial to both parties in this case.

### Results
The first result was to show how long bikes are checked out for. I did this by creating a line chart with "Hour(TripDuration)" and "Minute(TripDuration)" in our columns section and 
"CNT-citibike-tripdata.csv" in our rows section. I added "Hour(TripDuration)" to the filters section so I are able to filter to see how long users used the equipment. 5 minute trips seems to be the sweet spot for trip durations.
[link to first chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimes/CheckoutTimesforUsers?publish=yes)

The second result was to show how long trip durations were based on gender. I did this by dragging the bike count to the "Rows" section, trip duration information to the "Columns" section, "Hours" and "Genders" to the "filters" section and "Genders" info in the "Color" section of our "Marks" Section. The most frequent time duration for males was 5 minutes and the most frequent duration for females was also 5 minutes but the females had a significantly smaller sample size.
[link to second chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimesbygender/CheckoutTimesbyGender)

The third and fourth result showed us which days people were most active on based on gender. Here I had to perform a calculation in the "Calculated Fields" section. I took calculated "Gender" as "Number to string" from dimension and converted the numbers per gender to a string. The formula I used was 
(if [Gender]= '0' then 'UNKNOWN'
ELSEIF [Gender] = '1' then 'MALE'
ELSEIF [Gender] = '2' then 'FEMALE' END). After this calculation I needed to were able to get results based on gender. I added "WEEKDAY(StopTime)" to the Columns section and "WEEKDAY(Starttime)" to the rows section. Finally, I added "Number to string" to the filters section.
From the visualization I can see that people are most active on weekday mornings from 8am to 9am and weekday afternoon to evening from 5pm to 6pm. This makes sense considering biking may be an efficient way to navtigate the Downtown environment while traffic is at its peak.
[link to third and fourth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/tripsbyweekdayhrgender/TripsbyweekdayhrGender)

The fifth result showed us the amount of bike trips taken by gender for each day of the week by each Usertype. One discovery I made was that Customers that didn't identify with a gender were most active on Saturdays while subscribers were most likely to be men who were active on Thursdays. I was able to create this visua;ization by adding "GC" or "Number to string" to the columns section. I added "Usertype" and "WEEKDAY(Starttime)" to the rows section. In addition I added Usertype" and "GC" to the filters section. And Finally I was able to drag "CNT-citibike-tripdata.csv" to the "Color" Section. 
[link to fifth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/userTripsbygenderbyweekday/UserTripsbyGenderbyweekday)

Below is a dashboard that consists of all 5 visualizations

[link to dashboard](https://public.tableau.com/app/profile/brenton.ervin/viz/Dashboard1_16717560803090/Dashboard1)
