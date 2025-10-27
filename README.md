# 🎬 IMDb Top Rated Movies Scraper

This Python script scrapes the Top Rated Movies list from IMDb and saves the extracted details — Movie Name, Year of Release, and IMDb Rating — into an Excel file.

## 📘 Project Overview

The script performs the following steps:

Sends an HTTP request to IMDb’s Top Rated Movies page.

Parses the page using BeautifulSoup to extract movie details.

Writes the extracted data into an Excel sheet using openpyxl.

Saves the final output as IMDB Movie Rating.xlsx.

### 🧠 Technologies Used

Library	----------------------------Purpose

requests----------------------------	Sends HTTP requests to fetch IMDb webpage data

BeautifulSoup (bs4)	--------------------Parses and extracts structured data from HTML

openpyxl-----------------------------	Creates and writes data into an Excel file

⚙️ Installation

Before running the script, make sure the required dependencies are installed.

You can install them via pip:
```bash
pip install requests beautifulsoup4 openpyxl
```

🚀 How to Run

Clone this repository or download the script file.

Open a terminal or command prompt in the project directory.

Run the script using:
```bash
python imdb_scraper.py
```

After successful execution, check for the output file:

IMDB Movie Rating.xlsx

### 📂 Output Example

Movie Rank & Name	Year of Release	IMDB Rating

The Shawshank Redemption	1994	9.3

The Godfather	1972	9.2

The Dark Knight	2008	9.0

- (Note: Actual results may vary as IMDb updates its list.)

### 🛠️ Error Handling

The script uses try-except blocks to catch network or parsing errors.

It also includes a User-Agent header to mimic a real browser request, preventing request blocking by IMDb.

### 📄 Output File

- File Name: IMDB Movie Rating.xlsx

- Sheet Name: Top rated Movies

Columns:

- Movie Rank & Name

- Year of Release

IMDb Rating

⚠️ Disclaimer

This project is intended for educational purposes only.

IMDb content is subject to copyright, and scraping should be done responsibly and within the website’s terms of service.

💡 Future Enhancements

Add movie rank extraction.

Include movie genre, director, or runtime.

Export data to CSV or JSON formats.

Automate periodic scraping with cron jobs or Airflow.
