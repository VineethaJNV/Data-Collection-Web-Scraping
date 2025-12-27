# Data-Collection-Web-Scraping

Data Collection(From readily available API's and web scraping using Beautiful Soup)

## Secondary Sources of Data Collection

- DataBases - SQL(MySQL, PostgreSQL etc), NoSQL databases (MongoDB etc)
- Public Datasets - Kaggle, UCI ML Repo etc.
- API's - Twitter API, Stock API, Weather API etc.(https://free-apis.github.io/#/)
- Web Scraping - HTML pages, blogs/articles, social media pages etc.

## Primary Sources of data collection

- Sensors & Devices - IoT Devices, Health wearables, etc
- Surveys & Forms - customer satisfaction, feedback, etc.

## Artificial Data

- System Geneated - Logs, Video feeds, Synthetic data etc.(Generated Adversial N/W(GAN) can be use d to generate artificail data )


# There are 3 famous libraries for web Scraping
1. requests - Used to download the web page which is  HTML
2. Beautiful Soup - Parses and extracts data from HTML
3. Selenium - Automate browser to load dynamic  JS  pages


# Basic Get request
GET request iss used to retrieve a webpage or API response
* we can scrpe the data from https://toscrape.com/ => Scraping Sandbox
* And from https://www.scrapethissite.com/pages/ =>These 2 websites allow to scrape their data



# Headers
Websites often expect certain characters like "User-Agent" that lets them know that the requets is coming from a real browser.
This can help us avoid getting blocked when sending automated requests
headers={
    "user-agent":"Mozilla/5.0"
}
res = requests.get(url, headers=headers)

time.sleep() can be used to introduce delays in web scraping script
to avoid hitters too fast.



# Beautiful Soup 
- is a Python library used to parse HTML  and XML documents.
- Helps in extracting the data from web pages after downloading them with requests

# Beautiful Soup Methods
- find() => Finds the first matching element
- findall() => Finds all the elements
- find_parent()
- find_next()
- find_previous()


# Navigating DOM elements with Beaautiful Soup
- parent
- chidren
- descendents()
- next_siblings()
- previous_siblings()