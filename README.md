## Amazon Web Scraper

This is a Python project that scrapes the title and price of a specific product on Amazon India and saves it to a CSV file. The program uses the Beautiful Soup library for web scraping, requests for sending HTTP requests, and Pandas for data analysis.

### Requirements
- Python 3.x
- Beautiful Soup 4
- Pandas
- Requests

### Automation
To automate the process of checking the price of the product, you can use a while loop that runs the `check_price()` function every 24 hours using the time library. The `check_price()` function essentially repeats the same process of extracting and appending the data to the CSV file, but this time it runs in a loop, allowing the program to continuously monitor the price of the product over time.

### Customization
You can customize the program to extract data for any product on Amazon India by changing the URL of the product. You can also modify the program to extract data for multiple products at once by using a loop to iterate over a list of URLs.

### Future Improvements
The program can be further improved by adding features such as email alerts when the price of a product falls below a certain threshold or using machine learning to predict the future prices of a product based on historical data.

### Installation
pip install beautifulsoup4 pandas requests

### Usage
1. Edit the `product_url` variable in `amazon_scraper.py` to the URL of the product you want to scrape.
2. Run `amazon_scraper.py`
3. The program will create a CSV file in the same directory as `amazon_scraper.py` with the name `product_data.csv`. The file will contain the title, price, and date of the scraped data.

