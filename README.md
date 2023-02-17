# Web_scraping - Extracting Information of Github Topics 
web scraping is a automatic method to obtain large amounts of data from websites. Most of this data is unstructured data in an HTML format which is then converted into structured data in a spreadsheet or a database.

# Steps Followed 
1. import requests which allows to send HTTP requests using python and then the HTTP request returns a Response Object with all the response data (content, encoding, status, etc).
2. requests.get('https://github.com') sends a GET method request to the github url and print the content of page in the HTML form using requests.text  method.
3. We use bs4, BeautifulSoup Python library for pulling data out of HTML and XML files.
4. Parse the content into BeautifulSoup and iterate the topics titles by class name using doc.findall() method similary, we did for their respective descriptions and topics page link.
5. Created a list of extracted topics titles, their description and links.
6. Converted the lists in a dataframe using pandas. 
7. Created a CSV files from extracted information.
