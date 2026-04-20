## 🌐📘 Project: Wikipedia Scraper

---

### ✨ Overview

The **Wikipedia Scraper** is a simple yet powerful Python project that automates the process of fetching information from Wikipedia.
It takes a person’s name as input, intelligently finds their Wikipedia page using Google search, extracts useful content, and saves it into a text file.

---

### 🎯 Objective

✔ Automate Wikipedia data extraction
✔ Handle misspelled or partial inputs
✔ Store clean, readable content locally

---

### 🧰 Tech Stack

* 🐍 Python 3.x
* 🌍 `requests` – for HTTP requests
* 🍲 `BeautifulSoup` – for HTML parsing
* 📊 `pandas` – *(optional)* for data handling

---

### ⚙️ How It Works

🔹 **1. User Input**
User enters the name of a person

🔹 **2. Smart Search**
A Google search URL is created by appending **"Wikipedia"**
➡ Handles spelling mistakes automatically

🔹 **3. Fetch Results**

* Sends request to Google
* Parses HTML using BeautifulSoup

🔹 **4. Extract Wikipedia Link**

* Scans `<div>` and `<a>` tags
* Finds first link containing `en.wikipedia.org`

🔹 **5. Clean URL**

* Removes unnecessary Google redirect data
* Extracts the actual Wikipedia link

🔹 **6. Scrape Data**

* Sends request to Wikipedia page
* Extracts all paragraph (`<p>`) content

🔹 **7. Save Output**

* Stores data in a `.txt` file
* File saved in current working directory

---

### 📂 Output

📄 A text file (e.g., `Mahatma_Gandhi.txt`) containing:

* Clean Wikipedia paragraphs
* Readable and structured text

---

### ⚠️ Limitations

⚡ Depends on Google’s page structure (can change)
⚡ May occasionally pick incorrect search results
⚡ Extracts only paragraph text (no images/tables)

---
### 🧠 Conclusion

This project is a great starting point for learning **web scraping**. It combines real-world techniques like search automation, HTML parsing, and file handling into a practical and useful application.

---

⭐ *Simple idea. Powerful learning. Real-world application.*
