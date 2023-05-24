## Description
This project focuses on full web-scraping and data analysis. To web srcape, I identified HTML elements on a page,  identified their id and class attributes, and used these attributes to extract information via both automated browsing and HTML parsing. The project is divided into two parts. In the first part, I web scraped titles and preview text from Mars news articles on a webpage while in the second part, I scraped and analyze Mars weather data, which exists in a table.

## Library
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

## Dataset
The news article titles, summaries, dates, and images were scraped from <a href ="https://mars.nasa.gov/">NASA's Mars News</a> website in November 2022. See references for more details.

## Project Steps
### Part 1: Scrape Titles and Preview Text from Mars News
The first step was to use the automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html) and then inspect the page to identify which elements to scrape. I inspected the page using Chrome DevTools. Subsequently, I created a **Beautiful Soup** object and used it to extract the text elements from the website. I also added a python time sleep function to cause a two second delay in the execution of the program to effectively deal with issues that may arise when the webpage is not loading with the speed the computer is attempting to process it with. Finally, I then extracted the titles and preview text of the news articles that I scraped and stored the scraped results in a Python data structure as follows:

    {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
     'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}

### Part 2: ## Scrape and Analyze Mars Weather Data
In this part of the project, I scraped and analyzed Mars weather data. To begin, I used the automated browsing to visit the <a href="https://static.bc-edx.com/data/web/mars_facts/temperature.html">Mars Temperature Data Site</a>, inspected the page to identify the HTML table and then assembled the scraped data into a pandas dataframe. An explanation of the column headings is provided below:

> id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

### Step 2: Visualizations
-
## Summary of Results
- On average, the third month has the coldest minimum temperature on Mars, and the eighth month is the warmest. But it is always very cold there in human terms!
- Atmospheric pressure is, on average, lowest in the sixth month and highest in the ninth.
- The distance from peak to peak is roughly 1425-750, or 675 days. A year on Mars appears to be about 675 days from the plot. Internet search confirms that a Mars year is equivalent to 687 earth days.

## References
<a href ="https://static.bc-edx.com/data/web/mars_news/index.html">The Mars News website</a> is operated by edX Boot Camps LLC for educational purposes only. Images are used according to the <a href ="https://www.jpl.nasa.gov/jpl-image-use-policy">JPL Image Use Policy</a>, courtesy NASA/JPL-Caltech.
