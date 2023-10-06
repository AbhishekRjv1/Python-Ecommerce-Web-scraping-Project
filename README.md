# Python-Ecommerce-Web-scraping-Project

## Web Scraping and Data Conversion Script

This Python script is designed for web scraping product data from specified URLs and converting the scraped data into a CSV file. The script uses the `requests` library for making HTTP requests, `BeautifulSoup` from `bs4` for parsing HTML content, and `pandas` for handling and converting data.

## Prerequisites
- Python 3.x
- Libraries: `requests`, `BeautifulSoup`, `pandas`

## How to Use

### 1. Setup

Make sure you have Python installed on your system. If not, you can download and install it from [python.org](https://www.python.org/).

Install the required libraries using pip:

```bash
pip install requests beautifulsoup4 pandas
```

### 2. Input

Create a text file named `link.txt` containing the URLs you want to scrape, each URL on a new line. Place this file in the same directory as the script.

### 3. Run the Script

Execute the script using the following command:

```bash
python script_name.py
```

Replace `script_name.py` with the actual name of your Python script.

### 4. Output

The script will scrape data from the provided URLs and create a CSV file named `scrapped_data.csv` containing the scraped information.

## Code Explanation

- `get_link(link)`: Function to scrape data from a given URL and return the scraped information as a dictionary.

- `convert_df_to_csv(df, path_directory)`: Function to convert a DataFrame to a CSV file. Takes a DataFrame and the path where the CSV file should be saved as input.

- `main()`: The main function where the URLs are read from `link.txt`, scraped, and converted into a CSV file. Adjust the path and file names as per your requirements.

Please note: Be respectful of the websites you are scraping. Check their `robots.txt` file to ensure you are allowed to scrape their content. Additionally, consider adding a delay between requests (in this script, there is a 5-second delay) to avoid overloading the server with too many requests in a short period.
