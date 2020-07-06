# Ford Gobike Trip Data Exploration
## by Satvinder Kaur

## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

This dataset contains information about Ford Gobike trips from 2017. Ford Gobike is now known as Bay wheels which is a regional public bicycle sharing system in San Francisco Bay Area, California. This dataset contains around 500,000+ trip records. It can be downloaded from [Here](https://s3.amazonaws.com/baywheels-data/2017-fordgobike-tripdata.csv.zip) with the feature information available [Here](https://www.lyft.com/bikes/bay-wheels/system-data).

There are 519,700 rows each representing an individual bike trip with 13 features as follows:

- duration_sec
- start_time
- end_time
- start_station_id
- start_station_name
- start_station_latitude
- start_station_longitude
- end_station_id
- end_station_name
- end_station_latitude
- end_station_longitude
- bike_id
- user_type

For this project, I extracted the start month, start day and start hour of every trip from start_time feature.
Then, to save these extracted values I added columns month, day and hour in given dataset.
Finally, I assigned ordered categorical datatype to these columns.

## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

In the exploration of the this dataset, I found followings insights:

- The average trip duration is around 10 minutes, and most of the trip durations were between 5 minutes to 20 minutes.
- Most of the users are Subscribers. It indicates that people who use bike service on regular basic are more likely to subscribe for the service.
- The number of trips taken over the period of month has increased from June to October with slight decrease in November and December. This could be due to the holidays in these two months.
- Most of the trips are taken on weekdays compared to weekends. As most of the users are subscribers, it seems like they use the bike service of work commute on weekdays.
- The distribution of number of trip taken during a day shows that the most number of trips are taken at 8 am in the morning and another one at 5 pm in the evening. This gives even more evidence that the most users use this bike service for daily work commute for general business hours 9am to 5pm.
- Trip duration for subscribers is smaller than the customers.
- The features month or time of a day when trip started does not affect the distribution of trip durations.
- The start time of a trip slightly affect the trip durations, trip durations for 11am to 5pm are slightly longer than other day time hours which is quite as expected because people generally take more and longer bike trips in day time.
- Subscribers take more trips on weekdays compare to weekends and customers take more trips on weekends compare to weekdays. This could be due to subscribers using bike service as daily means of commute to work on weekdays and customers are the one time users who might be the visitors to the Bay area using bike services on weekends for one time.
- Subscribers take more trips during morning 7am to 9am and during evening 4pm to 6pm, while customers take most of the trips from 10am to 6pm.
- The distribution for the weekend Gobike trips is has a peak at 1pm, and most of the trips were taken in the middle of the day from 10am to 6pm.
- Also, most late night trips i.e after 11pm till 3am early morning are taken on weekends.
- The proportion of trips starting and ending on most of the stations are equal.
- The average trip duration for customers is greater than average trip duration of subscribers.

## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.

For the presentation, I have focused on my feature of interest "trip Duration".
First of all, I have introduced the distribution of trip durations over the given dataset to observe the average trip duration. Then I have introduced the distribution of different user type, to determine the most regular user types for the Gobike service. Then I have explained the effect of other features like user type and start day of trip on trip duration.

I have also included the trends of Gobike trips taken on weekdays vs weekends to see the effect of start day and start time of trip on number of trips.
Finally, I have also explained the patterns of hourly usage of Gobike services during a week for subscribers and customers.  

## Presentation Slides

Access the slides by using nbconvert to export the notebook and set up a server for the slides.
From the terminal or command line, run the following expression:

 > `jupyter nbconvert slide_deck.ipynb --to slides --post serve --template output_toggle.tpl`

This will open a tab in your web browser where you can scroll through your
presentation. Sub-slides can be accessed by pressing 'down' when viewing its parent
slide.

### Resources:

- https://seaborn.pydata.org/tutorial/categorical.html
- https://knowledge.udacity.com/questions/159800
