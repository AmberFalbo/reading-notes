# 401 Notes-17: Web Scraping
[Back to 401 Index](401-index.md)<br>


[How to Web Scrap with Python in 4 Minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)<br>
**Web Scraping**
Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

### **Important notes about web scraping:**
1. Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
2. Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.

### **Python Code**
*We start by importing the following libraries.*
```
import requests
import urllib.request
import time
from bs4 import BeautifulSoup
```
Next, we set the url to the website and access the site with our requests library.

```
url = 'http://web.mta.info/developers/turnstile.html'
response = requests.get(url)
```

You'll get a successful output message <Response [200]>

Next we need to parse the htmel with BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure.
```
soup = BeautifulSoup(response.text, “html.parser”)
```
We use the method .findAll to locate all of our `<a>` tags.
```
soup.findAll('a')
```
This code gives us every line of code that has an `<a>` tag. The information that we are interested in starts on line 38 as seen below. That is, the very first text file is located in line 38, so we want to grab the rest of the text files located below. (In the Example provided)
<br>
<br>
Next, let’s extract the actual link that we want. Let’s test out the first link.
```
one_a_tag = soup.findAll(‘a’)[38]
link = one_a_tag[‘href’]
```


This code saves the first text file, ` data/nyct/turnstile/turnstile_180922.txt ` to our variable link. The full url to download the data is actually ` http://web.mta.info/developers/data/nyct/turnstile/turnstile_180922.txt ` which I discovered by clicking on the first data file on the website as a test. We can use our urllib.request library to download this file path to our computer. We provide request.urlretrieve with two parameters: file url and the filename. For my files, I named them “turnstile_180922.txt”, “turnstile_180901”, etc.


```
download_url = 'http://web.mta.info/developers/'+ link
urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])
```

## **very cool!**

Last but not least, we should include this line of code so that we can pause our code for a second so that we are not spamming the website with requests. This helps us avoid getting flagged as a spammer.
```
time.sleep(1)
```

## [What is Web Scraping](https://en.wikipedia.org/wiki/Web_scraping)

Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites. Web scraping software may access the World Wide Web directly using the Hypertext Transfer Protocol, or through a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying, in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

Web scraping a web page involves fetching it and extracting from it. Fetching is the downloading of a page (which a browser does when a user views a page). Therefore, web crawling is a main component of web scraping, to fetch pages for later processing. Once fetched, then extraction can take place. The content of a page may be parsed, searched, reformatted, its data copied into a spreadsheet, and so on. Web scrapers typically take something out of a page, to make use of it for another purpose somewhere else. An example would be to find and copy names and telephone numbers, or companies and their URLs, to a list (contact scraping).



## [Build A Python App That Tracks Amazon Prices!](https://www.youtube.com/watch?v=Bg9r_yLk7VY)
*I wanted to code along but the installs weren't working the same with me, not sure the mac way or if they have changed since June 26, 2019 when this was made*







## [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)

Beautiful Soup is a Python library designed for quick turnaround projects like screen-scraping. Three features make it powerful:

1. Beautiful Soup provides a few simple methods and Pythonic idioms for navigating, searching, and modifying a parse tree: a toolkit for dissecting a document and extracting what you need. It doesn't take much code to write an application

2. Beautiful Soup automatically converts incoming documents to Unicode and outgoing documents to UTF-8. You don't have to think about encodings, unless the document doesn't specify an encoding and Beautiful Soup can't detect one. Then you just have to specify the original encoding.

3. Beautiful Soup sits on top of popular Python parsers like lxml and html5lib, allowing you to try out different parsing strategies or trade speed for flexibility.

- Beautiful Soup parses anything you give it, and does the tree traversal stuff for you. You can tell it "Find all the links", or "Find all the links of class externalLink", or "Find all the links whose urls match "foo.com", or "Find the table heading that's got bold text, then give me that text."

- Valuable data that was once locked up in poorly-designed websites is now within your reach. Projects that would have taken hours take only minutes with Beautiful Soup.





[Back to 401 Index](401-index.md)