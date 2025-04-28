# Tara_Hulcome_IMT542_I4
For this I4 assignment, I experimented with four different information structures / access technologies. Three of these attempts produced successful results (i.e., I was able to print a sample of text or data), and one attempt was unsuccessful (I've included the results as it was still interesting to test the process). 

A summary of the process for each example is listed below, and the full Python code is attached in IMT_542_I4_Tara_Hulcome.ipynb

## Example 1

•	**Task**: Retrieve sample (10 lines) of HTML text from an information architecture website blog. 

•	**Source UR**L: https://www.uxmatters.com/mt/archives/2016/11/the-name-of-the-practice-is-information-architecture.php

•	**Information structure**: HTML (PHP script).

•	**Access technology**: HTML parser using BeautifulSoup.

•	**Result**: Successful extraction.

•	**Pros**: It’s easy and fast to use BeautifulSoup (with the assistance of Google Gemini AI) to scrape information from publicly accessible websites.

•	**Cons**: The resulting output is quite messy and dense. It requires further structuring to improve readability. 



## Example 2

•	**Task**: Extract a sample of text from the executive summary of a PDF file (Australia’s Digital Trade Strategy).

•	**Source URL**: https://www.dfat.gov.au/sites/default/files/digital-trade-strategy.pdf

•	**Information structure**: PDF file 

•	**Access technology**: Manual file download via website, uploaded as local file to Google CoLab, and extracted text sample using PyPDF2 package.

•	**Result**: Successful extraction.

•	**Pros**: Easy to use PyPDF2 package to scrape text from PDF file – testing this method is very useful for my final project.

•	**Cons**: This method was more labor intensive, as I first needed to manually download the PDF file from the DFAT website before uploading as a local file to Google CoLab and then extracting text with Python (with assistance of Google Gemini AI).



## Example 3

•	**Task**: Retrieve details of the last 10 workbooks associated with a Tableau Public username. Return as a CSV file.

•	**Source URL**: https://public.tableau.com/app/profile/philip.hulcome1964/vizzes 

•	**Information structure**: CSV file. 

•	**Access technology**:  API connection over HTTP to Tableau Public website.

•	**Result**: Unsuccessful. Returned ‘No workbooks found’ result, and my troubleshooting couldn’t fix the error.

•	**Pros**: N/A

•	**Cons**: Based on my troubleshooting efforts: the error may have been because Tableau Public loads workbook content dynamically, so BeautifulSoup couldn’t retrieve dynamic elements. I attempted to use Selenium instead, with no luck. This task was clearly beyond my coding ability :(



## Example 4

•	**Task**: Retrieve sample of data from a CSV file (Harmonized Tariff Schedule of the United States, 2025) hosted on Data.Gov website.

•	**Information** **structure**: Downloadable CSV file hosted on URL.

•	**Source URL**: https://www.usitc.gov/sites/default/files/tata/hts/hts_2025_revision_10_csv.csv 

•	**Access** **technology**: Pandas package to parse CSV file.

•	**Result**: Successful.

•	**Pros**: It’s easy to use Pandas (with assistance of Google Gemini AI) to extract sample data from CSV files.

•	**Cons**: Pandas loaded the entire file into its memory – which is not ideal for extremely large data files. 

