                                               DAILY PASSENGER JOUNERY

About Dataset:
This dataset contains the daily number of passengers using different public transport services. Each row represents one day, and the columns show how many people used services like local bus routes, light rail, rapid routes, peak-hour buses, school transport, and a few other categories. It’s essentially a time-series dataset that helps us understand how public transport usage changes over time.The data comes from a public transport authority’s open-data portal, where daily ridership numbers are shared for analysis and reporting purposes.

Insights gathered:
1.	I noticed that weekdays always have a big jump in passenger numbers compared to weekends.This really shows that most people use public transport mainly for their regular routines like work and school, not so much for weekend outings.

2.	The School service numbers go up and down exactly with the school calendar.
That made me realize how much student travel actually contributes to the overall system — when schools close, the drop is really noticeable

3.	Light Rail usage stays pretty stable throughout the year.This gave me the impression that it has a steady group of regular users who rely on it regardless of the season
4.	Local Route and Rapid Route services consistently carry the most people.
From this, it seems like these routes are either more convenient .

5.	Light Rail usage stays pretty stable throughout the year.This gave me the impression that it has a steady group of regular users who rely on it regardless of the season.

6.	Whenever there are holidays, the passenger count dips across almost all services.It suggests that public transport demand is strongly tied to people’s daily routines, and once those routines pause, travel slows down to.

Overview of the Forecasting Model:

  For the forecasting part, I went with Holt’s Linear Trend Method because my data mainly showed a steady trend without any strong seasonal patterns. I didn’t want to overcomplicate things with a heavy model, so this felt like a clean and practical choice. It’s commonly used for short-term forecasting, and it matched the behaviour of my dataset really well.

  The idea behind Holt’s method is actually pretty simple. It looks at two things — the current value of the data and the direction in which it’s moving. Using these, the model updates its understanding of the trend and then projects it forward to predict the next few days. I liked this because it keeps the logic very understandable and doesn’t add unnecessary complexity.

  In my case, the ridership numbers were moving gradually, not jumping up and down too much, so this method captured that pattern nicely. It gave me smooth, sensible predictions for the next 7 days, and it didn’t require a lot of tuning or complicated steps. Overall, it felt like the right balance between being simple and still giving useful results.

  So in short, I chose Holt’s model because it was easy to implement, easy to explain, and it fit the nature of my data. It allowed me to get a clear forecast without getting stuck in too many technical details, which was exactly what I needed for this task.

 Conclusion:
 In the end, this project helped me understand how people actually use public transport on a daily basis. Weekdays, work routines, and school schedules clearly shape the demand. After exploring the data, I used Holt’s Linear Trend method to make a simple 7-day forecast, which gives a clear idea of how passenger numbers might change in the coming days. Overall, the analysis gave me a straightforward picture of the system and the travel patterns behind it.
 



