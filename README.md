# Airline On-Time Performance
## by Lyn Ndunge Nzioka


## Dataset

The dataset used for this analysis is the Airline On-Time Performance dataset which contains flight arrival and departure details for all commercial flights within the United States between 2007 and 2008. The dataset was obtained from a publicly available source. 

The **data wrangling** steps performed on the original dataset include:
1. Load the 2007 and 2008 airline on-time performance datasets using the Pandas library's read_csv function, specifying the number of rows to read as 100,000 for each dataset.
2. Concatenate the two datasets using the Pandas library's concat function, passing in the two dataframes and setting ignore_index parameter to True.
3. Drop unnecessary columns using the Pandas library's drop function, passing in the names of the columns to be dropped and setting axis parameter to 1 to indicate that we want to drop columns (as opposed to rows).
4. Drop rows with missing values using the Pandas library's dropna function, setting axis parameter to 0 to indicate that we want to drop rows (as opposed to columns).
5. Convert relevant columns to datetime and integer types using the Pandas library's to_datetime and astype functions, respectively.
6. Filter out flights with negative elapsed time using the Pandas library's boolean indexing feature.
7. Create a new column for flight delay by subtracting the CRSArrTime column from the ArrTime column and converting the resulting timedelta object to an integer representing the number of minutes of delay.
8. Filter out flights with negative or extreme delay times using the Pandas library's boolean indexing feature.
9. Create new columns for flight hour, flight season, and flight distance category using the Pandas library's apply function and lambda functions to apply custom logic to existing columns.
10. Save the cleaned dataset to a new file called cleaned_data.csv using the Pandas library's to_csv function.



## Summary of Findings

The main findings of the data exploration are that the flight delay time is heavily right-skewed, with most flights experiencing little to no delay time, but some flights experiencing extreme delay times. Flight delay time is also highly correlated with departure time and day of the week, with delays being more likely to occur later in the day and on certain days of the week. Additionally, the distance of the flight and the airline operating the flight are also associated with the delay time. The steps taken during the data exploration involved dropping unnecessary columns, dropping rows with missing values, converting relevant columns to datetime and integer types, filtering out flights with negative elapsed time, creating a new column for flight delay, filtering out flights with negative or extreme delay times, creating new columns for flight hour, flight season, and flight distance category, and saving the cleaned dataset to a new file called cleaned_data.csv. Overall, the data exploration helped to identify important relationships and patterns in the dataset that will be useful for further analysis and modeling. The airline on-time performance dataset contains information about flight delays, cancellations, and on-time performance of different airlines operating in the United States. To analyze the dataset, we categorized it into different variables such as flight delays in minutes, arrival delays by airline, cancellation distribution, commonly flown routes, reasons for flight cancellations, on-time performance by airline, and average arrival delays by distance and airline.


## Key Insights for Presentation

The overall goal of this presentation is to provide insights into the factors that contribute to flight delays and to identify the airlines that perform best based on the distance and day of the week. The presentation will also explore how the relationship between departure delay and arrival delay varies with distance and day of the week, and how the arrival delay differs across different airlines and months.

**Key Features:**

**Analyze flight delays and cancellations:** Explore the frequency, duration, and reasons for flight delays and cancellations.
**Evaluate airline performance:** Investigate the on-time arrival and departure rates, average delay times, and other metrics to identify the airlines that perform the best.
**Examine time and seasonality factors:** Study the effects of,day of the week, month, and season on flight delays and cancellations.
**Assess distance and routes:** Analyze the relationship between distance of travel and flight performance, as well as the performance of different flight routes.

**Key insights** 
What is the distribution of flight delays in minutes?
How do arrival delays vary by airline?
Is there a difference in arrival delays between weekday and weekend flights?
What are the most commonly flown routes?
What is the distribution of cancelled flights in the dataset ?
What are the most common reasons for flight cancellations?
How do different airlines compare in terms of on-time arrivals and departures?
What is the distribution of flight cancelled by the day of the week?
How does the average arrival delay vary by day of week?
How does the distance of a flight affect its arrival delay?
How does departure delay impact arrival delay for different airlines?
How does distance affect the relationship between departure delay and arrival delay?
Is there a correlation between the departure delay time and the arrival delay time, and does this relationship differ depending on the airline or day of the week?
How does the average arrival delay vary by distance and airline?
How does the relationship between DepDelay and ArrDelay vary with distance and day of week?
How does the arrival delay vary across different airlines and months, and is there a significant difference between them?

    
The findings of this analysis can be used to help airlines and airports identify areas for improvement and to make data-driven decisions to reduce flight delays.




# Airline-On-time-Performance
