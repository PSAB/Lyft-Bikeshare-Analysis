# Lyft Bikeshare Analysis
## by Pavan Sabnis


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

This dataset was provided by Lyft at https://www.lyft.com/bikes/bay-wheels/system-data. Each entry is a ride by a customer using bicycles that are part of Lyft's bikeshare program. These datasets are made publicly available by Lyft, and it contains the following information: 

Trip Duration (seconds)
Start Time and Date
End Time and Date
Start Station ID
Start Station Name
Start Station Latitude
Start Station Longitude
End Station ID
End Station Name
End Station Latitude
End Station Longitude
Bike ID
User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
Member Year of Birth
Member Gender

I added columns such as route distance (calculated using the latitude and longitude data) and member age (calculated using member year of birth) and a boolean column depicting whether a certain ride was started on a weekday. 
I also dropped certain rows with implausible data such as an extremely high age or trip duration. 




## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

My findings were primarily based on the overall distributions of variables as well as a few multivariate interactions (there is not too much numerical data in this dataset), but key findings include:

Plotted on a logarithmic scale, the distribution of Ride duration takes on a symmetric unimodal shape.
There are greater number of rides during the weekdays (each peak of 5 days) compared to weekends.

The median age of Lyft Bikeshare members is 34, with a minimum of age 18, a median of 32, and a third quartile of 39. There are members that are well into the 50s, however.

There are much higher frequencies of subscribers compared to customers.

With a logarithmic scale applied, the ride distance takes on a relatively symmetric shape. There is a jump of frequencies on 0 miles, because several users choose to dock at the same bike station from where they left their bikes.

Users tend to ride for longer over the weekends compared to weekdays. This pattern seems to be kept relatively steady.

97% of rides were used for commuting purposes.

There are much more male users than female users.

There are much more subscribers than customers.






## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.