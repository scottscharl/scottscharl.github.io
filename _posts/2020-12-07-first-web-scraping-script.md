---
title: Web Scraping in Python
---
I built a Python script that opens a web browser to YouTube and searches my name.

You could use code like this to automatically search Craigslist/eBay/etc. and notify you when someone puts up a rare item for sale.

Many thanks to [Hitesh Choudhary](https://www.linkedin.com/in/hiteshchoudhary/?originalSubdomain=in) for [this excellent tutorial](https://www.youtube.com/watch?v=f7LEWxX4AVI).

Note: When inspecting the YouTube page to copy the XPath, I could only get the script to work using the "full XPath" option (Hitesh says in the tutorial that you don't have to use the "full").

Here's the code:
```
# I installed the Selenium web browser, which allows a browser to be opened and run via the command line.
from selenium import webdriver

# We need to import the time module
import time

driver = webdriver.Chrome()

#This tells the browser to naviage to YouTube:
driver.get('https://youtube.com')

#The script waits 2 seconds to let the page load:
time.sleep(2)

# The script finds ths YouTube search box and types in the search parameters:
searchbox = driver.find_element_by_xpath('/html/body/ytd-app/div/div/ytd-masthead/div[3]/div[2]/ytd-searchbox/form/div/div[1]/input')
searchbox.send_keys('Scott Scharl')

# Finally, the script finds and clicks the search button.
searchButton = driver.find_element_by_xpath('/html/body/ytd-app/div/div/ytd-masthead/div[3]/div[2]/ytd-searchbox/form/button')
searchButton.click()

#done! I have automated a YouTube search for my name.
```
