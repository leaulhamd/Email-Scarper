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

Navigate to the project directory and run the script:
```bash
python3 email-scraper.py
```

Enter the target URL when prompted:
```bash
[+] Enter Target URL To Scan: https://example.com
```

### 3. Output
The tool will start crawling the website and display any email addresses it finds:
```bash
Found emails: {'info@example.com', 'contact@domain.com'}
```

### Example
Below is an example of how the tool works:
```bash
#############################################
#                                           #
#        Email-Scarper By M033n             #
#                                           #
#############################################

[+] Enter Target URL To Scan: https://example.com
[1] Processing https://example.com
Found emails: {'info@example.com'}
[2] Processing https://example.com/contact
Found emails: {'contact@domain.com'}
```

### Limitations
- This tool can only scrape public, accessible content from the given URL.
- It does not handle CAPTCHA or other anti-scraping measures.
- The script is limited to processing 100 URLs by default to prevent infinite crawling.

### License
This project is licensed under the MIT License.
