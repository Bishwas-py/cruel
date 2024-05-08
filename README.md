`Cruel` is a Python web-request library that allows you to extract detailed information from any webpage or site.

## Features

- Inbuilt beautiful soup instance
- ScraperAPI powered; so you don't have to worry about IP blocking

## Installation

You can install the `cruel` using pip:

```bash
pip install cruel
```

## Usage

Below are examples of how to use the `cruel` to extract data from Fiverr gig pages and user profiles.

### Scrape Example

```python
from cruel import session

session.set_scraper_api_key("XYZ-SCRAPER_API_KEY")
response = session.get("https://www.fiverr.com/username/your-gig-slug")  # your fiverr url should be here
print(response.soup)  # gives you beautiful soup instance
# You can use `response.soup` to further extract your information. 
```

> Get your ScraperAPI key [here](https://www.scraperapi.com/?fp_ref=enable-fiverr-api).

## Project Structure

The `cruel` is organized into several modules to enhance code readability and maintainability:

- `cruel`
    - `__init__.py`: For exporting `session`
- `cruel.utils`
    - `req.py`: Extending requests for Fiverr scraping
    - `scrape_utils.py`: Utilities for scraping

## License

[GPL](https://choosealicense.com/licenses/gpl-3.0/)

## Contributing

New [pull requests](https://github.com/Bishwas-py/cruel) are welcome.
For major changes, please open an issue first to discuss what you would like to change.

## Author

Check more of [my projects](https://bishwas.net/projects).