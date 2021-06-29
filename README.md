Simple webscraper of the moneysavingexpert forum written in Python. Outputs data as CSV format.

This webscraper was designed for a research project and not intended for commerical use. It is therefore quite idiosyncratic and may need further customisation for more general purpose usage.

The scraped data fields per thread post are (in order): rowhref,	rowtitle,	viewcount,	reply,	body, date_created

Uses BeautifulSoup for HTML parsing.

This package is not available via pip. You must download or clone this repository in order to use it.

Requirements

python +3 (developed using python@3.8.5)
Installation

Clone this repository:

git clone https://github.com/richardappell/mse-scraper/.git
Install dependencies via pip:

sudo pip install -r requirements.txt

Scrape all thread posts of a phpBB based forum

Required arguments:
  url: Full URL to forum thread in string format.
  pages: specify number of pages to scrape. Default is one page.
  postdata: specify on/off for whether to pull date of the thread post and body of the post. This is added to reduce scrape time. Defaulr is off
  
  %time for 5 pages of data was 20 seconds when on vs 4.26 seconds for off.

Report any issues to https://github.com/richardappell/mse-scraper//issues

Run tests:

make test
License

MIT - Tomas Aparicio

# mse-scraper


# Objective
The webscraper pulls data from the moneysavingexpertforum. 

#Options
You can specify the target url, number of pages to request data from and whether to pick up the body of the comment and date of original post.
