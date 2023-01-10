# Tableau-Project

# bikesharing
### Overview 
The purpose of this analysis was to visualize data regarding a bike sharing company and to convice investors that opening another location would be a wise decison. In order to do that
we needed to display how frequent people utilize the current bike sharing services. With the Visualizations created we can effectively show investors what they need to know in order to decide whether or not they want to invest into the company. The visualizations that we created show when people are most active and how long their trips are. The visualizatios also show the differences in activiy between genders. This gives the investors as well as the business great insight so they can plan and act accordingly. Potentially this could mean knowing when to deploy maintainence operations or knowing what audiences they need to market their services to more. The information we can extract from the visualizations is beneficial to both parties in this case.

### Results
The first result was to show how long bikes are checked out for. We did this by creating a line chart with "Hour(TripDuration)" and "Minute(TripDuration)" in our columns section and 
"CNT-citibike-tripdata.csv" in our rows section. We added "Hour(TripDuration)" to the filters section so we are able to filter to see how long users used the equipment. 5 minute trips seems to be the sweet spot for trip durations.
[link to first chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimes/CheckoutTimesforUsers?publish=yes)

The second result was to show how long trip durations were based on gender. We did this by dragging the bike count to the "Rows" section, trip duration information to the "Columns" section, "Hours" and "Genders" to the "filters" section and "Genders" info in the "Color" section of our "Marks" Section. The most frequent time duration for males was 5 minutes and the most frequent duration for females was also 5 minutes but the females had a significantly smaller sample size.
[link to second chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimesbygender/CheckoutTimesbyGender)

The third and fourth result showed us which days people were most active on based on gender. Here I had to perform a calculation in the "Calculated Fields" section. I took calculated "Gender" as "Number to string" from dimension and converted the numbers per gender to a string. The formula I used was 
(if [Gender]= '0' then 'UNKNOWN'
ELSEIF [Gender] = '1' then 'MALE'
ELSEIF [Gender] = '2' then 'FEMALE' END). After this calculation we needed to were able to get results based on gender. I added "WEEKDAY(StopTime)" to the Columns section and "WEEKDAY(Starttime)" to the rows section. Finally, I added "Number to string" to the filters section.
From the visualization we can see that people are most active on weekday mornings from 8am to 9am and weekday afternoon to evening from 5pm to 6pm. This makes sense considering biking may be an efficient way to navtigate the Downtown environment while traffic is at its peak.
[link to third and fourth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/tripsbyweekdayhrgender/TripsbyweekdayhrGender)

The fifth result showed us the amount of bike trips taken by gender for each day of the week by each Usertype. One discovery I made was that Customers that didn't identify with a gender were most active on Saturdays while subscribers were most likely to be men who were active on Thursdays. 
[link to fifth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/userTripsbygenderbyweekday/UserTripsbyGenderbyweekday)

The sixth result showed us how much each bike had been used and which ones were most likley to need maintenance.
This helps us be proactive in preventing people from using bikes that are not prepared for usage. This also has the potential to prevent injuries and other things that can hurt the brand. 
[link to fifth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/bikesneedingrepair/Maintenance)

The seventh result was used to show the most popular start locations predicated on gender. We used size to make the visualization easier to read. 
Since we have this information we can make our services more appealing to each gender by having bikes available at the location where they are most likely to start riding. 
![187202D1-8D7E-4A5F-8364-61D01D080AD5](https://user-images.githubusercontent.com/112785655/209229644-8e1d510e-e873-4b04-95cc-d1804f99de30.jpeg)

### Summary
We can conclude that people were most likely to ride the bikes for around 5 minutes. Secondly we can conclude that men and women ride bikes for similar amounnts of time when they use the service. Third and fourthly we can conclude that both gender are most active around 8am and 6pm on thursdays. We can also conclude that the buisness gets most of its transactions from male Subscribers. My first recomendation would be to add a chart that tells us which bikes were used the most for maintenance purposes. My secoond recommendation was to add a chart that would highlight starting locations based on gender for making units more accesssible to all genders. 

[link to dashboard](https://public.tableau.com/app/profile/brenton.ervin/viz/Dashboard1_16717560803090/Dashboard1)

[link to first chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimes/CheckoutTimesforUsers?publish=yes)

[link to second chart](https://public.tableau.com/app/profile/brenton.ervin/viz/checktimesbygender/CheckoutTimesbyGender)

[link to third chart](https://public.tableau.com/app/profile/brenton.ervin/viz/tripsbyweekdayhrgender/TripsbyweekdayhrGender)

[link to fourth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/userTripsbygenderbyweekday/UserTripsbyGenderbyweekday)

[link to fifth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/bikesneedingrepair/Maintenance)

[link to sixth chart](https://public.tableau.com/app/profile/brenton.ervin/viz/Startlocationsbygender/Startlocationsbygender)
