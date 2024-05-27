# Google Maps Data Scraper

This script demonstrates how to use Python and Playwright to scrape and extract data from Google Maps.

## Features

- **Scraping**: Utilizes Playwright to scrape data from Google Maps.
- **Data Extraction**: Extracts information such as business name, address, website, phone number, reviews count, and reviews average.
- **Output Formats**: Saves scraped data to both ***Excel*** (xlsx) and ***CSV*** formats.
- **Command-Line Interface**: Accepts search queries and total listings to scrape via command-line arguments.
- **Input Flexibility**: Supports reading search queries from either command-line arguments or an input file.

## Installation

1. Install dependencies:

```bash
pip install -r requirements.txt
playwright install chromium
```

## Usage

### Command-Line Arguments

```bash
python3 google_maps_scraper.py -s "search_query" -t total_listings_to_scrape
```

- `-s` or `--search`: Specify the search query.
- `-t` or `--total`: (Optional) Specify the total number of listings to scrape. Default is set to a large number.

### Input File

Alternatively, you can add search queries to an input file named `input.txt`. Each line in the file represents a separate search query.

### Output

The scraped data will be saved in the `output` directory in both Excel (xlsx) and CSV formats. The output files will be named based on the search query.

## Example

```bash
python3 google_maps_scraper.py -s "restaurants near me" -t 50
```

This command will scrape information for 50 listings of restaurants near the specified location.

## Notes

- This script is designed for educational purposes and should be used responsibly and in accordance with Google's terms of service.
- Consider running the script in headless mode (`headless=True`) for production use.
- Adjust the scraping logic and timeouts as needed based on network conditions and website responsiveness.



