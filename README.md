# Whiskey-Spider
"Web Scraping Whiskey Shop with Scrapy"

This Git repository contains a Scrapy spider script that scrapes data from the Whisky Shop website. The spider, named "WhiskeySpider," starts by visiting the main URL of the Scotch whisky section, filtering for in-stock items.

The `parse` method extracts information about each whiskey item, including its name, price, and product link. It uses CSS selectors to target specific elements on the page and yields a dictionary with the extracted data. If an item is sold out, it assigns the value "sold-out" to the price field.

The script also looks for a link to the next page and follows it if available, calling the `parse` method recursively to scrape data from subsequent pages.

This project demonstrates how to use Scrapy to scrape data from the Whisky Shop website. It showcases the utilization of CSS selectors to extract desired information and the handling of pagination to scrape multiple pages of data.

The scraped data can be used for various purposes, such as analyzing whiskey prices, monitoring product availability, or building a whiskey catalog.
