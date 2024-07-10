# Wikipedia Web Scraping Project

This project focuses on scraping information from Wikipedia using Python libraries.

## Steps Taken

### Data Collection
- **Objective**: Scrape data from the Wikipedia page listing the largest manufacturing companies by revenue.
- **URL**: [List of largest manufacturing companies by revenue](https://en.wikipedia.org/wiki/List_of_largest_manufacturing_companies_by_revenue)
- **Libraries Used**: Used `requests` for fetching web pages and `BeautifulSoup` for parsing HTML content.

### Data Preprocessing
- **Fetching HTML Content**: Retrieved the HTML content of the target Wikipedia page using `requests`.
- **Parsing HTML**: Parsed the HTML content using `BeautifulSoup` to navigate and extract the required data.
- **Extracting Information**: 
  - Identified and extracted the relevant table containing the list of companies.
  - Extracted column names and row data from the table.

### Data Storage
- **Structured Data**: Organized the extracted data into a pandas DataFrame.
- **Storage Method**: Stored the data in a CSV file for further analysis and usage.

### Extracted Data Sample

Below is a sample of the extracted data:

| No. | Company | Industry | Revenue (by US$ billion) | Headquarters |
| --- | ------- | -------- | ------------------------ | ------------ |
| 1   | Apple   | Electronics, telecommunications equipment | 274.515 | United States |
| 2   | Toyota Group | Engineering, various | 256.721 | Japan |
| 3   | Volkswagen Group | Automotive | 253.965 | Germany |
| 4   | Samsung Electronics | Electronics, various | 200.734 | South Korea |
| 5   | Foxconn | Electronics | 181.945 | Taiwan |
