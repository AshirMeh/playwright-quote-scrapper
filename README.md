Run the Scraper

    python main.py

    Output
        The scraped data is saved in a file named quotes.csv in the root directory.
        Each row contains:
            Quote text
            Author name
            Tags
            Author details (name, DOB, location, and bio)

Code Highlights
Scraping Workflow

    The scraper navigates to the homepage and validates the page's title.
    It extracts the top tags and iterates through their respective pages.
    It handles pagination dynamically, collecting quotes and their metadata.

Error Handling

    Timeout exceptions and missing elements are handled gracefully.
    Errors during individual quote processing do not interrupt the scraping process.
