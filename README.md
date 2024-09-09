# Email-Scarper

**Email Scraper** is a Python tool designed to extract email addresses from a target website. The tool navigates through links found on the provided website, collects emails, and displays them in the terminal.

## Features

- **Web Scraping**: Utilizes the `BeautifulSoup` library to parse HTML and find links on a webpage.
- **Email Extraction**: Uses regular expressions to identify and extract email addresses from the webpage.
- **Recursive Crawling**: Automatically follows links from the initial page and scrapes them as well.
- **Limit Control**: Includes a loop limit to avoid infinite crawling.
- **Error Handling**: Catches common exceptions such as connection errors and invalid URLs.

## Usage

### 1. Installation
Make sure you have Python 3 installed on your machine.

Install the necessary dependencies:
```bash
pip install requests beautifulsoup4
```
### 2. Running the Tool

Clone the repository:
```bash
    git clone https://github.com/your-username/email-scraper.git
```

