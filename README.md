# Currency Converter

A simple currency converter web app that shows live exchange rates for 200+ currencies.

![Currency Converter](https://img.shields.io/badge/Currency%20Converter-v1.0-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![HTML](https://img.shields.io/badge/HTML5-orange)
![CSS](https://img.shields.io/badge/CSS3-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## What is this project?

This is a beginner-friendly currency converter that helps you convert money from one currency to another using real exchange rates.

Example: Convert 100 US Dollars to Indian Rupees instantly.

---

## Features

- Convert between 200+ currencies
- Shows country flags with each currency
- Swap currencies with one click
- Works on mobile and desktop
- Free to use - no API key needed

---

## How to Use

1. Pick a currency from the "From" dropdown
2. Pick a currency from the "To" dropdown  
3. Type the amount you want to convert
4. Click the "Get Exchange Rate" button
5. See your converted amount instantly

---

## How the Code Works (For Beginners)

### HTML (index.html)
This is the structure of the page - the input box, dropdowns, and button.

### CSS (style.css)
This makes everything look nice - colors, spacing, and layout.

### JavaScript (src.js)
This is the brain of the app. It:
- Fetches live exchange rates from an API
- Updates flags when you change currency
- Calculates the converted amount
- Shows the result on the page

### Currency Codes (codes.js)
This file contains a list of all currencies with their country codes.

Examples:
- "USD" goes with "US" for USA flag
- "INR" goes with "IN" for India flag
- "EUR" goes with "FR" for France flag

---

## APIs Used

### Exchange Rate API
This API gives us the latest exchange rates.

URL Format:
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/{currency}.json

Example: https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/usd.json

When we visit this URL, we get data with all exchange rates for USD.

### Flags API
This API gives us country flags.

URL Format:
https://flagsapi.com/{country_code}/flat/64.png

Examples:
- https://flagsapi.com/US/flat/64.png for USA flag
- https://flagsapi.com/IN/flat/64.png for India flag
- https://flagsapi.com/GB/flat/64.png for UK flag

---

## Project Files

currency-converter/
├── index.html    # Web page structure
├── style.css     # Styling and design
├── src.js        # Main JavaScript code
├── codes.js      # Currency list
└── README.md     # This file

---

## What I Learned Making This

1. How to use async/await to fetch data from APIs
2. How to work with JSON data
3. How to create dropdown options dynamically with JavaScript
4. How to handle form submissions
5. How to use template literals (backticks) for strings
6. How to access API data like data.usd.inr

---

## Key JavaScript Concepts Used

async/await - To fetch data from the API
fetch() - To make API requests
addEventListener() - To respond to button clicks and dropdown changes
for...in loop - To loop through all currencies
document.querySelector() - To select elements from the page
toLowerCase() - To convert USD to usd for the API
toFixed() - To show only 2 decimal places
Template literals - To build strings with variables

---

## Common Beginner Questions

Q: Why do we use toLowerCase()?
A: The API expects lowercase currency codes (like "usd"), but our dropdown shows uppercase (like "USD").

Q: Why do we use await?
A: Fetching data from the internet takes time. await tells JavaScript to wait for the response.

Q: What is JSON?
A: JSON is a format for sending data. It looks like a JavaScript object with key-value pairs.

Q: Why no API key?
A: This API is completely free and open source. No registration needed.

---

## Run This Project

1. Download all files
2. Open index.html in your browser
3. No installation needed!

Or clone it:
git clone https://github.com/YOUR_USERNAME/currency-converter.git

---

## Future Improvements

- Add more cryptocurrencies
- Show exchange rate history
- Add dark mode
- Save favorite currency pairs

---

