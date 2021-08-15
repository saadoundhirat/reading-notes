# **Web Scrape with Python:**

- Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites. 

- Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

![](https://blog.apify.com/content/images/max/1132/1-YfeP5WFbn0MwI76kuTM38w.png)

#### Inspecting the Website

- The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data.


- We start by importing the following libraries.

```
import requests
import urllib.request
import time
from bs4 import BeautifulSoup
```

#### parse the html

- by using BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure. If you are interested in learning more about this library

```
soup = BeautifulSoup(response.text, “html.parser”)

## We use the method .findAll to locate all of our <a> tags.

soup.findAll('a')
```

- Web scraping is used for contact scraping, and as a component of applications used for web indexing, web mining and data mining, online price change monitoring and price comparison, product review scraping (to watch the competition), gathering real estate listings, weather data monitoring, website change detection, research, tracking online presence and reputation, web mashup and, web data integration.

- Web pages are built using text-based mark-up languages (HTML and XHTML), and frequently contain a wealth of useful data in text form. However, most web pages are designed for human end-users and not for ease of automated use. As a result, specialized tools and software have been developed to facilitate the scraping of web pages.

- Newer forms of web scraping involve listening to data feeds from web servers. For example, JSON is commonly used as a transport storage mechanism between the client and the web server.

- There are methods that some websites use to prevent web scraping, such as detecting and disallowing bots from crawling (viewing) their pages. In response, there are web scraping systems that rely on using techniques in DOM parsing, computer vision and natural language processing to simulate human browsing to enable gathering web page content for offline parsing.

#### Semantic annotation recognizing

- The pages being scraped may embrace metadata or semantic markups and annotations, which can be used to locate specific data snippets. If the annotations are embedded in the pages, as Microforms does, this technique can be viewed as a special case of DOM parsing. In another case, the annotations, organized into a semantic layer are stored and managed separately from the web pages, so the scrapers can retrieve data schema and instructions from this layer before scraping the pages.
