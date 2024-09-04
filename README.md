Amazon Mobile Phones Scraper
This project is a web scraper for extracting data from Amazon's mobile phones and accessories section. It uses Python with the Selenium library to automate browsing and data extraction. The extracted data is saved to a CSV file.

Prerequisites
Python 3.x
Selenium
Chrome WebDriver
Pandas
Numpy
Installation
Install the necessary Python libraries using pip:

bash
Copy code
pip install pandas numpy selenium webdriver-manager
Ensure you have Google Chrome installed, as the script uses ChromeDriver for Selenium automation.

Usage
Run the script: The script initializes a Selenium WebDriver session and navigates to the Amazon Egypt website's electronics section to scrape mobile phone data.

Scraping Process:

The script clicks through various categories and filters on Amazon to find the mobile phones section.
It iterates through the available pages and extracts details such as:
Full Name
Brand Name
Operating System
CPU Model
Price Before Sale
Price After Sale
Storage Capacity
RAM
Rating 
Number of Ratings
Purchased Last Month
Device Image URL
Reviews
About this Phone
Output: The extracted data is stored in a Pandas DataFrame and then exported to a CSV file named Mobiles & accessories.csv.

Notes
Make sure your ChromeDriver is compatible with your installed Chrome browser version.
The script is configured for Amazon Egypt (amazon.eg) and might require adjustments for other regions.
Known Issues
The script uses hardcoded XPaths, which may break if Amazon updates its website layout.
Some elements might not be found, leading to exceptions. The script attempts to handle these by using try-except blocks.
Make sure to respect Amazon's terms of service regarding web scraping.
License
This project is licensed under the MIT License.

