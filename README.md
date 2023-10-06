# email-scraper
This Python script is a simple web scraper designed to find email addresses on a given website. It uses BeautifulSoup for HTML parsing and requests for making HTTP requests.

## How to Use

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. Install the required dependencies:

    ```bash
    pip install beautifulsoup4 requests
    ```

3. Run the script:

    ```bash
    python scraper.py
    ```

   Follow the prompts to enter the target URL for scanning.

## Features

- Extracts email addresses from the target website.
- Handles relative and absolute URLs.
- Gracefully handles interruptions (Ctrl+C).

## Code Explanation

The script follows these main steps:

1. **User Input:**
   - You'll be prompted to enter the target URL.

2. **Initialization:**
   - URLs and data structures are initialized.

3. **Main Loop:**
   - Processes URLs until none are left or a limit is reached.

4. **Extracting Emails:**
   - Uses a regular expression to find email addresses.

5. **Parsing HTML:**
   - Utilizes BeautifulSoup for HTML parsing.

6. **Processing Anchor Tags:**
   - Extracts links from anchor tags and adds new URLs for processing.

7. **Interrupt Handling:**
   - Gracefully handles interruptions.

8. **Printing Emails:**
   - Outputs the unique email addresses found.

Feel free to modify and enhance the script to suit your specific needs!

## Notes

- The script has a limit of processing 100 URLs to avoid excessive crawling.
- If you encounter issues, check your internet connection and ensure the target website allows web scraping.
