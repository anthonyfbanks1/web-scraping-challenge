# Mars News and Weather Analysis
Scraping Mars news &amp; weather data using Splinter and Beautiful Soup for statistical analysis using Python Pandas and Matplotlib
- - -
![Curiosity_selfie](Images/curiosity.png)

Image Credit: NASA/JPL-Caltech/MSSS
- - -
## Project Structure  
### Code Files:  
All project code can be found in the [Deliverables](Deliverables/) folder.  
**Part 1 Mars News:** [mars_news.ipynb](Deliverables/mars_news.ipynb)  
**Part 2 Mars Weather:** [mars_weather.ipynb](Deliverables/mars_weather.ipynb)  

### Output:  
Scraped news articles & weather data can be found in the [Output](Output/) folder.  
**Mars News:** [mars_news_articles.json](Output/mars_news_articles.json)  
**Mars Weather:** [mars_weather_data.csv](Output/mars_weather_data.csv)  

### Images:  
Graphs generated from weather analysis can be found in the [Images](Images/) folder.  
**Average Temperature:** [ave_temp.png](Images/ave_temp.png)  
**Average Pressure:** [ave_pssr.png](Images/ave_pssr.png)  
**Daily Temperatures:** [daily_temps.png](Images/daily_temps.png)  

- - -
## Background
This assignment consists of two technical products. You will submit the following deliverables:

### Deliverable 1:
A Jupyter notebook containing code that scrapes the Mars news titles and preview text and prints/stores them in the following format:

```
{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
 ```
 
### Deliverable 2:
A Jupyter notebook containing code that scrapes the Mars weather data and that cleans, visualizes, and analyzes that data.

Analyze your dataset by using Pandas functions to answer the following questions:

1. How many months exist on Mars?
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    - Find the average minimum daily temperature for all of the months.
    - Plot the results as a bar chart.
4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    - Find the average daily atmospheric pressure of all the months.
    - Plot the results as a bar chart.
5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.

- - - 

## Deliverable 2 Analysis Results:

**Question 1:**  
In our dataset, the Martian year is broken up into 12 months, which are much longer than Earth months.  There are 22.57 Earth months (or 687 days) in a Martian year.  

**Question 2:**  
There are 1,977 Martian days worth of measurements in the dataset.  

**Question 3:**  
![Average_Temp](Images/ave_temp.png)  


On average, the third Martian month is the coldest, and the eighth month is the warmest, but the temperatures are always extremely cold in comparison to the temperatures we are used to on Earth!  

**Question 4:**  
![Average_Pressure](Images/ave_pssr.png) 


The average atmospheric pressure on Mars is lowest in the sixth month and highest in the ninth.  

**Question 5:**  
![Daily_Temps](Images/daily_temps.png)  


The distance from peak to peak is roughly 1480 - 795, or 685 sols.  A sol is very close to the same length as an Earth day, so we would expect this to be good for a rough estimate. A year on Mars appears to be about 685 days from the plot. Our notebook calculations above confirm that a Mars year is equivalent to 687 Earth days.  

- - - 
### References
The [Mars News website](https://static.bc-edx.com/data/web/mars_news/index.html) is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from [NASA's Mars News](https://mars.nasa.gov/) website in November 2022. Images are used according to the [JPL Image Use Policy](https://www.jpl.nasa.gov/jpl-image-use-policy), courtesy NASA/JPL-Caltech.
