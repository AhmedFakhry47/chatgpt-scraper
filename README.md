# chatgpt-scraper
This project builds an autonomous agent capable of fetching user-level order details from Coupang's website. The agent uses a combination of GPT-3.5-turbo-0125 for parsing and extracting text information from HTML content, Selenium WebDriver for web navigation, and BeautifulSoup for HTML parsing. The extracted order details are saved in a JSON file.

## Features
- **Web Automation**: Uses Selenium to navigate the Coupang website, log in, and fetch order pages.
- **HTML Parsing**: Utilizes BeautifulSoup to assist in parsing HTML content.
- **Text Extraction**: Employs OpenAI's GPT model to extract order details from HTML.
- **Data Storage**: Saves the extracted order details in a structured JSON format.

## Requirements

- Python 3.6+
- Selenium
- BeautifulSoup
- OpenAI API Key
- WebDriver for your preferred browser (Chrome in this example)

## Installation

1. Clone this repository to your local machine.

    ```sh
    git clone <repository_url>
    cd <repository_folder>
    ```

2. Install the required Python packages.

    ```sh
    pip install openai selenium webdriver-manager bs4 chromedriver-autoinstaller
    ```

3. Ensure you have the appropriate WebDriver for your browser. This example uses Chrome.

4. Obtain an OpenAI API key from the OpenAI website.

5. Install Chrome WebDriver if not already installed:

    ```sh
    chromedriver-autoinstaller.install()
    ```


## Script Overview

The script is divided into several sections:

- **Imports**: Necessary libraries and modules are imported.
- **Web Driver Setup**: Configuration and setup for Selenium WebDriver.
- **Parameters**: Configuration parameters for the Coupang website and agent prompts.
- **Utility Functions**: Helper functions for saving JSON and HTML files.
- **Agent Functions**: Core functions to fetch, parse, and extract order details.
- **Main Function**: `automated_agent` integrates all components to perform the entire process.
