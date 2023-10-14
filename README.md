# Stock-Image-Scraper
## Discription :
The provided code is a web scraping script designed to extract data from a web page and save it to a CSV file. It utilizes the Python programming language and several libraries for this purpose. Here's a breakdown of the code:

## Libraries:

numpy (np): A library for numerical operations in Python.
pandas (pd): A data manipulation and analysis library that helps create and manipulate data in a structured format.
BeautifulSoup: A Python library for web scraping that allows you to parse HTML or XML documents and extract data from web pages.
selenium: A web testing library used to automate web browser interactions. In this code, it's used to open the web page and retrieve its source.
chromedriver_binary: A package that provides the ChromeDriver executable for Selenium.
Coding Language:

The code is written in Python, a versatile and powerful programming language commonly used for web scraping, data analysis, and automation.

## Code Overview:

The code starts by importing necessary libraries.

It specifies the URL ('https://stock-pictures.netlify.app') that is to be scraped.

The Chrome WebDriver is initialized using Selenium to open the specified URL.

BeautifulSoup is used to parse the HTML content of the web page.

A list called 'data' is created to store the scraped information.

The script loops through all the HTML elements with the class 'container'. Inside the loop:

It checks if the image source does not contain 'gif'.
Extracts the image link.
Extracts tags, splits them into a list, and removes duplicates.
Extracts the number of likes and comments.
The extracted data is appended to the 'data' list.

The collected data is used to create a Pandas DataFrame named 'df' with columns 'Link', 'Tags', 'Likes', and 'Comments'.

The script checks for any missing data (null values) and displays the DataFrame.

Finally, it saves the DataFrame to a CSV file named 'data.csv'.

The code provides a practical example of web scraping, data extraction, and data manipulation using Python and related libraries. It's a valuable tool for collecting and analyzing data from web pages.
