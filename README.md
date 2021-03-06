# BookingCom-Reviews-Crawler

This is a project with Scrapy and Selenium combined in order to crawl booking.com site for hotels and their reviews of a pre-specified city. 

## Prerequisites

1- you need to download and add Geckodriver + Chromedriver (the drivers for firefox & chrome browsers) to your system's path.

2- make sure Firefox/Chrome is installed and compatible with the driver's version.

## Usage Instructions

1- first of all, make a new python virtual environment: ``` virtualenv <env_name> ```

2- navigate to the virtual env: ``` cd <env_name> ``` 

3- activate it:  ``` source bin/activate ```

4- clone the repository there: ``` git clone https://github.com/Raki22/BookingCom-Reviews-Crawler ```

5- run:  ``` pip install -r requirements.txt ```

6- navigate to ReviewsScraper folder: ``` cd ReviewsScraper ```

7- open the local terminal and run: ``` scrapy crawl hotels -a city="<name_of_the_city>" -a browser="firefox" -s filename="<file_name>.csv" --loglevel=ERROR ```

***Note: you can change browser argument value to "chrome", but still firefox is highly recommended.

## Expected Output: 

1- the named-by-you file will contain hotels information that exist in the named city and booking.com site.

2- plus, a reviews file for each hotel (automatically named, the name is extracted from the hotel link).
