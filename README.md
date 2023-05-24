## Description
This project focuses on full web-scraping and data analysis. To web srcape, I identified HTML elements on a page,  identified their id and class attributes, and used these attributes to extract information via both automated browsing and HTML parsing. The project is divided into two parts. In the first part, I web scraped titles and preview text from Mars news articles on a webpage while in the second part, I scraped and analyze Mars weather data, which exists in a table.

## Library
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

## Summary of Dataset

## Project Steps
### Step 1: Merging both data sets 
The first step was to use the automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html). Inspect the page to identify which elements to scrape. To identify which elements to scrape, inspect the page by using Chrome DevTools.
I also added a python time sleep function to cause a one second delay in the execution of the program

### Step 2: Summary Statistics 

### Step 2: Visualizations
-
## Summary of Results
- On average, the third month has the coldest minimum temperature on Mars, and the eighth month is the warmest. But it is always very cold there in human terms!
- Atmospheric pressure is, on average, lowest in the sixth month and highest in the ninth.
- The distance from peak to peak is roughly 1425-750, or 675 days. A year on Mars appears to be about 675 days from the plot. Internet search confirms that a Mars year is equivalent to 687 earth days.

## References
<a href ="https://static.bc-edx.com/data/web/mars_news/index.html"The Mars News website</a> is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from <a href ="https://mars.nasa.gov/">NASA's Mars News</a> website in November 2022. Images are used according to the <a href ="https://www.jpl.nasa.gov/jpl-image-use-policy">JPL Image Use Policy</a>, courtesy NASA/JPL-Caltech.
