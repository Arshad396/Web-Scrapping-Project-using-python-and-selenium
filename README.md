# 📊 Yahoo Finance Stocks Scraper

A Python-based web scraper that extracts **real-time Most Active stock data** from [Yahoo Finance](https://finance.yahoo.com/), cleans it, and exports the results to an Excel file. This project uses Selenium for browser automation and pandas for data handling.

---

## 🚀 Features

- ✅ Navigates Yahoo Finance through automated browser control.
- ✅ Scrapes key stock data across **multiple pages**, including:
  - 🏷️ Stock Name and Symbol
  - 💵 Current Price (USD)
  - 📈 Price Change
  - 📊 Volume (in Millions)
  - 🧾 Market Capitalization (in Billions)
  - 📉 Price-to-Earnings (P/E) Ratio
- ✅ Cleans and processes raw data for better readability and analysis.
- ✅ Saves the structured data to an `.xlsx` file.

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Selenium** (for web scraping and automation)
- **pandas & NumPy** (for data cleaning and transformation)
- **ChromeDriver** (for controlling Chrome browser)

---

## 📁 Project Structure

```
├── 01. stocks-scraper.py              # Initial procedural version of the scraper
├── 02. restructured-stocks-scraper.py # Refactored class-based version (recommended)
├── yahoo_finance-stocks.xlsx          # Output Excel file (auto-generated)
```

---

## 📦 How to Run the Project

### 1. Install Dependencies

Make sure you have Python installed, then run:

```bash
pip install selenium pandas numpy openpyxl
```

### 2. Set Up ChromeDriver

- Download [ChromeDriver](https://chromedriver.chromium.org/downloads)
- Ensure the version matches your installed Chrome browser
- Add it to your system PATH or place it in the project folder

### 3. Run the Scraper

Use the refactored version:

```bash
python 02.\ restructured-stocks-scraper.py
```

This will launch a Chrome window, navigate to Yahoo Finance, extract the stock data, clean it, and save it to `yahoo_finance-stocks.xlsx`.

---

## 📌 Notes

- Dynamic menus on Yahoo Finance are handled using simulated hover actions.
- Data is extracted across all available pages using the "Next" button.
- Ensure a stable internet connection and GUI environment to run the scraper.

---

## 📤 Output Sample

An Excel file (`yahoo_finance-stocks.xlsx`) with columns like:

| Symbol | Name | Price (USD) | Change | Volume (M) | Market Cap (B) | P/E Ratio |
|--------|------|-------------|--------|------------|----------------|-----------|

---

## 🤝 Contributions

Feel free to fork, modify, and submit pull requests. All improvements and suggestions are welcome!

---

## 📜 License

This project is licensed under the MIT License.
